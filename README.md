<div align="center">

# ⚙️ Better Control ⚙️

<img src="https://github.com/user-attachments/assets/21a9f732-28a0-4da4-b0ff-9f9093cb2b3b" width="650">

### *A sleek GTK-themed control panel for Linux* 🐧

[![AUR Package](https://img.shields.io/badge/AUR-better--control--git-429768?style=flat-square&logo=archlinux&logoColor=white&labelColor=444)](https://aur.archlinux.org/packages/better-control-git)
[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-429768.svg?style=flat-square&logo=github&labelColor=444)](LICENSE)
[![GitHub stars](https://img.shields.io/github/stars/quantumvoid0/better-control?style=flat-square&color=429768&logo=polestar&labelColor=444)](https://github.com/quantumvoid0/better-control/stargazers)
[![Latest Release](https://img.shields.io/github/v/release/quantumvoid0/better-control.svg?style=flat-square&color=429768&logo=speedtest&label=latest-release&labelColor=444)](https://github.com/quantumvoid0/better-control/releases/latest)

</div>
<br>

> [!IMPORTANT]
> 🚧 This project is under active development. Contributions, feature requests, ideas, and testers are welcome!

<br>

## ✨ Features

- 🔄 Seamless integration with your desktop environment
- 📱 Modern, clean interface for system controls
- 🎚️ Quick access to common system settings
- 🌙 Respects your system's light/dark theme settings
- 🧩 Modular design - use only what you need (see dependencies for more info)

## Dependencies
<details>
<summary><b>Dependencies</b></summary>
  
Before installing, ensure you have `git` and `base-devel` installed.

### Core Dependencies

| Dependency | Purpose |
|------------|---------|
| **GTK 3** | UI framework |
| **Python Libraries** | python-gobject, python-dbus, python-psutil, python-setproctitle |

### Feature-Specific Dependencies

| Feature | Required Packages |
|---------|------------------|
| **Wi-Fi Management** | NetworkManager, python-qrcode |
| **Bluetooth** | BlueZ & BlueZ Utils |
| **Audio Control** | PipeWire or PulseAudio |
| **Brightness** | brightnessctl |
| **Power Management** | power-profiles-daemon, upower |
| **Blue Light Filter** | gammastep |
| **USBGuard** | usbguard |
| **pillow** | for qrcode on wifi |

> [TIP]
> If you don't need a specific feature, you can safely omit its corresponding dependency and hide its tab in the settings.

</details>

# > 💾 Installation

<details>
<summary><b>🏗️ Arch-based Distributions</b></summary>

```bash
yay -S better-control-git
```
If you dont have an AUR helper like yay above , follow the steps below
```
git clone https://aur.archlinux.org/better-control-git.git
cd better-control-git
makepkg -si
```

</details>

<details>
<summary><b>❄️ Nix (Unofficial)</b></summary>

> This is an unofficial Nix flake maintained by the community. All issues related to it should be directed to their repository:
> 
> https://github.com/Rishabh5321/better-control-flake
</details>

<details>
<summary><b>🐧 Debian-based Distributions</b></summary>

```bash
sudo apt update && sudo apt install -y libgtk-3-dev network-manager bluez bluez-utils pulseaudio brightnessctl python3-gi python3-dbus python3 power-profiles-daemon gammastep python3-requests python3-qrcode python3-setproctitle python3-pil usbguard
```
```bash
git clone https://github.com/quantumvoid0/better-control.git
cd better-control
make
sudo make install
```
</details>

<details>
<summary><b>🎩 Fedora-based Distributions</b></summary>

```bash
sudo dnf install -y gtk3 NetworkManager bluez bluez-utils pulseaudio brightnessctl python3-gobject python3-dbus python3 power-profiles-daemon gammastep python3-requests python3-qrcode python3-setproctitle python3-pillow usbguard

```
```bash
git clone https://github.com/quantumvoid0/better-control.git
cd better-control
make
sudo make install
```
</details>

<details>
<summary><b>🌀 Void Linux</b></summary>

```bash
sudo xbps-install -S NetworkManager pulseaudio brightnessctl python3-gobject python3-dbus python3 power-profiles-daemon gammastep python3-requests python3-qrcode gtk+3 bluez python3-Pillow usbguard
sudo xbps-install -S python3-pip
pip install setproctitle

```
```bash
git clone https://github.com/quantumvoid0/better-control.git
cd better-control
make
sudo make install
```
</details>

<details>
<summary><b>🏔️ Alpine Linux</b></summary>

```bash
sudo apk add gtk3 networkmanager bluez bluez-utils pulseaudio brightnessctl py3-gobject py3-dbus python3 power-profiles-daemon gammastep py3-requests py3-qrcode py3-pip py3-setuptools gcc musl-dev python3-dev py3-pillow
pip install setproctitle

```
```bash
git clone https://github.com/quantumvoid0/better-control.git
cd better-control
make
sudo make install
```

</details>

# > 🗑️ Uninstallation

<details>
<summary><b>🏗️ Arch-based Distributions</b></summary>

```bash
sudo pacman -R better-control-git
```
> The above lines will not remove the dependencies , but if you want to remove dependencies use the lines below:
```
sudo pacman -Rns better-control-git
```
</details>

<details>
<summary><b>📦 Other Distributions</b></summary>
  
```bash
git clone https://github.com/quantumvoid0/better-control
cd better-control
sudo make uninstall
```
</details>

# > Usage

`control` or `better-control` command will run the gui application. use `control --help` or `better-control --help` to see more specific launch commands

## Keybindings

| Keybinding | Action |
|------------|--------|
| `Shift + S` | Open Settings Dialog |
| `Q` or `Ctrl + Q` | Quit Application |

# > 📚 Contribution
Feel free to propose PR and suggest new features, improvements. If you wish to contribute with translation for the app into your language, please see the `utils/translations.py` file.


## 📄 License

This project is licensed under the GNU General Public License v3.0. See the [LICENSE](LICENSE) for more details.


# > 🧪 Compatibility Matrix

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

<div align="center">

### Made with ❤️ for the Linux community

[Report Bug](https://github.com/quantumvoid0/better-control/issues) • 
[Request Feature](https://github.com/quantumvoid0/better-control/discussions) • 
[Contribute](https://github.com/quantumvoid0/better-control/tree/main?tab=readme-ov-file#--contribution)

</div>
