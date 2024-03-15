# CTkDLib

This is a special library for CTkDesigner apps, it contains some custom widgets made for customtkinter. 

This library is shared under MIT license, so you can use it with any application.

### How to install?
```
pip install ctkdlib
```
Pypi Page: https://pypi.org/project/ctkdlib/

## Features
- CTkCalendar
- CTkVideo
- CTkTooltip
- CTkChart
- CTkGraph
- CTkGif
- CTkMeter
- CTkPopupMenu
- CTkRangeSlider
- CTkColorPicker
- CTkDraw
- CTkSpinbox
- CTkHyperLink

# Documentation

### Common Methods for all widgets
- .configure(..args) : change the parameters
- .cget(param) : returns the value of a parameter
- .bind(func, command, add) : bind an event with the widget
- .unbind(func) : unbind the widget event
- .destroy() : destroy the widget completely
- .place_forget() : remove the widget from the page

## CTkCalendar

### Parameters

| Arguments | Description |
|---------|-------------|
| width | change width of widget |
| height | change height of widget |
| fg_color | change foreground color of widget |
| bg_color | change background color of widget |
| text_color | change the color of the text |
| corner_radius | change the corner roundness |
| border_width | change the width of the border |
| border_color | change the border color |
| font | change the font of the text |
| hover | enable/disable the hover effect |
| hover_color | change the color of hover effect |
| select_color | change the selected date color |
| command | add command when a data is selected |
| header_color | change the color of the header |
| header_text_color | change the color of the text in the header |

### Methods
- .current_data() : return the selected_date
- .set([day, month, year]) : switch the calendar to this date
- .select([day, month, year]) :  selects custom date

## CTkColorPicker

### Parameters

| Arguments | Description |
|---------|-------------|
| size | change the size of the color wheel |
| fg_color | change foreground color of widget frame |
| bg_color | change background color of widget |
| corner_radius | change the corner roundness |
| border_width | change the width of the border |
| border_color | change the border color |
| command | add command when a the color is changed |
| initial_color | set the defualt color, hex, (may not work with all colors) |

### Methods
- .get() : returns the selected color

## CTkHyperLink

### Parameters
| Arguments | Description |
|---------|-------------|
| width | change width of widget |
| height | change height of widget |
| fg_color | change foreground color of widget |
| text_color | change the color of the text |
| font | change the font of the text |
| url | add the url link which will be opened after clicking on the widget|
| image | add image to the link label |
| command | add command when a the text is clicked |

## CTkGraph

### Parameters
| Arguments | Description |
|---------|-------------|
| width | change width of widget |
| height | change height of widget |
| values | give the graph values, in list |
| fg_color | change foreground color of widget |
| corner_radius | change the corner roundness |
| border_width | change the width of the border |
| border_color | change the border color |
| graph_color | change the color of the graph content |
| axis_width | change the width of the x-y axis |
| axis_color | change the color of the axis |
| line_color | change the color of the graph lines |

## CTkChart

### Parameters
| Arguments | Description |
|---------|-------------|
| width | change width of widget |
| height | change height of widget |
| values | give the graph values, in list |
| fg_color | change foreground color of widget |
| bg_color | change background color of widget |
| text_color | change the color of the text |
| font | change the font of the text |
| corner_radius | change the corner roundness |
| border_width | change the width of the border |
| border_color | change the border color |
| axis_width | change the width of the x-y axis |
| axis_color | change the color of the axis |
| bar_width | change the width of the stats |
| bar_color | change the color of the stats |
| bar_text_color | change the color of the stat text |

## CTkRangeSlider

### Parameters
| Arguments | Description |
|--------|----------|
|command	| callback function, receives slider value as argument, two separate commands can be given by `command=(cmd1, cmd2)`|
|variables	| tuple: set two tkinter.IntVar or tkinter.DoubleVar objects |
|width	| slider width in px|
|height | slider height in px|
|corner_radius| corner roundness of the slider |
|border_width	| space around the slider rail in px |
|from_	| lower slider value |
|to	| upper slider value |
|number_of_steps |	number of steps in which the sliders can be positioned |
|fg_color	| foreground color, tuple: (light_color, dark_color) or single color |
|progress_color	| tuple: (light_color, dark_color) or single color or "transparent", color of the slider line before the button |
|border_color	| slider border color, tuple: (light_color, dark_color) or single color or "transparent", default is "transparent"|
|button_color |	color of the slider buttons, tuple: (light_color, dark_color) or single color or **((light_color_1, dark_color_1), (light_color_2, light_color_2)) for separate button colors** |
|button_hover_color |	hover color, tuple: (light_color, dark_color) or single color|
|button_width | width of the buttons in px |
|button_length | length of the buttons in px|
|button_corner_radius | corner roundness of the buttons |
|orientation | "horizontal" (standard) or "vertical" |
|state	| "normal" or "disabled" (not clickable) |
|hover | bool, enable/disable hover effect, default is True |

### Methods
- .set([value, value]) : set sliders to specific float value.
- .get() : get current values of slider.

## CTkMeter 

### Parameters
| Arguments | Description |
|---------|-------------|
| size | change the size of the color wheel |
| values | give the graph values, in list |
| fg_color | change foreground color of widget |
| bg_color | change background color of widget |
| border_width | change the width of the border |
| border_color | change the border color |
| scroll | enable/disable the mouse scroll which changes the value |
| progress_color	| tuple: (light_color, dark_color) or single color or "transparent", color of the meter line |
| from_	| lower meter value |
| to	| upper meter value |
| value | set default value of the meter |
| number_of_steps |	number of steps in which the meter can be positioned |
| line_width | change the thickness of the arc of meter |
| command | add command when value is changed |

### Methods
- .set([value, value]) : set custom value to the meter manually
- .get() : get current value of meter

## CTkSpinbox 

### Parameters
| Arguments | Description |
|---------|-------------|
| width | change width of widget |
| height | change height of widget |
| values | give the graph values, in list |
| fg_color | change foreground color of widget |
| bg_color | change background color of widget |
| corner_radius| corner roundness of the spinbox |
| border_width | change the width of the border |
| border_color | change the border color |
| button_color | change the color of the  + - buttons |
| button_hover_color | change the hover color of the  + - buttons |
| button_width | change the width of the + - buttons |
| entry_color | change the entry box color |
| from_	| lower spinbox value |
| to	| upper spinbox value |
| number_of_steps |	number of steps in which the spinbox can be positioned |
| value | set default value of the spinbox |
| text_color | change the color of the text |
| font | change the font of the text |
| command | add command when value is changed |

## CTkGif

### Parameters
| Arguments | Description |
|---------|-------------|
| width | change width of widget |
| height | change height of widget |
| path | the gif path location |
| loop | loop the gif animation infinitely |
| speed | change the speed of the gif animation |
| repeat | loop only for a specific time |

### Methods
- .start() : starts the gif animation
- .stop() : stops the gif animation
- .toggle() : start/stop the gif

## CTkDraw 

### Parameters
| Arguments | Description |
|---------|-------------|
| width | change width of widget |
| height | change height of widget |
| path | the image path location |
| fg_color | change foreground color of canvas |
| corner_radius | change corner roundness of the image |
| draw | bool, enable/disable writing on the canvas image |
| text_color | change the color of the pen |
| pen_size | change the size of the pen |
| brightness | change the brightness level of the image |
| contrast | change the contrast level of the image |
| saturation | change the color saturation of the image |
| sharpness | change the sharpness value of the image |
| blur | add gausian blur in the image |

### Methods
- .clear() : clears the drawings
- .paste(path, width, height, x, y) : paste a new image in top of the canvas
- .save(location) : save the canvas image

### CTkVideo

To use this widget, you have to install [pyav](https://pypi.org/project/av/) and [pyaudio](https://pypi.org/project/PyAudio/)

### Parameters
| Arguments | Description |
|---------|-------------|
| width | change width of widget |
| height | change height of widget |
| fg_color | change foreground color of widget |
| audio | enable/disable the audio while playing |
| keep_aspect | enable/disable aspect ration |

### Methods
- .load(file) : load the video file
- .play() : play the video file
- .pause() : pause the video
- .stop() : stop/end the video
- .mute()/.unmute() : enable/disable the audio
- .seek(second) : seek to a particular section of video
- .video_info() : returns the video information

(This widget is derivative of TkVideoPlayer)

## CTkTooltip

### Parameters
| Arguments | Description |
|---------|-------------|
| master | add the hover to the widget |
| text | specify the hover message |
| delay | show the message after hovering delay, default 1.5s |
| fg_color | change foreground color of widget |
| text_color | change the color of the text |
| font | change the font of the text |
| state | change the state of the widget |

## CTkPopupMenu

### Parameters
| Arguments | Description |
|---------|-------------|
| master | link the popup to the widget |
| width | change width of widget |
| height | change height of widget |
| fg_color | change foreground color of widget |
| bg_color | change background color of widget |
| border_width | change the width of the border |
| border_color | change the border color |
| text_color | change the color of the text |
| corner_radius | change corner roundness of the widget |
| hover | enable/disable the hover effect |
| hover_color | change the color of hover effect |
| font | change the font of the text |
| values | dict, add the menu content and commands, example: {"option1": command, "option2": None} |
| popup_type | spawn type, 0 for right click, 1 for below the widget, 2 for right side, 3 for left side after click |

## Methods:
- .popup() : spawn the popup menu manually
- .hide() : hides the popup menu
- .clear_all() : remove all the menu content
