# Maintainer: Aditya Shakya <adi1090x@gmail.com>

pkgname=gtk-themes
pkgver=1.0
pkgrel=1
pkgdesc="Adapta gtk theme for Archcraft"
arch=('any')
license=('GPL3')
makedepends=()
depends=()
conflicts=()
groups=()
provides=("${pkgname}")
options=(!strip !emptydirs)

prepare() {
	cp -af ../files/. ${srcdir}
}

package() {
	local _themesdir=${pkgdir}/usr/share/themes
	mkdir -p "$_themesdir"
	cp -r ${srcdir}/* "$_themesdir"
}
