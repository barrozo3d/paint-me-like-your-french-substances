---
title: Python API: ui Module
source: Article
url: file:///C:/Program%20Files/Adobe%20Substance%203D%20Painter/resources/python-doc/substance_painter/ui.html
author: Adobe Substance 3D Painter 12.1.4 bundled docs
ingested: 2026-09-04
app: "Substance 3D Painter"
version: "12.1.4 (Python API 0.3.5) -- bundled docs, resources/python-doc"
tags: [python-scripting, python-api, ui-plugin, painter-12, intermediate]
extraction_status: complete
frames_dir: tutorials/frames/python-api-ui-module/
frame_count: 0
frame_status: skipped
uncertainty_frames: []
---

# Python API: ui Module

**Source:** [Article](file:///C:/Program%20Files/Adobe%20Substance%203D%20Painter/resources/python-doc/substance_painter/ui.html)
**Author:** Adobe Substance 3D Painter 12.1.4 bundled docs
**Duration:** unknown | 1 section(s)

---

## Raw Data (for Claude Code extraction)

Frame capture was skipped for this ingest (--skip-video). Text-only extraction.


### Full Content [0:00]
**Transcript:** ui module  Entry points to customize Substance 3D Painter UI. class substance_painter.ui. UIMode ( value )  UI configurations enumeration. Members: Name Value Description Edition 1 Project edition mode Visualisation 2 (Iray) mode Baking 4 Baking mode Note The name used to define members is available as a string via the .name attribute (see python enum.Enum ). class substance_painter.ui. ApplicationMenu ( value )  Standard application menus enumeration. Members: Name Description File File menu Edit Edit menu Mode Mode menu Window Window menu Viewport Viewport menu Help Help menu Note The name used to define members is available as a string via the .name attribute (see python enum.Enum ). substance_painter.ui. show_main_window ( )  Show Substance 3D Painter main window in the windowing system and give it the focus. Raises : ServiceNotFoundError – If Substance 3D Painter has not started its UI service. substance_painter.ui. get_main_window ( ) PySide6.QtWidgets.QMainWindow  Get access to Substance 3D Painter main window. Returns : The application main window. Return type : PySide6.QtWidgets.QMainWindow Raises : ServiceNotFoundError – If Substance 3D Painter has not started its UI service. substance_painter.ui. get_layout ( mode : UIMode ) bytes  Get Substance 3D Painter layout state for the given UI mode. Parameters : mode ( UIMode ) – Selected UI mode. Returns : The layout state. Return type : bytes Raises : ServiceNotFoundError – If Substance 3D Painter has not started its UI service. substance_painter.ui. get_layout_mode ( layout : bytes ) UIMode  Get the Substance 3D Painter UI layout mode of a given state. Parameters : layout ( bytes ) – The layout state, obtained with get_layout() . Returns : The state associated UI mode. Return type : UIMode Raises : RuntimeError – In case of incorrect layout data. ServiceNotFoundError – If Substance 3D Painter has not started its UI service. substance_painter.ui. set_layout ( layout : bytes ) UIMode  Restore a Substance 3D Painter layout state optained with get_layout() . Parameters : layout ( bytes ) – The layout state to be restored. Returns : The restored UI mode. Return type : UIMode Raises : RuntimeError – In case of incorrect layout data. ServiceNotFoundError – If Substance 3D Painter has not started its UI service. substance_painter.ui. reset_layout ( mode : UIMode )  Reset Substance 3D Painter layout to default for a selected UI mode. Parameters : mode ( UIMode ) – Selected UI mode. Raises : ServiceNotFoundError – If Substance 3D Painter has not started its UI service. substance_painter.ui. add_dock_widget ( widget : PySide6.QtWidgets.QWidget , ui_modes : int = UIMode.Edition ) PySide6.QtWidgets.QDockWidget  Add a widget as a QDockWidget to the main window. If the widget has a windowIcon , it will be used as a quick button to easily reopen the QDockWidget when closed. If the widget has a unique objectName it will be used to properly save and restore the dock widget location and geometry. Parameters : widget ( PySide6.QtWidgets.QWidget ) – The widget to be added as a dock widget. ui_modes ( int , optional ) – A combination of UIMode flags. Returns : The corresponding dock widget. Return type : PySide6.QtWidgets.QDockWidget Raises : ServiceNotFoundError – If Substance 3D Painter has not started its UI service. substance_painter.ui. add_plugins_toolbar_widget ( widget : PySide6.QtWidgets.QWidget )  Add a widget to the plugins toolbar. Parameters : widget ( PySide6.QtWidgets.QWidget ) – The widget to be added. Raises : ServiceNotFoundError – If Substance 3D Painter has not started its UI service. substance_painter.ui. add_menu ( menu : PySide6.QtWidgets.QMenu )  Add the given menu to the application main window. Parameters : menu ( PySide6.QtWidgets.QMenu ) – The menu to be added. Raises : ServiceNotFoundError – If Substance 3D Painter has not started its UI service. substance_painter.ui. add_toolbar ( title : str , object_name : str , ui_modes : int = UIMode.Edition ) PySide6.QtWidgets.QToolBar  Create and add a toolbar to the application main window. Parameters : title ( str ) – The title of the toolbar. object_name ( str ) – The toolbar object name. A unique object name is mandatory for proper save and restore of the UI layout. ui_modes ( int ) – A combination of UIMode flags. Returns : The newly created toolbar. Return type : PySide6.QtWidgets.QToolBar Raises : ServiceNotFoundError – If Substance 3D Painter has not started its UI service. substance_painter.ui. add_action ( menu : ApplicationMenu , action : PySide6.QtGui.QAction )  Add the given action to the given application menu. This will clear the action tooltip. Parameters : menu ( ApplicationMenu ) – One of the predefined ApplicationMenu . action ( PySide6.QtGui.QAction ) – The action to be added. Raises : ServiceNotFoundError – If Substance 3D Painter has not started its UI service. substance_painter.ui. delete_ui_element ( element : PySide6.QtWidgets.QWidget )  Delete a UI element. The element passed as parameter is deleted. After that, any attempt to call a method on element will throw an exception. Parameters : element ( PySide6.QtWidgets.QWidget ) – The UI element to delete. substance_painter.ui. get_current_mode ( ) UIMode  Get the current UI mode. Returns : The current UI mode. Return type : UIMode Raises : ServiceNotFoundError – If Substance 3D Painter has not started its UI service. substance_painter.ui. switch_to_mode ( mode : UIMode ) None  Switch to some UI mode. Parameters : mode ( UIMode ) – UI mode to switch to. Raises : ServiceNotFoundError – If Substance 3D Painter has not started its UI service. Return type : None



---

## Structured Notes

### Core Technique
The documented entry points for putting your own PySide6 widgets into Painter's interface — dock widgets, toolbars, menu actions — plus reading, restoring and resetting the layout per UI mode.

### Summary
`substance_painter.ui` is small and almost entirely Qt-shaped: it hands you the real `QMainWindow` (`get_main_window()`), accepts your `QWidget` as a dock (`add_dock_widget`), your `QMenu` (`add_menu`), your `QAction` against one of six standard application menus (`add_action`), and creates toolbars for you (`add_toolbar`). Two enums govern placement: **`UIMode`** (`Edition` 1, `Visualisation` 2 — Iray, `Baking` 4 — note the values are **flags**, and several calls take "a combination of UIMode flags") and **`ApplicationMenu`** (`File`, `Edit`, `Mode`, `Window`, `Viewport`, `Help`). Almost every function raises **`ServiceNotFoundError`** if Painter has not started its UI service, which is the concrete reason a plugin should wait for the `GraphicalUserInterfaceStarted` event before touching any of it. Two details save real debugging time: a widget's **`windowIcon`** becomes the quick-button used to reopen a closed dock, and a **unique `objectName`** is what makes dock and toolbar geometry save and restore correctly — for `add_toolbar` the docs call a unique `object_name` *mandatory*.

### Key Steps
1. Wait for the UI to exist — connect to `substance_painter.event.GraphicalUserInterfaceStarted` before instantiating widgets, or expect `ServiceNotFoundError`.
2. Get the application window with **`get_main_window()`** (returns a real `PySide6.QtWidgets.QMainWindow`) and use it to parent dialogs.
3. Add a panel with **`add_dock_widget(widget, ui_modes=UIMode.Edition)`** — returns the created `QDockWidget`. Set the widget's `windowIcon` so a closed dock can be reopened from its quick button, and give it a unique `objectName` so its position and geometry persist.
4. Add a toolbar with **`add_toolbar(title, object_name, ui_modes=UIMode.Edition)`** — a **unique** `object_name` is mandatory for layout save/restore — or drop a single widget into the shared plugins toolbar with **`add_plugins_toolbar_widget(widget)`**.
5. Add commands with **`add_action(ApplicationMenu.File, action)`** (⚠️ this **clears the action's tooltip**) or install a whole `QMenu` with **`add_menu(menu)`**.
6. Scope UI to modes by combining `UIMode` flags, and read or change the mode at runtime with **`get_current_mode()`** and **`switch_to_mode(mode)`**.
7. Save and restore layouts: **`get_layout(mode)`** returns `bytes`, **`get_layout_mode(layout)`** tells you which mode a saved blob belongs to, **`set_layout(layout)`** restores it and returns the restored mode, **`reset_layout(mode)`** goes back to default. Bad layout data raises `RuntimeError`.
8. Clean up on unload with **`delete_ui_element(element)`** for every widget and action you added — the object is destroyed, and any later call on it raises.

### Nodes / Tools / Settings
- **Enums:** `UIMode` — `Edition` (1), `Visualisation` (2, Iray), `Baking` (4); `ApplicationMenu` — `File`, `Edit`, `Mode`, `Window`, `Viewport`, `Help`. Both expose `.name` (standard `enum.Enum`).
- **Window:** `show_main_window()`, `get_main_window() -> QMainWindow`.
- **Adding UI:** `add_dock_widget(widget, ui_modes) -> QDockWidget`, `add_plugins_toolbar_widget(widget)`, `add_menu(menu)`, `add_toolbar(title, object_name, ui_modes) -> QToolBar`, `add_action(menu, action)`.
- **Removing UI:** `delete_ui_element(element)`.
- **Modes:** `get_current_mode()`, `switch_to_mode(mode)`.
- **Layouts:** `get_layout(mode) -> bytes`, `get_layout_mode(layout) -> UIMode`, `set_layout(layout) -> UIMode`, `reset_layout(mode)`.
- **Exceptions:** `ServiceNotFoundError` (UI service not started) on nearly every call; `RuntimeError` on malformed layout data.

### Difficulty
Intermediate

### Foundry App & Version
Substance 3D Painter 12.1.4, Python API 0.3.5. Widgets are **PySide6** (`PySide6.QtWidgets`, `PySide6.QtGui`).

### Tags
`python-scripting`, `python-api`, `ui-plugin`, `painter-12`, `intermediate`

---

## Related Tutorials
- [Versioning Plugin Example](versioning-plugin-example.md) — `add_dock_widget`, `add_action` and `delete_ui_element` used end to end.
- [Python API: event Module](python-api-event-module.md) — `GraphicalUserInterfaceStarted`, the event to wait for before building UI.
- [substance_painter_plugins Module](substance-painter-plugins-module.md) — the plugin lifecycle that owns these widgets.

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
