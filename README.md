# Chinuk Wawa - XKB integration (Linux)

Chinuk Wawa is an indigenous trade language once extensively used throughout the Pacific Northwest by Native American tribes. It is taught in an immersive classroom setting by the [Confederated Tribes of Grand Ronde](https://www.grandronde.org/services/education/shawash-ili%CA%94i-skul/). Remote learning and academic accreditation for Chinuk Wawa is available through [Lane Community College](https://www.lanecc.edu/programs-academics/academic-departments/humanities-division/language-studies-department/chinuk-wawa).

This installs a Chinuk Wawa custom keyboard onto most Linux distributions without the need of additional software.

## Installation

1. Open a terminal and run the following command. You will need the root password to install a single text file to system.
```
sudo curl -o /usr/share/X11/xkb/symbols/custom "https://raw.githubusercontent.com/bridgesense/chinuk-wawa-custom-keyboard/refs/heads/main/custom"
```
2. Activate the layout on your desktop via the keyboard settings by selecting "A user-defined custom Layout". Here's an example for KDE Plasma. You may also need to add an additional keyboard layout for toggling between the two.

![select layout](https://github.com/bridgesense/chinuk-wawa-custom-keyboard/blob/main/media/select_layout.jpeg?raw=true)

3. Toggle the keyboard layout using the taskbar or the keyboard shortcut appropriate to your Linux window manager. In KDE the shortcut is Meta+Alt+k.

![toggle keyboard](https://github.com/bridgesense/chinuk-wawa-custom-keyboard/blob/main/media/toggle_keyboard.jpeg?raw=true)
## The Layout

![noramal state](https://github.com/bridgesense/chinuk-wawa-custom-keyboard/blob/main/media/cw_normal.jpeg?raw=true)

![shift state](https://github.com/bridgesense/chinuk-wawa-custom-keyboard/blob/main/media/cw_shift.jpeg?raw=true)

### Notes:

Although this keyboard works in most settings, xkb only allows the binding of one Unicode character to a single key. The letters `q̓`, `t̓`, `x̣`, and `ƛ̓` do not have a single Unicode equivalent. To use these characters it is necessary to type the letter twice, once in standard state and once in shift state.

For example to get the letter `q̓`, type q and then type shift+q.

One advantage to the xkb system is that the keyboard is available to all applications, including the terminal.

![terminal example](https://github.com/bridgesense/chinuk-wawa-custom-keyboard/blob/main/media/terminal_example.jpeg?raw=true)
