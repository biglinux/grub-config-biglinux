# Maintainer: Bruno Goncalves <biglinux.com.br>

pkgname=grub-config-biglinux
pkgver=1_r3_2019_06_09
pkgrel=1
arch=('any')
license=('')
url="https://github.com/biglinux/grub-config-biglinux"
pkgdesc="Change grub configuration to BigLinux"

source=('git+https://github.com/biglinux/grub-config-biglinux.git')
sha256sums=('SKIP')
makedepends=('git')
install=${pkgname}.install

pkgver() {
    cd ${pkgname}
    printf "1_r$(git rev-list --count HEAD)_$(date "+%Y_%m_%d")"
}


package() {
    depends=('grub')
    
    cp -r "${srcdir}/${pkgname}/usr" "${pkgdir}/usr"
}

