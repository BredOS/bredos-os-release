# Maintainer: Snehit Sah <snehitsah@protonmail.com>

pkgname=bred-os-release
fname=os-release
pkgver=1.0
pkgrel=1
pkgdesc="BredOS os-release file info"
arch=('any')
license=('GPL3')
backup=(usr/lib/os-release)
source=('os-release')
sha256sums=('7b17065f1e8a3cfda924b7fa478d9ce2d90f1a850b3ab69436704ad007fad65a')
install=${fname}.install

pkgver() {
    date +%Y%m%d
}

package() {
    mkdir -p ${pkgdir}/usr/lib/
    install -m644 ${srcdir}/${fname} ${pkgdir}/usr/lib/${fname}-new
}
