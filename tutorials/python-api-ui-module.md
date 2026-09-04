---
title: Python API: ui Module
source: Article
url: file:///C:/Program%20Files/Adobe%20Substance%203D%20Painter/resources/python-doc/substance_painter/ui.html
author: Adobe Substance 3D Painter 12.1.4 bundled docs
ingested: 2026-09-04
app: "[PENDING]"
version: "[PENDING]"
tags: []
extraction_status: pending
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
[PENDING EXTRACTION]

### Summary
[PENDING EXTRACTION]

### Key Steps
[PENDING EXTRACTION]

### Layers / Tools / Settings
[PENDING EXTRACTION]

### Difficulty
[PENDING EXTRACTION]

### App & Version
[PENDING EXTRACTION]

### Tags
[PENDING EXTRACTION]

---

## Related Tutorials
[PENDING EXTRACTION]
