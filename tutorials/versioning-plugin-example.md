---
title: Versioning Plugin Example
source: Article
url: file:///C:/Program%20Files/Adobe%20Substance%203D%20Painter/resources/python-doc/plugins/versioning_plugin.html
author: Adobe Substance 3D Painter 12.1.4 bundled docs
ingested: 2026-09-04
app: "Substance 3D Painter"
version: "12.1.4 (Python API 0.3.5) -- bundled docs, resources/python-doc"
tags: [python-scripting, python-api, plugin, ui-plugin, export, painter-12, intermediate]
extraction_status: complete
frames_dir: tutorials/frames/versioning-plugin-example/
frame_count: 0
frame_status: skipped
uncertainty_frames: []
---

# Versioning Plugin Example

**Source:** [Article](file:///C:/Program%20Files/Adobe%20Substance%203D%20Painter/resources/python-doc/plugins/versioning_plugin.html)
**Author:** Adobe Substance 3D Painter 12.1.4 bundled docs
**Duration:** unknown | 1 section(s)

---

## Raw Data (for Claude Code extraction)

Frame capture was skipped for this ingest (--skip-video). Text-only extraction.


### Full Content [0:00]
**Transcript:** Versioning Plugin  versioning_plugin.py  """This is a skeleton for a plugin to integrate Substance 3D Painter with a versioning system. This plugin listens for project events and provides a custom export action. All methods whose name starts with ``on_`` can be customized to integrate the application with a versioning system. """ from PySide6 import QtWidgets , QtCore , QtGui import substance_painter.export import substance_painter.project import substance_painter.textureset import substance_painter.ui class VersioningPlugin : def __init__ ( self ): # Create a dock widget to report plugin activity. self . log = QtWidgets . QTextEdit () self . log . setReadOnly ( True ) self . log . setWindowTitle ( "Projects Versioning" ) substance_painter . ui . add_dock_widget ( self . log ) # Create a custom export action in the FILE application menu. self . export_action = QtGui . QAction ( "Versioned Export..." ) self . export_action . triggered . connect ( self . export_textures ) substance_painter . ui . add_action ( substance_painter . ui . ApplicationMenu . File , self . export_action ) # Subscribe to project related events. connections = { substance_painter . event . ProjectOpened : self . on_project_opened , substance_painter . event . ProjectCreated : self . on_project_created , substance_painter . event . ProjectAboutToClose : self . on_project_about_to_close , substance_painter . event . ProjectAboutToSave : self . on_project_about_to_save , substance_painter . event . ProjectSaved : self . on_project_saved , } for event , callback in connections . items (): substance_painter . event . DISPATCHER . connect ( event , callback ) def __del__ ( self ): # Remove all added UI elements. substance_painter . ui . delete_ui_element ( self . log ) substance_painter . ui . delete_ui_element ( self . export_action ) def on_project_opened ( self , e ): self . log . append ( "Project ` {} ` opened." . format ( substance_painter . project . name ())) ################################## # Add custom integration code here def on_project_created ( self , e ): self . log . append ( "New project created." ) ################################## # Add custom integration code here def on_project_about_to_close ( self , e ): self . log . append ( "Project ` {} ` closed." . format ( substance_painter . project . name ())) ################################## # Add custom integration code here def on_project_about_to_save ( self , e ): self . log . append ( "Project will be saved in ` {} `." . format ( e . file_path )) ################################## # Add custom integration code here def on_project_saved ( self , e ): self . log . append ( "Project ` {} ` saved." . format ( substance_painter . project . name ())) ################################## # Add custom integration code here def on_export_about_to_start ( self , export_configuration ): self . log . append ( "Export textures." ) ################################## # Add custom integration code here def on_export_finished ( self , res ): self . log . append ( res . message ) self . log . append ( "Exported files:" ) for file_list in res . textures . values (): for file_path in file_list : self . log . append ( " {} " . format ( file_path )) ################################## # Add custom integration code here def on_export_error ( self , err ): self . log . append ( "Export failed." ) self . log . append ( repr ( err )) ################################## # Add custom integration code here @QtCore . Slot () def export_textures ( self ): """Export base color of all Texture Sets to a location choosen by the user.""" json_config = dict () # Set export directory. export_path = QtWidgets . QFileDialog . getExistingDirectory ( substance_painter . ui . get_main_window (), "Choose export directoty" ) if not export_path : # Export aborted. return json_config [ "exportPath" ] = export_path + "/" + substance_painter . project . name () # Export configuration. json_config [ "exportShaderParams" ] = False channels = [] for channel in "RGBA" : channels . append ({ "destChannel" : channel , "srcChannel" : channel , "srcMapType" : "DocumentMap" , "srcMapName" : "BaseColor" }) json_config [ "exportPresets" ] = [{ "name" : "OnlyBaseColorExamplePreset" , "maps" : [{ "fileName" : "$textureSet_BaseColor" , "channels" : channels , }] }] json_config [ "exportParameters" ] = [{ "parameters" : { "fileFormat" : "png" , "bitDepth" : "8" , "dithering" : True , "paddingAlgorithm" : "infinite" } }] # Create the list of Texture Sets to export. json_config [ "exportList" ] = [] for texture_set in substance_painter . textureset . all_texture_sets (): try : stack = texture_set . get_stack () channel = stack . get_channel ( substance_painter . textureset . ChannelType . BaseColor ) if channel . is_color (): json_config [ "exportList" ] . append ({ "rootPath" : texture_set . name (), "exportPreset" : "OnlyBaseColorExamplePreset" , }) except : pass # Do the export. self . on_export_about_to_start ( json_config ) try : res = substance_painter . export . export_project_textures ( json_config ) self . on_export_finished ( res ) except ValueError as err : self . on_export_error ( err ) VERSIONING_PLUGIN = None def start_plugin (): """This method is called when the plugin is started.""" global VERSIONING_PLUGIN VERSIONING_PLUGIN = VersioningPlugin () def close_plugin (): """This method is called when the plugin is stopped.""" global VERSIONING_PLUGIN del VERSIONING_PLUGIN if __name__ == "__main__" : start_plugin ()



---

## Structured Notes

### Core Technique
A complete, runnable plugin skeleton that wires all three halves of the API together: a docked Qt log widget, a custom **File** menu action, subscriptions to the five project lifecycle events, and a scripted texture export — written as the integration point for a versioning system.

### Summary
Adobe ships this as `versioning_plugin.py`, and it is the most useful single file in the bundled docs because it shows the *shape* of a real plugin rather than one call at a time. A `VersioningPlugin` class builds a read-only `QTextEdit` and registers it with `substance_painter.ui.add_dock_widget()`, adds a "Versioned Export..." `QAction` to `ApplicationMenu.File`, and connects five project events through `substance_painter.event.DISPATCHER`. Every handler is named `on_*` and left deliberately empty with a marked comment block — the documented seam where studio integration code goes. `__del__` tears the UI back down with `delete_ui_element()`, and module-level `start_plugin()` / `close_plugin()` satisfy the plugin contract. The export action builds a complete `json_config` by hand — export path, an inline preset packing R/G/B/A from the **BaseColor** document map, PNG/8-bit/dithering/infinite padding parameters, and an `exportList` assembled by walking `all_texture_sets()` and keeping the stacks whose BaseColor channel `is_color()`.

### Key Steps
1. **Build the UI in `__init__`:** create a read-only `QtWidgets.QTextEdit`, set its `windowTitle`, and register it with `substance_painter.ui.add_dock_widget(self.log)`.
2. **Add the menu action:** `QtGui.QAction("Versioned Export...")`, connect `triggered` to the export slot, then `substance_painter.ui.add_action(substance_painter.ui.ApplicationMenu.File, self.export_action)`.
3. **Subscribe to lifecycle events** by iterating a `{event_class: callback}` dict and calling `substance_painter.event.DISPATCHER.connect(event, callback)` — `ProjectOpened`, `ProjectCreated`, `ProjectAboutToClose`, `ProjectAboutToSave`, `ProjectSaved`.
4. **Write the `on_*` handlers** as the integration seam. Each logs and carries a `####` comment block for custom code. Note `on_project_about_to_save(e)` reads **`e.file_path`** off the event object — events carry payload.
5. **Tear down in `__del__`:** `substance_painter.ui.delete_ui_element()` for both the dock widget and the action. Skipping this leaves orphaned UI behind on unload.
6. **Ask the user for a destination** with `QtWidgets.QFileDialog.getExistingDirectory(substance_painter.ui.get_main_window(), ...)` — parenting to the main window is what `get_main_window()` is for — and abort quietly when the dialog returns empty.
7. **Compose the export config:** `exportPath` = chosen directory + project name; `exportShaderParams: False`; an inline `exportPresets` entry named `OnlyBaseColorExamplePreset` whose single map `$textureSet_BaseColor` maps each of R/G/B/A from `srcMapType: "DocumentMap"`, `srcMapName: "BaseColor"`; and `exportParameters` of `png` / `8`-bit / `dithering: True` / `paddingAlgorithm: "infinite"`.
8. **Build `exportList` defensively:** for each `substance_painter.textureset.all_texture_sets()`, `get_stack()`, `get_channel(ChannelType.BaseColor)`, and append `{"rootPath": texture_set.name(), "exportPreset": ...}` only when `channel.is_color()` — wrapped in `try/except` so a texture set without that channel is skipped rather than fatal.
9. **Run it through the plugin's own hooks:** call `on_export_about_to_start(json_config)`, then `substance_painter.export.export_project_textures(json_config)` inside `try/except ValueError`, passing the result to `on_export_finished(res)` (which walks `res.textures.values()` to log every written file) or the error to `on_export_error(err)`.
10. **Satisfy the plugin contract at module level:** a global instance created in `start_plugin()` and deleted in `close_plugin()`, plus an `if __name__ == "__main__": start_plugin()` for direct execution.

### Nodes / Tools / Settings
- **UI:** `substance_painter.ui.add_dock_widget()`, `add_action()`, `ApplicationMenu.File`, `get_main_window()`, `delete_ui_element()`.
- **Events:** `substance_painter.event.DISPATCHER.connect()`; `ProjectOpened`, `ProjectCreated`, `ProjectAboutToClose`, `ProjectAboutToSave` (payload `file_path`), `ProjectSaved`.
- **Export:** `substance_painter.export.export_project_textures(json_config)`; result fields `message`, `textures` (dict keyed by stack); raises `ValueError` on an invalid config.
- **Texture sets:** `substance_painter.textureset.all_texture_sets()`, `Stack.get_channel()`, `ChannelType.BaseColor`, `channel.is_color()`.
- **Qt:** PySide6 — `QtWidgets.QTextEdit`, `QtGui.QAction`, `QtWidgets.QFileDialog.getExistingDirectory`, `@QtCore.Slot()`.
- **Plugin contract:** module-level `start_plugin()` / `close_plugin()` holding a global instance.

### Difficulty
Intermediate

### Foundry App & Version
Substance 3D Painter 12.1.4, Python API 0.3.5. UI code is **PySide6** — an older plugin written against PySide2 will not import unchanged.

### Tags
`python-scripting`, `python-api`, `plugin`, `ui-plugin`, `export`, `painter-12`, `intermediate`

---

## Related Tutorials
- [substance_painter_plugins Module](substance-painter-plugins-module.md) — the `start_plugin`/`close_plugin` contract this file implements.
- [Python API: ui Module](python-api-ui-module.md) — full reference for the dock/menu/toolbar calls used here.
- [Python API: event Module](python-api-event-module.md) — every event class this plugin connects to, plus the export events.
- [Python API: export Module](python-api-export-module.md) — the full `json_config` schema this plugin writes a minimal version of.

---

> **Provenance.** Ingested from the Python API documentation **bundled inside**
> Substance 3D Painter 12.1.4 on this machine
> (`C:\Program Files\Adobe Substance 3D Painter\resources\python-doc`, reached in
> the app via Help → scripting documentation). It is first-party Adobe
> documentation, but the `url:` is a local `file://` path and therefore not
> reachable from another machine — the public Experience League paths for the
> Python API redirect to a generic page, which is why the bundled copy is the
> source. Re-fetchable on any machine with Painter installed at the same path;
> the API version (`0.3.5`) is the thing to check before trusting a signature.
