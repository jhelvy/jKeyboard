# jKeyboard
This repository contains the files for creating my custom keyboard:
- The `wasd_file` folder contains all the Adobe Illustrator files for making my [WASD keyboard](http://www.wasdkeyboards.com/).
- The `karabiner` folder contains all the files for my [Karabiner-Elements](https://pqrs.org/osx/karabiner/) settings.

# My Customized WASD Keyboard
The keyboard looks like this:
![alt text](https://raw.github.com/jhelvy/jKeyboard/master/wasd_files/keyboard_preview.jpg "Keyboard Layout")

The most significant thing about this design is the blue "hyper" key that is in place of the <kbd>caps lock</kbd> key. I use Karabiner-Elements to modify the keyboard such that when this "hyper" key is held down the functionality of many other keys also change, which is indicated by the small blue icons in the lower-right corners of each key.

# Karabiner-Elements Settings
The Karabiner-Elements settings can be found in the `karabiner` folder. There are two versions:
1. The `jSettings` file contains the settings for my WASD custom keyboard, which I use with a Mac Mini
2. The `jSettings_macbook` file contains the settings for my Macbook. The only difference between the two is that the main `jSettings` has a couple extra shortcuts to toggle the `finder` and `Alfred` windows.

## Navigation
|           Key Combination            |    Action    |
|:-------------------------------------|:-------------|
| <kbd>caps lock</kbd> |Trigger Key|
| <kbd>caps lock</kbd> + <kbd>J</kbd> / <kbd>I</kbd> / <kbd>K</kbd> / <kbd>L</kbd> | <kbd>←</kbd> / <kbd>↑</kbd> / <kbd>↓</kbd> / <kbd>→</kbd> |

|<kbd>caps lock</kbd> + <kbd>left ⌘</kbd> + <kbd>J</kbd> / <kbd>I</kbd> / <kbd>K</kbd> / <kbd>L</kbd> | <kbd>left ⌘</kbd> + <kbd>←</kbd> / <kbd>↑</kbd> / <kbd>↓</kbd> / <kbd>→</kbd>|

|<kbd>caps lock</kbd> + <kbd>U</kbd> / <kbd>O</kbd> | <kbd>left ⌘</kbd> + <kbd>←</kbd> / <kbd>→</kbd> (Go to Start / End of Line)|

|<kbd>caps lock</kbd> + <kbd>spacebar</kbd> | <kbd>fn</kbd> |

|<kbd>caps lock</kbd> + <kbd>spacebar</kbd> + <kbd>I</kbd> / <kbd>K</kbd> | <kbd>⇞</kbd> / <kbd>⇟</kbd> (Page Up / Page Down)|

|<kbd>caps lock</kbd> + <kbd>spacebar</kbd> + <kbd>J</kbd> / <kbd>L</kbd> | <kbd>left ⌃</kbd> + <kbd>←</kbd> / <kbd>→</kbd>(Go to Start / End of Next Word)|

## Selecting Text
|           Key Combination              |    Action    |
|:---------------------------------------|:-------------|
|<kbd>caps lock</kbd> + <kbd>A</kbd> + <kbd>J</kbd> / <kbd>I</kbd> / <kbd>K</kbd> / <kbd>L</kbd> | <kbd>shift</kbd> + <kbd>←</kbd> / <kbd>↑</kbd> / <kbd>↓</kbd> / <kbd>→</kbd> (Select Text)|
|<kbd>caps lock</kbd> + <kbd>A</kbd> + <kbd>U</kbd> / <kbd>O</kbd> | <kbd>shift</kbd> + <kbd>left ⌘</kbd> + <kbd>←</kbd> / <kbd>→</kbd> (Select until Start/End of Line) |
|<kbd>caps lock</kbd> + <kbd>A</kbd> + <kbd>,</kbd> / <kbd>.</kbd> | Select until Start/End of Next Word |
|<kbd>caps lock</kbd> + <kbd>A</kbd> + <kbd>[</kbd> / <kbd>]</kbd> | Select until Start/End the Paragraph |

## Common Shortcuts
|     Key Combination     |    Action    |
|:------------------------|:-------------|
|<kbd>caps lock</kbd> + `H`        |Forward Delete|
|<kbd>caps lock</kbd> + `N`        |Delete|
|<kbd>caps lock</kbd> + `S`        |Cut|
|<kbd>caps lock</kbd> + `D`        |Copy|
|<kbd>caps lock</kbd> + `F`        |Paste|
|<kbd>caps lock</kbd> + `R`        |Undo|
|<kbd>caps lock</kbd> + `T`        |Redo|
|<kbd>caps lock</kbd> + `M`        |Find|
|<kbd>caps lock</kbd> + `Comma`    |Find Previous|
|<kbd>caps lock</kbd> + `Period`   |Find Next|
|<kbd>caps lock</kbd> + `E`        |Escape|

## Other Shortcuts
|     Key Combination     |    Action    |
|:------------------------|:-------------|
|<kbd>caps lock</kbd> + `C`        |Open Google Chrome|
|<kbd>caps lock</kbd> + `Z`        |Open the file `'foo.txt'` in my Dropbox Folder|
|<kbd>caps lock</kbd> + `8`        |Open Terminal|
|<kbd>caps lock</kbd> + `2`        |`Left_Command` + `Left_Option` + `2` (Split Sublime Text into Two Windows)|
|<kbd>caps lock</kbd> + `G`        |Type my usual email send off ("Cheers, John")|
|<kbd>caps lock</kbd> + `Y`        |`Control` + `Y` (My Sublime Text shortcut to send selected text to a REPL)|
|<kbd>caps lock</kbd> + `9`        |`Control` + `9` (My Sublime Text shortcut to shift focus to the LEFT panel)|
|<kbd>caps lock</kbd> + `0`        |`Control` + `0` (My Sublime Text shortcut to shift focus to the RIGHT panel)|

## Function Keys
|     Key      |    Action    |
|:-------------|:-------------|
|  f1          |Brightness Decrease|
|  f2          |Brightness Increase|
|  f3          |Mission Control|
|  f4          |Dashboard|
|  f5          |Open Gmail in Google Chrome|
|  f6          |Open Google Calendar in Google Chrome|
|  f7          |Open Facebook in Google Chrome|
|  f8          |Open Intellicast Weather in Google Chrome|
|  f9          |Screen Shot|
|  f10         |Mute|
|  f11         |Volume Decrease|
|  f12         |Volume Increase|
