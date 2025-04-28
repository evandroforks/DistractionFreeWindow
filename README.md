# [DistractionFreeWindow](https://github.com/aziz/DistractionFreeWindow) for [Sublime Text](https://www.sublimetext.com)

[![License](https://img.shields.io/github/license/aziz/DistractionFreeWindow.svg?style=flat-square)](https://github.com/aziz/DistractionFreeWindow/blob/master/LICENSE)
[![Downloads via Package Control](https://img.shields.io/packagecontrol/dt/DistractionFreeWindow.svg?style=flat-square)](https://packagecontrol.io/packages/DistractionFreeWindow)
[![Latest release](https://img.shields.io/github/release/aziz/DistractionFreeWindow.svg?style=flat-square)](https://github.com/aziz/DistractionFreeWindow/releases/latest)

<br>

<p align="center">
  <img width="750" src="https://raw.githubusercontent.com/aziz/DistractionFreeWindow/master/docs/screencast.gif" alt="Screencast">
</p>

<br>

> Screencast shows [gruvbox](https://github.com/Briles/gruvbox) Theme & Color Scheme, [Operator Mono](http://www.typography.com/fonts/operator/overview) Medium as font.

---

## Description

[Sublime Text](https://www.sublimetext.com)'s [`distraction free mode`](https://www.sublimetext.com/docs/3/distraction_free.html) but not full-screen!
A windowed UI is more manageable and accessible, yet it can be simple and sublime!

DistractionFreeWindow was inspired by [this forum post](https://forum.sublimetext.com/t/non-fullscreen-distraction-free-mode/12343).


## Installation

### By Package Control

1. Download & Install **`Sublime Text 3`** (https://www.sublimetext.com/3)
1. Go to the menu **`Tools -> Install Package Control`**, then,
    wait few seconds until the installation finishes up
1. Now,
    Go to the menu **`Preferences -> Package Control`**
1. Type **`Add Channel`** on the opened quick panel and press <kbd>Enter</kbd>
1. Then,
    input the following address and press <kbd>Enter</kbd>
    ```
    https://raw.githubusercontent.com/evandrocoan/StudioChannel/master/channel.json
    ```
1. Go to the menu **`Tools -> Command Palette...
    (Ctrl+Shift+P)`**
1. Type **`Preferences:
    Package Control Settings – User`** on the opened quick panel and press <kbd>Enter</kbd>
1. Then,
    find the following setting on your **`Package Control.sublime-settings`** file:
    ```js
    "channels":
    [
        "https://packagecontrol.io/channel_v3.json",
        "https://raw.githubusercontent.com/evandrocoan/StudioChannel/master/channel.json",
    ],
    ```
1. And,
    change it to the following, i.e.,
    put the **`https://raw.githubusercontent...`** line as first:
    ```js
    "channels":
    [
        "https://raw.githubusercontent.com/evandrocoan/StudioChannel/master/channel.json",
        "https://packagecontrol.io/channel_v3.json",
    ],
    ```
    * The **`https://raw.githubusercontent...`** line must to be added before the **`https://packagecontrol.io...`** one, otherwise,
      you will not install this forked version of the package,
      but the original available on the Package Control default channel **`https://packagecontrol.io...`**
1. Now,
    go to the menu **`Preferences -> Package Control`**
1. Type **`Install Package`** on the opened quick panel and press <kbd>Enter</kbd>
1. Then,
    search for **`DistractionFreeWindow`** and press <kbd>Enter</kbd>

See also:

1. [ITE - Integrated Toolset Environment](https://github.com/evandrocoan/ITE)
1. [Package control docs](https://packagecontrol.io/docs/usage) for details.


## Usage

Use the keybinding `Super+F11` to toggle DistractionFreeWindow mode.

### Changing Layout

Users of the [`MaxPane`](https://packagecontrol.io/packages/MaxPane) plug-in will appreciate that [`DistractionFreeWindow`](https://packagecontrol.io/packages/DistractionFreeWindow) directly integrates with it and simplifies the layout when you go into **DistractionFreeWindow mode** and restores the layout after comming back out of it.

## Customization

### Settings

DistractionFreeWindow inherits `distraction free mode` settings from the core application.
You can set these via `Preferences > Settings - Distraction Free`, compare the official docs:

<https://www.sublimetext.com/docs/3/distraction_free.html>

The following toggle actions can be customized:

```json
// Packages/User/Preferences.sublime-settings

{
    "distraction_free_window.toggle_menu": true,
    "distraction_free_window.toggle_minimap": true,
    "distraction_free_window.toggle_status_bar": true,
    "distraction_free_window.toggle_tabs": true
}
```

### Key Bindings

You can adjust the default key binding <kbd>Super</kbd><kbd>F11</kbd> via `Preferences > Package Settings > DistractionFreeWindow > Key Bindings` from the main menu.

## License

See the [`LICENSE`](LICENSE) for details.
