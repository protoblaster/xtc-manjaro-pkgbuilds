# Maintainer: XTC <protoblaster11@protonmail.com>
pkgname=xtc-wallpapers
_pkgname=xtc-wallpapers
pkgver=1.0
pkgrel=1
pkgdesc="A collection of wallpapers found from various places on the Internet"
arch=('any')
url="https://github.com/protoblaster/xtc-wallpapers.git"
license=('GPL')
makedepends=('git')
provides=("${pkgname}")
options=(!strip !emptydirs)
source=("git+${url}")
md5sums=('SKIP')

package() {
	cd "${srcdir}/${pkgname}"
	install -d "${pkgdir}/usr/share/backgrounds/${_pkgname}"
	install -m644 ${srcdir}/${pkgname}/*.jpg "${pkgdir}/usr/share/backgrounds/${_pkgname}"
	install -m644 ${srcdir}/${pkgname}/*.png "${pkgdir}/usr/share/backgrounds/${_pkgname}"
}
