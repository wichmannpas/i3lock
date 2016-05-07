This is my i3lock fork of Lixxia's copy.
It has following differences:
- Display current keyboard layout(used source files of xkb-switch( https://github.com/ierton/xkb-switch ). Use "--no-keyboard-layout" option to turn this off
- Display caps lock state (if it's active the "CAPS" label will appear). Use "--no-caps-lock-state" option to turn this off
- Display input visualisation: as you type your password appears string with asteriks showing number of characters. Use "--no-input-visualisation" to turn this off
- Specify button radius('-R' option, default 90)
- Specify time font size(a.k.a. PRIMARY_FONT_SIZE in source code), ('-F' option, default 32)
- Specify circle opacity('-O' option, default 0.4)
- Specify border and text opacity('-T' option default 1)
- Specify unlock indicator position providing '-X' and '-Y' arguments with desired x and y offsets from right bottom corner(see screenshots below)
## Example Usage
'i3lock -i ~/Pictures/wallpaper.png -c '#000000' -o '#191d0f' -w '#572020' -l '#000000' -e -V -C -L'
## Screenshots
#### Default
i3lock -i /home/caco3/Pictures/wallpaper.png
![Default state](/screenshots/defaultBehaviour.png?raw=true "")
#### Key Press
![On key press](/screenshots/defaultBehaviourKeyPress.png?raw=true "")
#### Verifying
![Veryfing](/screenshots/defaultBehaviourVerifying.png?raw=true "")
##### Using '-R' and '-F' options
Using -R and -F options allow you to do something like this
i3lock -i /home/caco3/Pictures/wallpaper.png -c '#000000' -o '#191d0f' -w '#572020' -l '#FFFFFF' -e -O .1 -R 1300 -F 100
![With '-R' and '-F'](/screenshots/defaultBehaviourWithBigRadiusAndBigFont.png?raw=true "")

##### Using '-X' and '-Y' options
Or even something like this(with '-X' and '-Y' options)
i3lock -i /home/caco3/Pictures/wallpaper.png -c '#000000' -o '#191d0f' -w '#572020' -l '#FFFFFF' -e -O .1 -R 1300 -F 100 -X 400 -Y 200
![With '-X' and '-Y'](/screenshots/defaultBehaviourWithBigRadiusAndBigFontOffsetted.png?raw=true "")
