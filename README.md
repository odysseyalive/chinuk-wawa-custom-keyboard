# Chinuk Wawa - XKB integration (Linux)

Chinuk Wawa is a trade language once in use by several Native American tribes in the Pacific Northwest. It is taught in an immersive classroom setting by the [Confederated Tribes of Grand Ronde](https://www.grandronde.org/services/education/shawash-ili%CA%94i-skul/).

This installs a Chinuk Wawa custom keyboard onto most Linux distributions without the need for installing additional software.

## Installation

1. Open a terminal and run the following command. You will need the root password to install the file.
```
sudo curl -o /usr/share/X11/xkb/symbols/custom "https://raw.githubusercontent.com/bridgesense/chinuk-wawa-custom-keyboard/refs/heads/main/custom"
```
2. Activate the layout on your desktop via the keyboard settings by selecting "A user-defined custom Layout". Here's an example for KDE Plasma.

![select layout](https://github.com/bridgesense/chinuk-wawa-custom-keyboard/blob/main/media/select_layout.jpeg?raw=true)

3. Toggle the keyboard layout using the taskbar or the keyboard shortcut appropriate to your Linux window manager. In KDE 

![toggle keyboard](https://github.com/bridgesense/chinuk-wawa-custom-keyboard/blob/main/media/toggle_keyboard.jpeg?raw=true)
## The Layout

![noramal state](https://github.com/bridgesense/chinuk-wawa-custom-keyboard/blob/main/media/cw_normal.jpeg?raw=true)

![shift state](https://github.com/bridgesense/chinuk-wawa-custom-keyboard/blob/main/media/cw_shift.jpeg?raw=true)

### Notes:

Although this keyboard works in most settings, xkb only allows the binding of one Unicode character to a single key. The letters `q̓`, `t̓`, `x̣`, and `ƛ̓` do not have a single Unicode equivalent. To use these characters it is necessary to type the letter twice, once in standard state and once in shift state.

For example to get the letter `q̓`, type q then shift+q.

One advantage to the xkb system is that it the keyboard is available in all applications, including the terminal.

![terminal example](https://github.com/bridgesense/chinuk-wawa-custom-keyboard/blob/main/media/terminal_example.jpeg?raw=true)
