Version Management: Major Updates: +1.0, Minor updates: +0.1 

### 8.1
- Fixed a text issue while generating .py file
- Fixed CTkRangeSlider widget for MacOS
- Added manual entry box for size option of circular widgets
- Fixed CTkTooltip not working on SegmentedButtons
- Fixed the icon in the mac executable

## V8
- Project Mode Export with separate files (beta)
- New Widget: CTkRadarChart
- New Widget: CTkPieChart
- Added Page Name Option
- Layers window
- Bg color issue for fixed frame widgets
- New Line can be added using \n in text
- Horizontal scrollable frame improved
- Root bg color fixed
- Released the MacOS version

### 7.2
- Fixed a lock frame issue
- Fixed a major image path issue
  
### 7.1
- Fixed a grid issue
- Fixed a save file option after opening new project

## V7
- Added new grid background for better widget placement (Ctrl+q)
- New Undo feature (experimental), currently recovers deleted widgets and placements
- Fixed duplicate issue when moved to top 
- Now we can fix the parameter window to right side when opened, helpful if you window size is large. Just click the new gear icon in the bottom of param window
- Now we have ability to link a slider and label, where the label text changes to the slider value
Applicable widgets: CTkSlider, CTkRangeSlider, CTkMeter, CTkColorPicker
- Added Ctrl+C and Ctrl+V for widgets
- Added ability to duplicate whole frame and it's subwidgets
- Added feathering (corner softness) in CTkDraw widget (ctkdlib)
- Now the lock parameter can be saved in Json
- Fixed CTkListbox parameter window issue when open through the menu
- Now the slider value and textbox text can be exported
- Added scrollable frame orientation
- And many more minor improvements and bug fixes...
- 
## V6
- New quick preview option (runs locally)
- Unlock option added
- Added navigation to segmented buttons
- Ability to change page of a widget
- Fixed spawn overlap issue with fixed widgets
- Added label in font scale
- Fixed reload image issue of label/button
- Added delay option in tooltip
- New document option in file menu
- Tried to reduce antivirus false detection, see [#20](https://github.com/Akascape/CTkDesigner-Support/discussions/20)
- More bug fixes

## V5
- New widget: ScrollableFrame
- Now you can add widgets in both normal and scrollable frame
- Acrylic theme for windows
- Alpha/transparency in widgets using pyinstyles
- Modified the app detail section where you can add title/icon in the app
- Fixed issues related to images Can't clear image file reference from Application
- Fixed duplicate button with image error
- Fixed adding Image to Draw error
- Updated ctkdlib

## V4
- 3 new widgets
  - gif
  - video player
  - draw canvas
- Ability to add hover tooltips on any widget
- Ability to add popup menu on right click or any side of the widget after clicking (suitable for making a ctkmenubar)
- Ability to manually set the slider value by right-clicking on the option
- Uploaded custom_widgets library to pypi, called ctkdlib: https://pypi.org/project/ctkdlib/
- Ability to add variable names for each widget if required
- Now images can properly be added with CTkDraw widget where we can adjust corners, brightness, blur, etc...
- Fixed one Font and Image dialog bug issue
- Minor bug fixes in the pages feature

## V3
- 3 new widgets
  - calendar
  - chart
  - listbox
- Added Pages for multiple windows
- Navigation in pages through buttons
- Added font and image dialog boxes
- Ability to fix widgets in all pages

### V3.2
- fixed bg color issue when frame is moved above other widgets
- added manual coordinate window
- dpi scale issue fixed (mouse movement)

### V3.1
- fixed unicode text error
  
## V2 
- 7 special widgets added
   - color picker
   - spin box
   - table
   - graph
   - hyperlink
   - circular meter
   - range slider
- Added CTkSegmentedButton
- Auto bg adjustments
- pep8 refactorization in exported code
- moved scale settings to export menu
- Icon settings
  
## V1
- 13 CTk widgets
- DRAG & DROP
- Move and place widgets with mouse
- Adjust all widget parameters
- Precise place method
- 13 CTk widgets 
- Create and preview themes
- Export to .py
- Save/Open created templates again
- All required functionalities and shortcuts added
- WYSIWYG: what you see is what you get
