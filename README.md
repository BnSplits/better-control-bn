# ⚙️ Better Control

<img src="https://github.com/user-attachments/assets/3ae2383d-971b-4280-bd64-6c6c18dd05de" width="650">

### _A sleek GTK-themed control panel for Linux_ 🐧

[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-429768.svg?style=flat-square&logo=github&labelColor=444)](LICENSE)
[![Latest Release](https://img.shields.io/github/v/release/quantumvoid0/better-control.svg?style=flat-square&color=429768&logo=speedtest&label=latest-release&labelColor=444)](https://github.com/quantumvoid0/better-control/releases/latest)

<br>

> [!IMPORTANT]
> 🚧 This project is under active development. Contributions, feature requests, ideas, and testers are welcome!

<br>

### ✨ Features

- 🔄 Seamless integration with your desktop environment
- 📱 Modern, clean interface for system controls
- 🎚️ Quick access to common system settings and ton of features
- 🌙 Respects your system's light/dark theme settings
- 🧩 Modular design - use only what you need and remove the ones you dont use (see dependencies for more info)

<details>
<summary><b>Dependencies</b></summary>
<br><br>
Before installing, ensure you have `git` and `base-devel` installed.

### Core Dependencies

| Dependency           | Purpose                                                         |
| -------------------- | --------------------------------------------------------------- |
| **GTK 3**            | UI framework                                                    |
| **Python Libraries** | python-gobject, python-dbus, python-psutil, python-setproctitle |

### Feature-Specific Dependencies

| Feature               | Required Packages             |
| --------------------- | ----------------------------- |
| **Wi-Fi Management**  | NetworkManager, python-qrcode |
| **Bluetooth**         | BlueZ & BlueZ Utils, papirus-icon-theme           |
| **Audio Control**     | PipeWire or PulseAudio        |
| **Brightness**        | brightnessctl                 |
| **Power Management**  | power-profiles-daemon, upower |
| **Blue Light Filter** | gammastep                     |
| **USBGuard**          | USBGuard                      |
| **pillow**            | For QR Code on wifi           |

> [TIP]
> If you don't need a specific feature, you can safely omit its corresponding dependency and hide its tab in the settings.

</details>

# 💾 Installation & Uninstallation

#### ➡️ Method 1 : Manual Build

> when you do maunal build make sure to get all dependencies by yourself

```bash
git clone https://github.com/BnSplits/better-control-bn.git
cd better-control-bn
sudo make install
```

<br>

# 🫴 Usage

`control` or `better-control` command will run the gui application. use `control --help` or `better-control --help` to see more specific launch commands you can use with stuff like waybar.

You can use `betterctl` to update or uninstall the application.

### Keybindings

| Keybinding        | Action               |
| ----------------- | -------------------- |
| `Shift + S`       | Open Settings Dialog |
| `Q` or `Ctrl + Q` | Quit Application     |

<br><br>

# 📚 Contribution

Feel free to propose PR and suggest new features, improvements. If you wish to contribute with translation for the app into your language, please see the `utils/translations.py` file.

## 📄 License

This project is licensed under the GNU General Public License v3.0. See the [LICENSE](LICENSE) for more details.

<br><br>

# 🧪 Compatibility Matrix

Better Control has been tested on Arch Linux with Hyprland, GNOME, and KDE Plasma. It should work on most Linux distributions with minor adjustments.

<table>
  <tr>
    <th align="center" width="200">Category</th>
    <th align="center">Compatibility</th>
  </tr>
  <tr>
    <td align="center"><b>Operating System</b></td>
    <td align="center">Linux</td>
  </tr>
  <tr>
    <td align="center"><b>Distributions</b></td>
    <td align="center">Arch-based ✓ • Fedora-based ✓ • Debian-based ✓ • Void ✓ • Alpine ✓</td>
  </tr>
  <tr>
    <td align="center"><b>Desktop Environments</b></td>
    <td align="center">GNOME (tested) ✓ • KDE Plasma (tested) ✓ • XFCE • LXDE/LXQT</td>
  </tr>
  <tr>
    <td align="center"><b>Window Managers</b></td>
    <td align="center">Hyprland (tested) ✓ • Sway (tested) ✓ • i3 • Openbox • Fluxbox</td>
  </tr>
  <tr>
    <td align="center"><b>Display Protocol</b></td>
    <td align="center">Wayland (recommended) ✓ • X11 (partial functionality)</td>
  </tr>
</table>

> [!NOTE]
> If you test Better Control on a different setup, please share your experience in the discussions or issues section.

<br>

### Made with ❤️ for the Linux community

[Report Bug](https://github.com/quantumvoid0/better-control/issues) •
[Request Feature](https://github.com/quantumvoid0/better-control/discussions) •
[Contribute](https://github.com/quantumvoid0/better-control/tree/main?tab=readme-ov-file#--contribution)
