# Maintainer: Parch Linux Team <team@parchlinux.org>
# Based on raspi-config by RPi-Distro

pkgname=parch-config
pkgver=1.0
pkgrel=1
pkgdesc="Parch Linux Configuration Tool - Desktop/WSL/Server/RPi"
arch=('any')
url="https://github.com/parchlinux/parch-config"
license=('AGPL3')
depends=(
    'alsa-utils'
    'parted'
    'psmisc'
    'dconf'
    'i2c-tools'
    'rfkill'
    'wpa_supplicant'
    'networkmanager'
)
optdepends=(
    'iw: WiFi configuration'
    'xorg-xrandr: display configuration'
    'plymouth: boot splash'
    'picom: compositor'
    'ufw: firewall'
    'docker: containers'
    'reflector: mirror ranking'
    'nvidia: NVIDIA GPU support'
)
provides=('parch-config')
conflicts=('raspi-config')
source=("git+https://github.com/parchlinux/parch-config.git")
sha256sums=('SKIP')

package() {
    install -dm750 "${pkgdir}/etc/sudoers.d/"
    install -dm755 "${pkgdir}/usr/lib/parch-config"
    install -dm755 "${pkgdir}/usr/share/parch-config"
    install -dm755 "${pkgdir}/usr/bin"

    install -Dm755 "${srcdir}/${pkgname}/parch-config" "${pkgdir}/usr/bin/parch-config"
    install -Dm440 "${srcdir}/${pkgname}/etc/sudoers.d/010_proxy" "${pkgdir}/etc/sudoers.d/010_proxy"
    install -Dm644 "${srcdir}/${pkgname}/autologin@.service" "${pkgdir}/usr/lib/systemd/system/autologin@.service"

    if [ -d "${srcdir}/${pkgname}/usr/lib/raspi-config" ]; then
        cp -r "${srcdir}/${pkgname}/usr/lib/raspi-config/"* "${pkgdir}/usr/lib/parch-config/"
    fi

    if [ -d "${srcdir}/${pkgname}/usr/share/raspi-config" ]; then
        cp -r "${srcdir}/${pkgname}/usr/share/raspi-config/"* "${pkgdir}/usr/share/parch-config/"
    fi
}
