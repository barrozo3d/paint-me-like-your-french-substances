---
title: Versioning Plugin Example
source: Article
url: file:///C:/Program%20Files/Adobe%20Substance%203D%20Painter/resources/python-doc/plugins/versioning_plugin.html
author: Adobe Substance 3D Painter 12.1.4 bundled docs
ingested: 2026-09-04
app: "[PENDING]"
version: "[PENDING]"
tags: []
extraction_status: pending
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
