# Parch Configuration Tool (parch-config)

<p align="center">
  <img src="https://raw.githubusercontent.com/parchlinux/art/master/logo.png" width="200" alt="Parch Linux Logo">
</p>

<p align="center">
  <a href="https://parchlinux.org">
    <img src="https://img.shields.io/badge/Parch-Linux-0d3de3?style=for-the-badge" alt="Parch Linux">
  </a>
  <a href="https://github.com/parchlinux/parch-config/blob/master/LICENSE">
    <img src="https://img.shields.io/badge/License-AGPL--3.0-green?style=for-the-badge" alt="License: AGPL-3.0">
  </a>
</p>

## About

**parch-config** is a configuration tool for Parch Linux, an Arch Linux-based distribution. It is based on [raspi-config](https://github.com/RPi-Distro/raspi-config) by the Raspberry Pi Foundation, adapted and extended for Parch Linux with smart features for Desktop, WSL, and Server usage.

## Features

### Platform Support

- **Raspberry Pi (aarch64)**: Full Raspberry Pi configuration including:
  - Overclocking, Device tree, SPI/I2C/Serial
  - Camera, Display options, GPIO fan, LEDs

- **x86_64 Desktop**: Smart desktop configuration:
  - **GPU Drivers** - Auto-detect NVIDIA/AMD/Intel, install/configure
  - **Display Manager** - Switch SDDM/GDM/LightDM/Ly with install
  - **Desktop Environment** - Install KDE/GNOME/XFCE/MATE/Cinnamon/Wayfire/Sway/Cosmic
  - **Screen Blanking** - Disable DPMS
  - **Resolution** - Change via xrandr
  - **Plymouth** - Boot splash screen
  - **Compositor** - Configure picom

- **WSL**: WSL-specific settings:
  - GPU acceleration (WSLg)
  - Memory limits
  - Windows interop
  - systemd toggle

- **Server**: System services and security:
  - SSH with hardening options
  - UFW Firewall
  - Docker container runtime
  - NetworkManager
  - SSH hardening (disable root, key-only auth, Fail2Ban)

### Display Manager Support

- **SDDM** - Simple Desktop Display Manager
- **GDM** - GNOME Display Manager
- **LightDM** - Lightweight Display Manager
- **Cosmic Greeter** - System76
- **Ly** - Terminal-based DM

### Package Manager

- Mirror ranking with reflector
- AUR helper (paru/yay) configuration
- Keyring updates
- Cache cleaning

### Locale & Time

- Timezone (timedatectl)
- Locale configuration
- Keyboard layout
- NTP sync

## Installation

```bash
# Build from source
git clone https://github.com/parchlinux/parch-config.git
cd parch-config
makepkg -si

# Or install with pacman (once published)
sudo pacman -S parch-config
```

## Usage

```bash
sudo parch-config
```

## License

AGPL-3.0 - See [LICENSE](LICENSE)

## Acknowledgments

- Raspberry Pi Foundation for raspi-config
- Arch Linux community
