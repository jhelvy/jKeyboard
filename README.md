# jKeyboard
This repository contains the files for creating my custom keyboard:
- The `./wasd_files` folder contains all the Adobe Illustrator files for making my customized [WASD keyboard](http://www.wasdkeyboards.com/).
- The `./karabiner` folder contains the json files for my [Karabiner-Elements](https://pqrs.org/osx/karabiner/) settings.

# Table of Contents
- [Customized WASD Keyboard](#customized-wasd-keyboard)
- [Karabiner-Elements Settings](#karabiner-elements-settings)
  - [Installation (mac)](#installation-mac)
  - [jhelvy caps_lock keyboard](#jhelvy-caps_lock-keyboard)
    - [Navigation](#navigation)
    - [Selecting Text](#selecting-text)
    - [Common Shortcuts](#common-shortcuts)
    - [Other Shortcuts](#other-shortcuts)
  - [jhelvy function keys](#jhelvy-function-keys)
  - [Other Custom Commands](#other-custom-commands)
  - [WASD-Specific Keys](#wasd-specific-keys)
- [Example json Settings](#example-json-settings)
- [License](#license)

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
|<kbd>caps lock</kbd> + <kbd>command</kbd> + <kbd>I</kbd> / <kbd>K</kbd> | <kbd>command</kbd> + <kbd>↑</kbd> / <kbd>↓</kbd> | Home / End |
|<kbd>caps lock</kbd> + <kbd>command</kbd> + <kbd>J</kbd> / <kbd>L</kbd> | <kbd>command</kbd> + <kbd>←</kbd> / <kbd>→</kbd> | Go to Start / End of Line |
|<kbd>caps lock</kbd> + <kbd>U</kbd> / <kbd>O</kbd> | <kbd>command</kbd> + <kbd>←</kbd> / <kbd>→</kbd> | Go to Start / End of Line |
|<kbd>caps lock</kbd> + <kbd>spacebar</kbd> | <kbd>fn</kbd> | Function key |
|<kbd>caps lock</kbd> + <kbd>spacebar</kbd> + <kbd>I</kbd> / <kbd>K</kbd> | <kbd>⇞</kbd> / <kbd>⇟</kbd> | Page Up / Page Down |
|<kbd>caps lock</kbd> + <kbd>spacebar</kbd> + <kbd>J</kbd> / <kbd>L</kbd> | <kbd>control</kbd> + <kbd>←</kbd> / <kbd>→</kbd> | Go to Start / End of Next Word |

### Selecting Text
|   Key Combination  |    Maps to    |   Description  |
|:-------------------|:--------------|:---------------|
|<kbd>caps lock</kbd> + <kbd>A</kbd> + <kbd>J</kbd> / <kbd>I</kbd> / <kbd>K</kbd> / <kbd>L</kbd> | <kbd>shift</kbd> + <kbd>←</kbd> / <kbd>↑</kbd> / <kbd>↓</kbd> / <kbd>→</kbd> | Select Text |
|<kbd>caps lock</kbd> + <kbd>A</kbd> + <kbd>U</kbd> / <kbd>O</kbd> | <kbd>command</kbd> + <kbd>shift</kbd> + <kbd>←</kbd> / <kbd>→</kbd> | Select until Start / End of Line |
|<kbd>caps lock</kbd> + <kbd>A</kbd> + <kbd>,</kbd> / <kbd>.</kbd> | <kbd>control</kbd> + <kbd>shift</kbd> + <kbd>←</kbd> / <kbd>→</kbd> | Select until Start / End of Next Word |
|<kbd>caps lock</kbd> + <kbd>A</kbd> + <kbd>[</kbd> / <kbd>]</kbd> | <kbd>option</kbd> + <kbd>shift</kbd> + <kbd>↑</kbd> / <kbd>↓</kbd> | Select until Start / End of Paragraph |

### Common Shortcuts
|   Key Combination  |    Maps to    |   Description  |
|:-------------------|:--------------|:---------------|
|<kbd>caps lock</kbd> + <kbd>N</kbd> | <kbd>backspace</kbd> | Backspace / Delete |
|<kbd>caps lock</kbd> + <kbd>H</kbd> | <kbd>del</kbd> | Forward Delete |
|<kbd>caps lock</kbd> + <kbd>S</kbd> | <kbd>command</kbd> + <kbd>X</kbd> | Cut |
|<kbd>caps lock</kbd> + <kbd>D</kbd> | <kbd>command</kbd> + <kbd>C</kbd> | Copy |
|<kbd>caps lock</kbd> + <kbd>F</kbd> | <kbd>command</kbd> + <kbd>V</kbd> | Paste |
|<kbd>caps lock</kbd> + <kbd>R</kbd> | <kbd>command</kbd> + <kbd>Z</kbd> | Undo |
|<kbd>caps lock</kbd> + <kbd>T</kbd> | <kbd>command</kbd> + <kbd>Y</kbd> | Redo |
|<kbd>caps lock</kbd> + <kbd>M</kbd> | <kbd>command</kbd> + <kbd>F</kbd> | Find |
|<kbd>caps lock</kbd> + <kbd>.</kbd> | <kbd>command</kbd> + <kbd>G</kbd> | Find Next |
|<kbd>caps lock</kbd> + <kbd>,</kbd> | <kbd>command</kbd> + <kbd>shift</kbd> + <kbd>G</kbd> | Find Previous |
|<kbd>caps lock</kbd> + <kbd>E</kbd> | <kbd>Esc</kbd> | Escape |

### Other Shortcuts
|     Key Combination     |    Action    |
|:------------------------|:-------------|
|<kbd>caps lock</kbd> + <kbd>C</kbd> | Open Google Chrome |
|<kbd>caps lock</kbd> + <kbd>Z</kbd> | Open the file `'foo.txt'` in my Dropbox Folder |
|<kbd>caps lock</kbd> + <kbd>8</kbd> | Open Terminal |
|<kbd>caps lock</kbd> + <kbd>2</kbd> | <kbd>command</kbd> + <kbd>control</kbd> + <kbd>2</kbd> (my Sublime Text shortcut to split into two windows)|
|<kbd>caps lock</kbd> + <kbd>G</kbd> | Type my usual email send off ("Cheers, John") |
|<kbd>caps lock</kbd> + <kbd>Y</kbd> |<kbd>control</kbd> + <kbd>Y</kbd> (my Sublime Text shortcut to send selected text to a REPL) |
|<kbd>caps lock</kbd> + <kbd>9</kbd> |<kbd>control</kbd> + <kbd>9</kbd> (my Sublime Text shortcut to shift focus to the LEFT panel) |
|<kbd>caps lock</kbd> + <kbd>0</kbd> |<kbd>control</kbd> + <kbd>0</kbd> (my Sublime Text shortcut to shift focus to the RIGHT panel) |

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
|  <kbd>f9</kbd>  | <kbd>command</kbd> + <kbd>shift</kbd> + <kbd>3</kbd> (Screen Shot) |
|  <kbd>f10</kbd> | Mute |
|  <kbd>f11</kbd> | Volume Decrease |
|  <kbd>f12</kbd> | Volume Increase |

## Other Custom Commands
|     Key      |    Action    |
|:-------------|:-------------|
| Tap <kbd>Left shift</kbd>  | <kbd>(</kbd> |
| Tap <kbd>Right shift</kbd> | <kbd>)</kbd> |
| Hold <kbd>Esc</kbd>   | <kbd>command</kbd> + <kbd>W</kbd> (Close Window) |

## WASD-Specific Keys
These only work on my WASD keyboard (not a standard Apple keyboard):

|     Key      |    Action    |
|:-------------|:-------------|
| <kbd>Right control</kbd> | <kbd>option</kbd> + <kbd>A</kbd> (My Alfred Shortcut) |
| <kbd>Menu</kbd> | Open Finder |

# Example json Settings
I learned a lot about how to write json settings to get Karabiner-Elements to do different things. I included a few examples in the `./karabiner/json_examples` folder.
|     File      |    Description    |
|:--------------|:------------------|
| caps_lock arrows.json | Hold the <kbd>caps lock</kbd> key to turn the <kbd>J</kbd> / <kbd>I</kbd> / <kbd>K</kbd> / <kbd>L</kbd> keys into the <kbd>←</kbd> / <kbd>↑</kbd> / <kbd>↓</kbd> / <kbd>→</kbd> keys |
| open application.json | Launch an Application (in this case Google Chrome) by holding <kbd>right option</kbd> + <kbd>C</kbd>

# License
 GPL-3

📣 Shout-out to [@jasonrudolph](https://github.com/jasonrudolph/keyboard),  [@Vonng](https://github.com/Vonng/Capslock), and the [Karabiner Vi Mode Setting](https://pqrs.org/osx/karabiner/complex_modifications/#vi_mode) for inspiration - I learned a lot by copying a lot of their json code!
