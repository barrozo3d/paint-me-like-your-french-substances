---
title: substance_painter_plugins Module
source: Article
url: file:///C:/Program%20Files/Adobe%20Substance%203D%20Painter/resources/python-doc/plugins/substance_painter_plugins.html
author: Adobe Substance 3D Painter 12.1.4 bundled docs
ingested: 2026-09-04
app: "Substance 3D Painter"
version: "12.1.4 (Python API 0.3.5) -- bundled docs, resources/python-doc"
tags: [python-scripting, python-api, plugin, painter-12, intermediate]
extraction_status: complete
frames_dir: tutorials/frames/substance-painter-plugins-module/
frame_count: 0
frame_status: skipped
uncertainty_frames: []
---

# substance_painter_plugins Module

**Source:** [Article](file:///C:/Program%20Files/Adobe%20Substance%203D%20Painter/resources/python-doc/plugins/substance_painter_plugins.html)
**Author:** Adobe Substance 3D Painter 12.1.4 bundled docs
**Duration:** unknown | 1 section(s)

---

## Raw Data (for Claude Code extraction)

Frame capture was skipped for this ingest (--skip-video). Text-only extraction.


### Full Content [0:00]
**Transcript:** substance_painter_plugins module  This module allows to manage the Substance 3D Painter Plugins: listing existing Plugins, loading or unloading a given Plugin, etc. A Substance 3D Painter Plugin is a standard Python module, placed in a path added to substance_painter_plugins.path , which can use the Substance 3D Painter Python API to do certain tasks. Example import importlib import substance_painter_plugins # Get the list of available Plugin names: all_plugins_names = substance_painter_plugins . plugin_module_names () for name in all_plugins_names : print ( name ) # Load the "hello world" Plugin: plugin = importlib . import_module ( "hello_plugin" ) # Start the Plugin if it wasn't already: if not substance_painter_plugins . is_plugin_started ( plugin ): substance_painter_plugins . start_plugin ( plugin ) substance_painter_plugins. path = []  A list of strings that specifies the search path for plugins. Initialized from SUBSTANCE_PAINTER_PLUGINS_PATH environment variable, Substance 3D Painter installation directory and Substance 3D Painter user resources directory. You need to call explicitly substance_painter_plugins.update_sys_path after updating this variable. A plugins directory is expected to contain three subdirectories, automatically added to sys.path : plugins : Modules that are loaded as optional components. startup : Modules that are always loaded at application startup. modules : Utility modules, shared across plugins. Modules in plugins/ and startup/ directories are expected to have a start_plugin() and a close_plugin() methods, respectively called after loading the module and before unloading it. Modules added in plugins/ directory take precedence over modules added in startup/ directory. Type : list substance_painter_plugins. plugins = {}  Currently started plugins. Type : dict substance_painter_plugins. start_plugin ( module )  Start the given Substance 3D Painter plugin. Parameters : module – A Python module that is expected to have a start_plugin method. substance_painter_plugins. close_plugin ( module , gc_collect = True )  Close the given Substance 3D Painter plugin. Parameters : module – A Python module that is expected to have a close_plugin method. gc_collect – Run a full garbage collection if set to True. substance_painter_plugins. is_plugin_started ( module )  Check if the given plugin is currently started. Parameters : module – A Python module. Returns : True if the given module is currently started, False otherwise. substance_painter_plugins. reload_plugin ( module )  Reload a plugin and start it. Read importlib.reload(module) documentation for possible caveats. See start_plugin() and close_plugin() for details about starting and closing a plugin. If the plugin has a reload_plugin method, it will be executed after closing and before restarting the plugin. The purpose of reload_plugin method is to reload manually all sub-modules the plugin depends on (in case the plugin is a Python package for example). Parameters : module – A Python module. Returns : The reloaded plugin module. See also start_plugin() , close_plugin() , importlib.reload(module) documentation . substance_painter_plugins. startup_module_names ( )  List the names of the available startup modules. Returns : The names of all the available startup modules. Return type : list[str] substance_painter_plugins. plugin_module_names ( )  List the names of the available plugins modules. Returns : The names of all the available plugins modules. Return type : list[str] substance_painter_plugins. load_startup_modules ( )  Load all startup modules. substance_painter_plugins. close_all_plugins ( )  Close all started plugins. substance_painter_plugins. update_sys_path ( )  Update sys.path according to substance_painter_plugins.path and SUBSTANCE_PAINTER_PLUGINS_PATH environment variable.



---

## Structured Notes

### Core Technique
A Substance 3D Painter plugin is an ordinary Python module placed on `substance_painter_plugins.path`, exposing `start_plugin()` and `close_plugin()`; the `substance_painter_plugins` module lists, starts, stops and reloads them.

### Summary
This is the plugin host: the module that discovers plugin modules, tracks which are running, and loads or unloads them. `substance_painter_plugins.path` is a list of search paths initialised from the **`SUBSTANCE_PAINTER_PLUGINS_PATH`** environment variable plus the Painter installation directory and the user resources directory — and changing it does nothing until `update_sys_path()` is called explicitly. Each plugins directory is expected to hold **three subdirectories**, all added to `sys.path`: `plugins/` (optional components), `startup/` (always loaded at application startup), and `modules/` (shared utility code). Modules in `plugins/` and `startup/` must define `start_plugin()` and `close_plugin()`, called after load and before unload respectively, and **`plugins/` takes precedence over `startup/`** when the same module name appears in both.

### Key Steps
1. Put the plugin `.py` module (or package) in a `plugins/` subdirectory of a path on `substance_painter_plugins.path`.
2. To add a search path from script, append to `substance_painter_plugins.path` and then call **`update_sys_path()`** — the update is not automatic. To add one from outside the app, set **`SUBSTANCE_PAINTER_PLUGINS_PATH`**.
3. Give the module a **`start_plugin()`** and a **`close_plugin()`**; Painter calls them after loading and before unloading.
4. Enumerate what is available with **`plugin_module_names()`** (from `plugins/`) and **`startup_module_names()`** (from `startup/`).
5. Import a plugin by name with `importlib.import_module("hello_plugin")`, then guard with **`is_plugin_started(module)`** before calling **`start_plugin(module)`** — the pattern in the module's own example.
6. Stop one with **`close_plugin(module, gc_collect=True)`** (a full garbage collection runs when `gc_collect` is True), or stop everything with **`close_all_plugins()`**.
7. **Iterate during development with `reload_plugin(module)`** — it closes, reloads and restarts. If the plugin defines its own `reload_plugin` method, that runs *between* close and restart, which is where a package reloads its own sub-modules (plain `importlib.reload` will not).
8. `load_startup_modules()` loads everything in `startup/`; `substance_painter_plugins.plugins` is the dict of currently started plugins.

### Nodes / Tools / Settings
- **`substance_painter_plugins.path`** (list) — search paths; initialised from `SUBSTANCE_PAINTER_PLUGINS_PATH`, the install directory and the user resources directory.
- **Directory contract:** `plugins/` (optional, `start_plugin`/`close_plugin` required), `startup/` (always loaded at startup, same contract), `modules/` (shared utilities). `plugins/` wins over `startup/`.
- **`update_sys_path()`** — must be called after modifying `path`.
- **`start_plugin(module)`**, **`close_plugin(module, gc_collect=True)`**, **`is_plugin_started(module)`**, **`reload_plugin(module)`**, **`close_all_plugins()`**, **`load_startup_modules()`**.
- **`plugin_module_names()`**, **`startup_module_names()`** — discovery; **`plugins`** (dict) — what is running.
- Environment variable: **`SUBSTANCE_PAINTER_PLUGINS_PATH`**.

### Difficulty
Intermediate

### Foundry App & Version
Substance 3D Painter 12.1.4, Python API 0.3.5. (This skill's `App & Version` heading is shared with the Foundry-suite sibling skills; the app here is Adobe's.)

### Tags
`python-scripting`, `python-api`, `plugin`, `painter-12`, `intermediate`

---

## Related Tutorials
- [Versioning Plugin Example](versioning-plugin-example.md) — a complete plugin built on this contract, with `start_plugin`/`close_plugin` at the bottom of the file.
- [Python API: event Module](python-api-event-module.md) — what a started plugin subscribes to.
- [Python API: ui Module](python-api-ui-module.md) — what a started plugin adds to the interface.

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
