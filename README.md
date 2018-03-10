
# jKeyboard
This repository contains the files for creating my custom keyboard:
- The `./wasd_files` folder contains all the Adobe Illustrator files for making my customized [WASD keyboard](http://www.wasdkeyboards.com/).
- The `./karabiner` folder contains the json files for my [Karabiner-Elements](https://pqrs.org/osx/karabiner/) settings.

# Table of Contents


# Customized WASD Keyboard
My [WASD keyboard](http://www.wasdkeyboards.com/) looks like this:
![alt text](https://raw.github.com/jhelvy/jKeyboard/master/wasd_files/keyboard_preview.jpg "Keyboard Layout")

In addition to adding a bunch of customized icons (e.g. the function keys), I changed the  `caps lock` key to a blue `hyper` key that when held down (with the help of [Karabiner-Elements](https://pqrs.org/osx/karabiner/)) essentially creates another keyboard with an entirely different functionality (indicated by the small blue icons in the lower-right corners of each key).

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
| `caps lock` + `J` / `I` / `K` / `L` | `←` / `↑` / `↓` / `→` | Arrow Keys |
|`caps lock` + `⌘` + `I` / `K` | `⌘` + `↑` / `↓` | Home / End |
|`caps lock` + `⌘` + `J` / `L` | `⌘` + `←` / `→` | Go to Start / End of Line |
|`caps lock` + `U` / `O` | `⌘` + `←` / `→` | Go to Start / End of Line |
|`caps lock` + `spacebar` | `fn` | Function key |
|`caps lock` + `spacebar` + `I` / `K` | `⇞` / `⇟` | Page Up / Page Down |
|`caps lock` + `spacebar` + `J` / `L` | `⌃` + `←` / `→` | Go to Start / End of Next Word |

### Selecting Text
|   Key Combination  |    Maps to    |   Description  |
|:-------------------|:--------------|:---------------|
|`caps lock` + `A` + `J` / `I` / `K` / `L` | `⇧` + `←` / `↑` / `↓` / `→` | Select Text |
|`caps lock` + `A` + `U` / `O` | `⌘` + `⇧` + `←` / `→` | Select until Start / End of Line |
|`caps lock` + `A` + `,` / `.` | `⌃` + `⇧` + `←` / `→` | Select until Start / End of Next Word |
|`caps lock` + `A` + `[` / `]` | `⌥` + `⇧` + `↑` / `↓` | Select until Start / End of Paragraph |

### Common Shortcuts
|   Key Combination  |    Maps to    |   Description  |
|:-------------------|:--------------|:---------------|
|`caps lock` + `N` | `⌫` | Backspace / Delete |
|`caps lock` + `H` | `⌦` | Forward Delete |
|`caps lock` + `S` | `⌘` + `X` | Cut |
|`caps lock` + `D` | `⌘` + `C` | Copy |
|`caps lock` + `F` | `⌘` + `V` | Paste |
|`caps lock` + `R` | `⌘` + `Z` | Undo |
|`caps lock` + `T` | `⌘` + `Y` | Redo |
|`caps lock` + `M` | `⌘` + `F` | Find |
|`caps lock` + `.` | `⌘` + `G` | Find Next |
|`caps lock` + `,` | `⌘` + `⇧` + `G` | Find Previous |
|`caps lock` + `E` | `⎋` | Escape |

### Other Shortcuts
|     Key Combination     |    Action    |
|:------------------------|:-------------|
|`caps lock` + `C` | Open Google Chrome |
|`caps lock` + `Z` | Open the file `'foo.txt'` in my Dropbox Folder |
|`caps lock` + `8` | Open Terminal |
|`caps lock` + `2` | `⌘` + `⌃` + `2` (my Sublime Text shortcut to split into two windows)|
|`caps lock` + `G` | Type my usual email send off ("Cheers, John") |
|`caps lock` + `Y` |`⌃` + `Y` (my Sublime Text shortcut to send selected text to a REPL) |
|`caps lock` + `9` |`⌃` + `9` (my Sublime Text shortcut to shift focus to the LEFT panel) |
|`caps lock` + `0` |`⌃` + `0` (my Sublime Text shortcut to shift focus to the RIGHT panel) |

## jhelvy function keys
|     Key      |    Action    |
|:-------------|:-------------|
|  `f1`  | Brightness Decrease |
|  `f2`  | Brightness Increase |
|  `f3`  | Mission Control |
|  `f4`  | Dashboard |
|  `f5`  | Open Gmail in Google Chrome |
|  `f6`  | Open Google Calendar in Google Chrome |
|  `f7`  | Open Facebook in Google Chrome |
|  `f8`  | Open Intellicast Weather in Google Chrome |
|  `f9`  | `⌘` + `⇧` + `3` (Screen Shot) |
|  `f10` | Mute |
|  `f11` | Volume Decrease |
|  `f12` | Volume Increase |

## Other Custom Commands
|     Key      |    Action    |
|:-------------|:-------------|
| Tap `Left ⇧`  | `(` |
| Tap `Right ⇧` | `)` |
| Hold `Esc  ⎋`   | `⌘` + `W` (Close Window) |

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
