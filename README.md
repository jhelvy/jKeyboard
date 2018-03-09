# jKeyboard
This repository contains the files for creating my custom keyboard:
- The `wasd_file` folder contains all the Adobe Illustrator files for making my [WASD keyboard](http://www.wasdkeyboards.com/).
- The `karabiner` folder contains all the files for my [Karabiner-Elements](https://pqrs.org/osx/karabiner/) settings.

# My Customized WASD Keyboard
The keyboard looks like this:
![alt text](https://raw.github.com/jhelvy/jKeyboard/master/wasd_files/keyboard_preview.jpg "Keyboard Layout")

The most significant thing about this design is the blue "hyper" key that is in place of the "Caps_lock" key. I use Karabiner-Elements to modify the keyboard such that when this "hyper" key is held down the functionality of many other keys also change, which is indicated by the small blue icons in the lower-right corners of each key.

# Karabiner-Elements Settings
The Karabiner-Elements settings can be found in the `karabiner` folder. There are two versions:
1. The `jSettings` file contains the settings for my WASD custom keyboard, which I use with a Mac Mini
2. The `jSettings_macbook` file contains the settings for my Macbook. The only difference between the two is that the main `jSettings` has a couple extra shortcuts to toggle the `finder` and `Alfred` windows.

## Navigation
|           Key Combination            |    Action    |
|:-------------------------------------|:-------------|
|`Caps_lock`                           |Trigger Key|
|`Caps_lock` + `J/I/K/L`               |Arrow Keys (Left / Up / Down / Right)|
|`Caps_lock` + `Left_⌘` + `J/I/K/L`   |`⌘` + Arrow Keys|
|`Caps_lock` + `U/O`                   |Go to Start / End of Next Word|
|`Caps_lock` + `Spacebar`              |Fn|
|`Caps_lock` + `Spacebar` + `J/I/K/L`  |Home / Page Up / Page Down / End|
|`Caps_lock` + `Spacebar` + `U/O`      |Go to Start / End of Line|

## Selecting Text
|           Key Combination              |    Action    |
|:---------------------------------------|:-------------|
|`Caps_lock` + `A` + `J/I/K/L`           |Select Text|
|`Caps_lock` + `A` + `U/O`               |Select until Start/End of Line|
|`Caps_lock` + `A` + `Comma/Period`      |Select until Start/End of Next Word|
|`Caps_lock` + `A` + `Open/Close Bracket`|Select until Start/End the Paragraph|

## Common Shortcuts
|     Key Combination     |    Action    |
|:------------------------|:-------------|
|`Caps_lock` + `H`        |Forward Delete|
|`Caps_lock` + `N`        |Delete|
|`Caps_lock` + `S`        |Cut|
|`Caps_lock` + `D`        |Copy|
|`Caps_lock` + `F`        |Paste|
|`Caps_lock` + `R`        |Undo|
|`Caps_lock` + `T`        |Redo|
|`Caps_lock` + `M`        |Find|
|`Caps_lock` + `Comma`    |Find Previous|
|`Caps_lock` + `Period`   |Find Next|
|`Caps_lock` + `E`        |Escape|

## Other Shortcuts
|     Key Combination     |    Action    |
|:------------------------|:-------------|
|`Caps_lock` + `C`        |Open Google Chrome|
|`Caps_lock` + `Z`        |Open the file `'foo.txt'` in my Dropbox Folder|
|`Caps_lock` + `Y`        |`Control` + `Y` (My Sublime Text shortcut to send selected text to a REPL)|
|`Caps_lock` + `9`        |`Control` + `9` (My Sublime Text shortcut to shift focus to the LEFT panel)|
|`Caps_lock` + `0`        |`Control` + `0` (My Sublime Text shortcut to shift focus to the RIGHT panel)|
