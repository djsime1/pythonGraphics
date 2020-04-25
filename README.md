# Python Graphics 
### (A student fork)

*Reffer to [bbrzuszk/pythonGraphics wiki](https://github.com/bbrzuszk/pythonGraphics/wiki) for most documentation!*  
Also, [check out some of my demo files! (djsime1/scraps)](https://github.com/djsime1/scraps)

## Modifications:
- **Error message improvements**: checkMouse*/getMouse* now error with their proper name instead of just checkMouse or getMouse.

- **getMouseMiddle()**: Pauses for the user to middle-click a mouse button in the window and return where the mouse was middle-clicked as a Point object  
Example: `clickPoint = win.getMouseMiddle()`

- **checkMouseMiddle()**: Similar to getMouseMiddle(), but does not pause for a user middle-click. Returns the last point where the mouse was middle-clicked or None if the window has not been middle-clicked since the previous call to checkMouseMiddle or getMouseMiddle.  
Example: `clickPoint = win.checkMouseMiddle()` *Note: clickPoint may be None!*

- **checkScroll()**: Returns integer depending on user's last scroll action. Positive value if scrolled up, negative if scrolled down, zero if no scroll action since last check. (Tested and confirmed on Windows/Linux)  
Example: `scrollDir = win.checkScroll()` *Note: does not return a point!*
