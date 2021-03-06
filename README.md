# jKeyboard
If you were a professional guitarist, wouldn't you play on a premium guitar?

If you were a chef, wouldn't you invest in a premium chef knife?

Well, as someone who types literally [millions](http://whatpulse.org/jhelvy) of keystrokes a year for my profession, I decided to invest in a premium keyboard by combining [Karabiner-Elements](https://pqrs.org/osx/karabiner/) with a customized [WASD Keyboard](http://www.wasdkeyboards.com/). This repository contains the files for creating my custom keyboard:
- The `karabiner` folder contains the json files for my [Karabiner-Elements](https://pqrs.org/osx/karabiner/) settings.
- The `wasd_files` folder contains the Adobe Illustrator file used to make my customized [WASD keyboard](http://www.wasdkeyboards.com/).

My [Karabiner-Elements](https://pqrs.org/osx/karabiner/) settings enable all sorts of keyboard modifications, including:
- Use <kbd>J</kbd> / <kbd>I</kbd> / <kbd>K</kbd> / <kbd>L</kbd> as arrow keys for [navigating the cursor](#navigation) and [selecting text](#selecting-text).
- Create more convenient and comfortable shortcuts for [common commands](#common-shortcuts), like `cut`, `copy`, `paste`, `delete`, `backspace`, `undo`, `redo`, `find`, and `escape`.
- [Launch applications](#other-shortcuts) like `Google Chrome` or `Terminal` with a single hotkey.
- Open `Google Chrome` to a webpage (e.g. gmail) with a single hotkey
- Type my email send off (`"Cheers, John"`) with a single hotkey.

# Table of Contents
- [Customized WASD Keyboard](#customized-wasd-keyboard)
- [Karabiner-Elements Settings](#karabiner-elements-settings)
  - [Installation (mac)](#installation-mac)
  - [Caps_lock Keyboard](#caps_lock-keyboard)
    - [Navigation](#navigation)
    - [Selecting Text](#selecting-text)
    - [Common Shortcuts](#common-shortcuts)
    - [Other Shortcuts](#other-shortcuts)
  - [Custom Function Keys](#custom-function-keys)
  - [Other Commands](#other-commands)
- [Example json Settings](#example-json-settings)
- [License](#license)

# Customized WASD Keyboard
My [WASD keyboard](http://www.wasdkeyboards.com/) looks like this:
![alt text](https://raw.github.com/jhelvy/jKeyboard/master/wasd_files/keyboard_preview.jpg "Keyboard Layout")

All I did to create this was edit the Adobe Illustrator keyboard file (`./wasd_files/keyboard_layout_104.ai`). In addition to adding a bunch of customized icons (e.g. the function keys), I changed the  <kbd>caps lock</kbd> key to a blue <kbd>hyper</kbd> key that when held down (with the help of [Karabiner-Elements](https://pqrs.org/osx/karabiner/)) essentially creates another keyboard with an entirely different functionality (indicated by the small blue icons in the lower-right corners of each key).

For those curious, the Chinese text on the spacebar is the idiom "晴耕雨读", which literally means "Sunny farm rain read." The meaning is to farm on sunny days and read on rainy days. In other words, work hard, life a simple life, and enjoy each present moment.

# Karabiner-Elements Settings
The [Karabiner-Elements](https://pqrs.org/osx/karabiner/) json settings are found in `./karabiner/jKeyboard.json`. These particular settings include three separate "profiles" that you can select in the Karabiner preference window: 1) jKeyboard-Apple, 2) jKeyboard-WASD, and 3) jKeyboard-CM. The main profile is "jKeyboard-Apple," which is configured for a standard Apple keyboard and includes all the settings described on this page. The other two profiles have additional functionality that is specific to my [WASD keyboard](http://www.wasdkeyboards.com/) and another keyboard by Cooler Master, which I use on different Mac machines.

## Installation (mac)
1. Download [Karabiner-Elements](https://pqrs.org/osx/karabiner/) and Install.
2. Open the `karabiner.json` configuration file. To find it, open Terminal.app and type `open ~/.config`, which will open the hidden .config directory in a new Finder window. There you can navigate to `karabiner/karabiner.json` and open/edit that file.
3. Copy-paste the settings in one of the json files in the `./karabiner/` folder in this repo to overwrite the default karabiner.json file.

## Caps_lock Keyboard
One of the primary things my `jKeyboard` settings does is modify the <kbd>caps lock</kbd> key such that when held down it essentially creates another keyboard with an entirely different functionality. Here is a summary of the current settings:

### Navigation
|   Key Combination  |    Maps to    |   Description  |
|:-------------------|:--------------|:---------------|
| <kbd>caps lock</kbd> | Nothing | Trigger for "hyper" keyboard |
| <kbd>caps lock</kbd> + <kbd>J</kbd> / <kbd>I</kbd> / <kbd>K</kbd> / <kbd>L</kbd> | <kbd>←</kbd> / <kbd>↑</kbd> / <kbd>↓</kbd> / <kbd>→</kbd> | Arrow Keys |
|<kbd>caps lock</kbd> + <kbd>command</kbd> + <kbd>I</kbd> / <kbd>K</kbd> | <kbd>command</kbd> + <kbd>↑</kbd> / <kbd>↓</kbd> | Home / End |
|<kbd>caps lock</kbd> + <kbd>command</kbd> + <kbd>J</kbd> / <kbd>L</kbd> | <kbd>command</kbd> + <kbd>←</kbd> / <kbd>→</kbd> | Go to Start / End of Line |
|<kbd>caps lock</kbd> + <kbd>U</kbd> / <kbd>O</kbd> | <kbd>command</kbd> + <kbd>←</kbd> / <kbd>→</kbd> | Go to Start / End of Line |
|<kbd>caps lock</kbd> + <kbd>spacebar</kbd> | <kbd>control</kbd> | Control key |
|<kbd>caps lock</kbd> + <kbd>spacebar</kbd> + <kbd>I</kbd> / <kbd>K</kbd> | <kbd>⇞</kbd> / <kbd>⇟</kbd> | Page Up / Page Down |
|<kbd>caps lock</kbd> + <kbd>spacebar</kbd> + <kbd>J</kbd> / <kbd>L</kbd> | <kbd>control</kbd> + <kbd>←</kbd> / <kbd>→</kbd> | Go to Start / End of Next Word |

### Selecting Text
|   Key Combination  |    Maps to    |   Description  |
|:-------------------|:--------------|:---------------|
|<kbd>caps lock</kbd> + <kbd>A</kbd> | <kbd>shift</kbd> | Shift key |
|<kbd>caps lock</kbd> + <kbd>A</kbd> + <kbd>J</kbd> / <kbd>I</kbd> / <kbd>K</kbd> / <kbd>L</kbd> | <kbd>shift</kbd> + <kbd>←</kbd> / <kbd>↑</kbd> / <kbd>↓</kbd> / <kbd>→</kbd> | Select Text |
|<kbd>caps lock</kbd> + <kbd>A</kbd> + <kbd>command</kbd> + <kbd>I</kbd> / <kbd>K</kbd> | <kbd>command</kbd> + <kbd>shift</kbd> + <kbd>↑</kbd> / <kbd>↓</kbd> | Select all to top / bottom |
|<kbd>caps lock</kbd> + <kbd>A</kbd> + <kbd>command</kbd> + <kbd>J</kbd> / <kbd>L</kbd> | <kbd>command</kbd> + <kbd>shift</kbd> + <kbd>←</kbd> / <kbd>→</kbd> | Select until Start / End of Line |
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
|<kbd>caps lock</kbd> + <kbd>C</kbd> | Open `Google Chrome` |
|<kbd>caps lock</kbd> + <kbd>Z</kbd> | Open the file `'foo.txt'` in my Dropbox Folder |
|<kbd>caps lock</kbd> + <kbd>Quote (')</kbd> | Open my `Dropbox` folder |
|<kbd>caps lock</kbd> + <kbd>/</kbd> | Open my `Downloads` folder |
|<kbd>caps lock</kbd> + <kbd>P</kbd> | Open my `pCloud Drive` folder |
|<kbd>caps lock</kbd> + <kbd>A</kbd> + <kbd>P</kbd> | Open my `pCloud Sync` folder |
|<kbd>caps lock</kbd> + <kbd>8</kbd> | Open `Terminal` |
|<kbd>caps lock</kbd> + <kbd>2</kbd> | <kbd>command</kbd> + <kbd>control</kbd> + <kbd>2</kbd> (my Sublime Text shortcut to split into two windows)|
|<kbd>caps lock</kbd> + <kbd>G</kbd> | Type my email send off ("`Cheers, John`") |
|<kbd>caps lock</kbd> + <kbd>Y</kbd> |<kbd>control</kbd> + <kbd>Y</kbd> (my Sublime Text shortcut to send selected text to a REPL) |
|<kbd>caps lock</kbd> + <kbd>9</kbd> |<kbd>control</kbd> + <kbd>9</kbd> (my Sublime Text shortcut to shift focus to the LEFT panel) |
|<kbd>caps lock</kbd> + <kbd>0</kbd> |<kbd>control</kbd> + <kbd>0</kbd> (my Sublime Text shortcut to shift focus to the RIGHT panel) |

## Custom Function Keys
I also changed my function keys to do certain things. While <kbd>f1</kbd> to <kbd>f4</kbd> and <kbd>f10</kbd> to <kbd>f12</kbd> are the standard mac settings, the keys <kbd>f5</kbd> to <kbd>f8</kbd> open specific web pages, and <kbd>f9</kbd> takes a screen shot:

|     Key      |    Action    |
|:-------------|:-------------|
|  <kbd>f1</kbd>  | Brightness Decrease |
|  <kbd>f2</kbd>  | Brightness Increase |
|  <kbd>f3</kbd>  | Mission Control |
|  <kbd>f4</kbd>  | Dashboard |
|  <kbd>f5</kbd>  | Open `Gmail` in Google Chrome |
|  <kbd>f6</kbd>  | Open `Google Calendar` in Google Chrome |
|  <kbd>f7</kbd>  | Open `Facebook` in Google Chrome |
|  <kbd>f8</kbd>  | Open `Intellicast Weather` in Google Chrome |
|  <kbd>f9</kbd>  | <kbd>command</kbd> + <kbd>shift</kbd> + <kbd>3</kbd> (Save screen shot to Desktop) |
|  <kbd>f10</kbd> | Mute |
|  <kbd>f11</kbd> | Volume Decrease |
|  <kbd>f12</kbd> | Volume Increase |

## Other Commands
These are a few other tricks that I find particularly useful:

|     Key      |    Action    |
|:-------------|:-------------|
| Tap <kbd>Left shift</kbd>  | <kbd>(</kbd> |
| Tap <kbd>Right shift</kbd> | <kbd>)</kbd> |
| Hold <kbd>Esc</kbd>   | <kbd>command</kbd> + <kbd>W</kbd> (Close Window) |

# Example json Settings
I learned a lot about how to write json settings to get Karabiner-Elements to do different things. I included the following examples in the `./karabiner/json_examples` folder.

|     File      |    Description    |
|:--------------|:------------------|
| caps_lock_arrows.json | Hold the <kbd>caps lock</kbd> key to turn the <kbd>J</kbd> / <kbd>I</kbd> / <kbd>K</kbd> / <kbd>L</kbd> keys into the <kbd>←</kbd> / <kbd>↑</kbd> / <kbd>↓</kbd> / <kbd>→</kbd> keys |
| launch_application.json | Launch an Application (in this case Google Chrome) by typing <kbd>right option</kbd> + <kbd>C</kbd> |
| open_browser_to_page.json | Open Google Chrome to www.google.com by typing <kbd>right option</kbd> + <kbd>C</kbd> |
| tap_shift_keys_for_parentheses.json | Tap <kbd>left_shift</kbd> / <kbd>right_shift</kbd> to get <kbd>(</kbd> / <kbd>)</kbd> |

# License
 GPL-3

📣 Shout-out to [@jasonrudolph](https://github.com/jasonrudolph/keyboard),  [@Vonng](https://github.com/Vonng/Capslock), and the [Karabiner Vi Mode Setting](https://pqrs.org/osx/karabiner/complex_modifications/#vi_mode) for inspiration - I learned a lot by copying a lot of their json code!
