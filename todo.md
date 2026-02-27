# parch-config Todo List

## High Priority

### 1. Kernel & Boot
- [ ] Add kernel update/removal option (linux-zen, linux-lts, etc.)
- [ ] Add bootloader config (GRUB, systemd-boot)
- [ ] Add early KMS driver loading
- [ ] Add kernel parameters editor

### 2. Desktop Features
- [ ] Add multiple monitor/display config
- [ ] Add Wayland vs X11 selection/info
- [ ] Add HiDPI scaling config
- [ ] Add theming (GTK, Qt, icons)
- [ ] Add cursor/theme configuration
- [ ] Add automatic driver switching (PRIME)

### 3. Server Features  
- [ ] Add fail2ban config wizard
- [ ] Add SSH key management (generate, add)
- [ ] Add cron/anacron config
- [ ] Add systemd service management
- [ ] Add log viewer/cleanup
- [ ] Add backup configuration

### 4. Package Management
- [ ] Add package group installer (base, base-devel, etc.)
- [ ] Add AUR package browser/info
- [ ] Add orphan package cleaner
- [ ] Add pacman.conf editor (parallel downloads, color)

### 5. Hardware
- [ ] Add Bluetooth device pairing
- [ ] Add printer config (CUPS)
- [ ] Add scanner config
- [ ] Add webcam config
- [ ] Add sound card selection
- [ ] Add touchpad config

## Medium Priority

### 6. System Info
- [ ] Add system benchmark option
- [ ] Add hardware info (inxi integration)
- [ ] Add disk health check (SMART)
- [ ] Add temperature monitoring
- [ ] Add memory/CPU usage viewer

### 7. Security
- [ ] Add AppArmor/SELinux config
- [ ] Add sysctl tuning (performance/security)
- [ ] Add encryption config (LUKS)
- [ ] Add user management (add/remove)

### 8. Networking
- [ ] Add VPN config (WireGuard, OpenVPN)
- [ ] Add host file editor
- [ ] Add network shares (Samba/NFS)
- [ ] Add proxy configuration

### 9. WSL Specific
- [ ] Add WSL specific GPU install (directx, vulkan)
- [ ] Add WSL backup/export
- [ ] Add WSL version switch (WSL1/WSL2)

### 10. RPi Specific (aarch64)
- [ ] Add camera enable/disable
- [ ] Add jack/headphone config
- [ ] Add USB boot config
- [ ] Add bootloader update

## Low Priority

### 11. User Experience
- [ ] Add theming to parch-config itself
- [ ] Add dark/light mode
- [ ] Add config backup/restore
- [ ] Add preset profiles (gaming, server, minimal)
- [ ] Add changelog viewer

### 12. Parch Specific
- [ ] Add Parch ISO downloader
- [ ] Add Parch repo configuration
- [ ] Add Parch-specific packages installer
- [ ] Add welcome screen info
- [ ] Add live USB creator

### 13. Maintenance
- [ ] Add system update all
- [ ] Add orphan packages cleaner
- [ ] Add journal cleanup
- [ ] Add old kernel remover
- [ ] Add tmp cleanup

### 14. Integration
- [ ] Add hardware detection auto-install
- [ ] Add gaming setup (Steam, Proton)
- [ ] Add Flatpak/Flathub config
- [ ] Add Snap support

## Ideas for Future

### AI/ML
- [ ] Add Ollama/LM Studio setup
- [ ] Add CUDA/cuDNN config for NVIDIA

### Containers
- [ ] Add Podman config
- [ ] Add Kubernetes/k3s installer

### Virtualization
- [ ] Add VirtualBox config
- [ ] Add QEMU/KVM config
- [ ] Add libvirt manager

---

## Quick Wins to Implement

1. **Kernel management** - Switch between kernels
2. **GRUB customizer** - Theme, timeout, entries
3. **Mirror tester** - Interactive mirror selection
4. **Font installer** - Popular fonts quick install
5. **Codec pack** - Multimedia codecs
6. **Steam setup** - Gaming ready
7. **VirtualBox guest** - Guest additions
8. **Samba config** - File sharing
9. **NFS config** - Network filesystems
10. **Cron editor** - Task scheduler UI
