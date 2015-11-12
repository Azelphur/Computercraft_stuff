Simple plugin to allow caching for monitors so that you can have flicker-free display.

Wrap a peripheral with easymonitor.wrap("side") then call write as normal, write also has extra additional optional parameters

write(text, x, y, color, bgcolor)

when you are ready for the monitor to be redrawn, call monitor.draw()
