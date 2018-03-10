
# jKeyboard
This repository contains the files for creating my custom keyboard:
- The `./wasd_files` folder contains all the Adobe Illustrator files for making my customized [WASD keyboard](http://www.wasdkeyboards.com/).
- The `./karabiner` folder contains the json files for my [Karabiner-Elements](https://pqrs.org/osx/karabiner/) settings.

# Table of Contents


# Customized WASD Keyboard
My [WASD keyboard](http://www.wasdkeyboards.com/) looks like this:
![alt text](https://raw.github.com/jhelvy/jKeyboard/master/wasd_files/keyboard_preview.jpg "Keyboard Layout")

In addition to adding a bunch of customized icons (e.g. the function keys), I changed the  <kbd>caps lock</kbd> key to a blue <kbd>hyper</kbd> key that when held down (with the help of [Karabiner-Elements](https://pqrs.org/osx/karabiner/)) essentially creates another keyboard with an entirely different functionality (indicated by the small blue icons in the lower-right corners of each key).

# Karabiner-Elements Settings
The [Karabiner-Elements](https://pqrs.org/osx/karabiner/) json settings files can be found in the `./karabiner` folder. There are two versions:

1. The `jKeyboard_wasd.json` file contains the settings for my WASD custom keyboard, which I use with a Mac Mini
2. The `jKeyboard_mac.json` file contains the settings for my Macbook.

The only difference between the two is that the main `jKeyboard_wasd.json` has a couple [extra custom commands](#wasd-specific-keys) that are specific to my WASD keyboard. Otherwise, I use the `jKeyboard_mac.json` settings for my laptop or any standard Apple keyboard.

## Installation (mac)
1. Download [Karabiner-Elements](https://pqrs.org/osx/karabiner/) and Install.
2. Open the `karabiner.json` configuration file by typing the following into Terminal (obviously, replace [USER NAME] with your user name):
```
open ~/.config
/Users/[USER NAME]/.config/karabiner/karabiner.json
```

3. Copy-paste the settings in one of the json files in the `./karabiner/` folder in this repo to overwrite the default karabiner.json file.

## jhelvy caps_lock keyboard

### Navigation
|   Key Combination  |    Maps to    |   Description  |
|:-------------------|:--------------|:---------------|
| <kbd>caps lock</kbd> + <kbd>J</kbd> / <kbd>I</kbd> / <kbd>K</kbd> / <kbd>L</kbd> | <kbd>←</kbd> / <kbd>↑</kbd> / <kbd>↓</kbd> / <kbd>→</kbd> | Arrow Keys |
|<kbd>caps lock</kbd> + <kbd>⌘</kbd> + <kbd>I</kbd> / <kbd>K</kbd> | <kbd>⌘</kbd> + <kbd>↑</kbd> / <kbd>↓</kbd> | Home / End |
|<kbd>caps lock</kbd> + <kbd>⌘</kbd> + <kbd>J</kbd> / <kbd>L</kbd> | <kbd>⌘</kbd> + <kbd>←</kbd> / <kbd>→</kbd> | Go to Start / End of Line |
|<kbd>caps lock</kbd> + <kbd>U</kbd> / <kbd>O</kbd> | <kbd>⌘</kbd> + <kbd>←</kbd> / <kbd>→</kbd> | Go to Start / End of Line |
|<kbd>caps lock</kbd> + <kbd>spacebar</kbd> | <kbd>fn</kbd> | Function key |
|<kbd>caps lock</kbd> + <kbd>spacebar</kbd> + <kbd>I</kbd> / <kbd>K</kbd> | <kbd>⇞</kbd> / <kbd>⇟</kbd> | Page Up / Page Down |
|<kbd>caps lock</kbd> + <kbd>spacebar</kbd> + <kbd>J</kbd> / <kbd>L</kbd> | <kbd>⌃</kbd> + <kbd>←</kbd> / <kbd>→</kbd> | Go to Start / End of Next Word |

### Selecting Text
|   Key Combination  |    Maps to    |   Description  |
|:-------------------|:--------------|:---------------|
|<kbd>caps lock</kbd> + <kbd>A</kbd> + <kbd>J</kbd> / <kbd>I</kbd> / <kbd>K</kbd> / <kbd>L</kbd> | <kbd>⇧</kbd> + <kbd>←</kbd> / <kbd>↑</kbd> / <kbd>↓</kbd> / <kbd>→</kbd> | Select Text |
|<kbd>caps lock</kbd> + <kbd>A</kbd> + <kbd>U</kbd> / <kbd>O</kbd> | <kbd>⌘</kbd> + <kbd>⇧</kbd> + <kbd>←</kbd> / <kbd>→</kbd> | Select until Start / End of Line |
|<kbd>caps lock</kbd> + <kbd>A</kbd> + <kbd>,</kbd> / <kbd>.</kbd> | <kbd>⌃</kbd> + <kbd>⇧</kbd> + <kbd>←</kbd> / <kbd>→</kbd> | Select until Start / End of Next Word |
|<kbd>caps lock</kbd> + <kbd>A</kbd> + <kbd>[</kbd> / <kbd>]</kbd> | <kbd>⌥</kbd> + <kbd>⇧</kbd> + <kbd>↑</kbd> / <kbd>↓</kbd> | Select until Start / End of Paragraph |

### Common Shortcuts
|   Key Combination  |    Maps to    |   Description  |
|:-------------------|:--------------|:---------------|
|<kbd>caps lock</kbd> + <kbd>N</kbd> | <kbd>⌫</kbd> | Backspace / Delete |
|<kbd>caps lock</kbd> + <kbd>H</kbd> | <kbd>⌦</kbd> | Forward Delete |
|<kbd>caps lock</kbd> + <kbd>S</kbd> | <kbd>⌘</kbd> + <kbd>X</kbd> | Cut |
|<kbd>caps lock</kbd> + <kbd>D</kbd> | <kbd>⌘</kbd> + <kbd>C</kbd> | Copy |
|<kbd>caps lock</kbd> + <kbd>F</kbd> | <kbd>⌘</kbd> + <kbd>V</kbd> | Paste |
|<kbd>caps lock</kbd> + <kbd>R</kbd> | <kbd>⌘</kbd> + <kbd>Z</kbd> | Undo |
|<kbd>caps lock</kbd> + <kbd>T</kbd> | <kbd>⌘</kbd> + <kbd>Y</kbd> | Redo |
|<kbd>caps lock</kbd> + <kbd>M</kbd> | <kbd>⌘</kbd> + <kbd>F</kbd> | Find |
|<kbd>caps lock</kbd> + <kbd>.</kbd> | <kbd>⌘</kbd> + <kbd>G</kbd> | Find Next |
|<kbd>caps lock</kbd> + <kbd>,</kbd> | <kbd>⌘</kbd> + <kbd>⇧</kbd> + <kbd>G</kbd> | Find Previous |
|<kbd>caps lock</kbd> + <kbd>E</kbd> | <kbd>⎋</kbd> | Escape |

### Other Shortcuts
|     Key Combination     |    Action    |
|:------------------------|:-------------|
|<kbd>caps lock</kbd> + <kbd>C</kbd> | Open Google Chrome |
|<kbd>caps lock</kbd> + <kbd>Z</kbd> | Open the file `'foo.txt'` in my Dropbox Folder |
|<kbd>caps lock</kbd> + <kbd>8</kbd> | Open Terminal |
|<kbd>caps lock</kbd> + <kbd>2</kbd> | <kbd>⌘</kbd> + <kbd>⌃</kbd> + <kbd>2</kbd> (my Sublime Text shortcut to split into two windows)|
|<kbd>caps lock</kbd> + <kbd>G</kbd> | Type my usual email send off ("Cheers, John") |
|<kbd>caps lock</kbd> + <kbd>Y</kbd> |<kbd>⌃</kbd> + <kbd>Y</kbd> (my Sublime Text shortcut to send selected text to a REPL) |
|<kbd>caps lock</kbd> + <kbd>9</kbd> |<kbd>⌃</kbd> + <kbd>9</kbd> (my Sublime Text shortcut to shift focus to the LEFT panel) |
|<kbd>caps lock</kbd> + <kbd>0</kbd> |<kbd>⌃</kbd> + <kbd>0</kbd> (my Sublime Text shortcut to shift focus to the RIGHT panel) |

## jhelvy function keys
|     Key      |    Action    |
|:-------------|:-------------|
|  <kbd>f1</kbd>  | Brightness Decrease |
|  <kbd>f2</kbd>  | Brightness Increase |
|  <kbd>f3</kbd>  | Mission Control |
|  <kbd>f4</kbd>  | Dashboard |
|  <kbd>f5</kbd>  | Open Gmail in Google Chrome |
|  <kbd>f6</kbd>  | Open Google Calendar in Google Chrome |
|  <kbd>f7</kbd>  | Open Facebook in Google Chrome |
|  <kbd>f8</kbd>  | Open Intellicast Weather in Google Chrome |
|  <kbd>f9</kbd>  | <kbd>⌘</kbd> + <kbd>⇧</kbd> + <kbd>3</kbd> (Screen Shot) |
|  <kbd>f10</kbd> | Mute |
|  <kbd>f11</kbd> | Volume Decrease |
|  <kbd>f12</kbd> | Volume Increase |

## Other Custom Commands
|     Key      |    Action    |
|:-------------|:-------------|
| Tap <kbd>Left ⇧</kbd>  | <kbd>(</kbd> |
| Tap <kbd>Right ⇧</kbd> | <kbd>)</kbd> |
| Hold `Esc  ⎋`   | <kbd>⌘</kbd> + <kbd>W</kbd> (Close Window) |

## WASD-Specific Keys
These only work on my WASD keyboard (not a standard Apple keyboard):

# Symbol Reference

| Symbol  | Key    |
|:--------|:-------|
| ⌃      | Control |
| ⌥      | Option  |
| ⇧      | Shift   |
| ⌘      | Command |
| ⎋      | Escape |

# Inspiration
📣 Shout-out to [@jasonrudolph](https://github.com/jasonrudolph/keyboard),  [@Vonng](https://github.com/Vonng/Capslock), and the [Karabiner Vi Mode Setting](https://pqrs.org/osx/karabiner/complex_modifications/#vi_mode) for inspiration - I learned a lot by copying a lot of their json code!

# License
 GPL-3
