This is my i3lock fork of Lixxia's copy.
It has following differences:
- Display current keyboard layout(used source files of xkb-switch( https://github.com/ierton/xkb-switch ). If '-L' option is provided to program arguments current keyboard layout shall be displayed.
- Display caps lock state (if it's active "CAPS" sign shall appear). If '-C'option is provided caps lock will be displayed.
- Display input visualisation: as you type your password appears string with asteriks showing number of characters. If '-V' option is provided your input will be visualised.
- Specify button radius('-R' option, default 90)
- Time font size(a.k.a. PRIMARY_FONT_SIZE in source code), ('-F' option, default 32)
- Circle opacity('-O' option, default 0.4)
- Border and text opacity('-T' option default 1)
## Example Usage
'i3lock -i ~/Pictures/wallpaper.png -c '#000000' -o '#191d0f' -w '#572020' -l '#000000' -e -V -C -L'
## Screenshots
#### Default
![Default state](/screenshots/lockscreen.png?raw=true "")
#### Key Press
![On key press](/screenshots/lockscreenkeypress.png?raw=true "")
#### Escape/Backspace
![On escape or backspace](/screenshots/lockscreenesc.png?raw=true "")
