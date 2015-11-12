Monitorwidgets is a simple plugin to make it easy for multiple pieces of code to use the same monitor. Useful for monitoring setups.

Plugins are very simple, create a file in the monitorwidgets_plugins folder, in it you should have two functions.

function draw(monitor, settings)
Return a list of line pairs and colours, for example...
{{"Hello world", colors.orange}, {"The weather today is Sunny", colors.green}} would render a two lines, one in orange and one in green.

monitor parameter is the monitor object for the monitor being written to, this is useful if you need to modify aspects of the monitor (eg scale) or if you want to do caching (should be done on a per-monitor basis)
settings parameter is the settings passed through from the config file.

function getTitle
Return the title of your plugin, for title bars.

The config file is fairly simple, and allows you to configure the width, height, x and y of widgets. Note that these positions pertain to the contents of the window, title bars and borders will be drawn outside this area. Eg if you put a window at 1,1 and enable borders, the top and left border will not be drawn as they would be off screen.
