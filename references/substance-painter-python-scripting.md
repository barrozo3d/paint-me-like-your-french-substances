# Substance Painter Python API & Plugins

## Overview
Painter embeds a Python 3 interpreter and exposes a first-party `substance_painter` module (Adobe-maintained, documented at `adobedocs.github.io/painter-python-api`). Scripts run either as one-off snippets in the **Python Console** (Window → Views → Python Console) or as installed **plugins** (auto-loaded from the user plugins folder, with a UI entry under the Python menu).

## Key Submodules
- `substance_painter.project` — open/close/save projects, check `is_open()`, read project-level metadata.
- `substance_painter.textureset` — enumerate Texture Sets, read/write per-set properties, list/select channels.
- `substance_painter.layerstack` — read and mutate the layer stack: insert Fill/Paint/Group layers, set blend mode/opacity/visibility, get/set masks, add mask effects/generators programmatically.
- `substance_painter.resource` — query and import Shelf resources (materials, smart materials, generators, alphas) by URL/ID, useful for batch-applying an asset across many projects.
- `substance_painter.export` — trigger texture export using a named/config-defined export preset, headlessly (no dialog).
- `substance_painter.baking` — configure and trigger baking (mesh maps) from script, including per-Texture-Set bake settings, without opening the Baking dialog.
- `substance_painter.event` — subscribe to application events (`ProjectOpened`, `ExportTexturesEnded`, layer stack changes, etc.) so a plugin can react rather than poll.
- `substance_painter.ui` — add custom dock widgets, menu entries, and toolbar buttons using Qt (PySide2/PySide6 depending on Painter version) for a full custom panel.

## Plugin Structure
A minimal plugin is a folder (or single `.py`) placed in Painter's plugin directory containing:
```python
import substance_painter.event as event
import substance_painter.ui as ui

def start_plugin():
    # register UI, event callbacks, etc. — called once on load
    ...

def close_plugin():
    # unregister everything registered in start_plugin — called on unload/app close
    ...

if __name__ == "__main__":
    start_plugin()
```
Painter calls `start_plugin()`/`close_plugin()` by convention — omitting a clean `close_plugin()` (removing callbacks/widgets) is the most common cause of duplicate UI elements or dangling event handlers after a plugin reload during development.

## Common Automation Patterns
- **Batch export:** loop over multiple open/opened projects, call `substance_painter.export.export_project_textures(config)` per project with a preset (Unreal/Unity/custom) — used for asset-pack pipelines that shouldn't require manually clicking Export per asset.
- **Batch material application:** use `resource.list_resources()` / `resource.ResourceID` to look up a Smart Material by name, then `layerstack.insert_layer()` + apply it — automates "drop this smart material on every Texture Set" across a batch of meshes.
- **Headless-ish scripting:** Painter is not truly headless (no official CLI-only mode as of this writing), but scripts triggered via a plugin button or the Python Console can run project creation → baking → material application → export end-to-end without further manual clicks once started.

## Using External Modules
Painter's embedded Python can `import` pure-Python packages placed on its `sys.path` (see Adobe's "Using external modules" doc), but cannot easily install C-extension packages via pip into the embedded interpreter — for anything beyond the standard library plus pure-Python deps, prefer driving Painter from an external MCP/automation bridge (see the "Live Substance Painter Connection" section of `SKILL.md`) rather than fighting the embedded interpreter's package isolation.

## Common Gotchas
- API surface differs meaningfully between major Painter versions (the `substance_painter` module has grown across releases) — always check `references/version-tracker.md` and the live docs for the installed version before assuming a call exists.
- Layer stack mutations from script do not always auto-refresh every UI panel immediately — a manual redraw/selection-change may be needed to see the result while developing interactively.
- `substance_painter.export` requires a valid export preset/config dict; a malformed channel mapping fails silently or exports empty/black textures rather than raising an obvious error — verify output on a test asset first.
