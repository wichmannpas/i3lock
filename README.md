This is my fork of [Lixxia's i3lock copy](https://github.com/Lixxia/i3lock).

It has following differences:

 - Display current **keyboard layout**(used source files of [xkb-switch]( https://github.com/ierton/xkb-switch )). Use **"--no-keyboard-layout"** option to turn it off
 - Display **caps lock state** (if it's active the "CAPS" label will appear). Use **"--no-caps-lock-state"** option to turn it off
 - Display **input visualisation**: as you type your password appears string with asteriks showing number of characters. Use **"--no-input-visualisation"** to turn it off
 - Specify **button radius**(**'-R'** option, default 90)
 - Specify time **font size**(a.k.a. PRIMARY_FONT_SIZE in source code), (**'-F'** option, default 32)
 - Specify **circle opacity**(**'-O'** option, default 0.4)
 - Specify **border and text opacity**(**'-T'** option default 1)
 - Specify unlock indicator **position** providing **'-X'** and **'-Y'** arguments with desired x and y offsets from **right bottom corner**(see screenshots below)

## Screenshots
#### Default
	i3lock -i ~/Pictures/wallpaper.png

![Default state](/screenshots/defaultBehaviour.png?raw=true "")
#### Key Press
![On key press](/screenshots/defaultBehaviourKeyPress.png?raw=true "")
#### Verifying
![Verifying](/screenshots/defaultBehaviourVerifying.png?raw=true "")
#### Backspace
![Backspace](/screenshots/defaultBehaviourBackspace.png?raw=true"")

#### -R option allows user to specify radius of the indicator
	'i3lock -i ~/Pictures/wallpaper.png -R 150'

!['-R'](/screenshots/usingROption.png?raw=true "")

#### Specify font size with '-F' option
	'i3lock -i ~/Pictures/wallpaper.png -R 150 -F 50'

!['-R', '-F'](/screenshots/usingRAndFOptions.png?raw=true "")

#### Pass a big radius
	'/i3lock -i ~/Pictures/wallpaper.png -R 800'

![Big radius](/screenshots/bigRadius.png?raw=true "")

#### And combine it with specific font size
	'/i3lock -i ~/Pictures/wallpaper.png -R 800 -F 100'

![Big radius and big font](/screenshots/bigRadiusAndFontSize.png?raw=true "")

#### Or do even something like this(with '-X' and '-Y' options)
	'i3lock -i ~/Pictures/wallpaper.png -R 1300 -F 100 -X 400 -Y 200'

![Offset](/screenshots/bigRadiusAndFontSizeXYOffset.png?raw=true "")

## Installation

	$ git clone https://github.com/cac03/i3lock.git
	$ cd i3lock
	# make install
