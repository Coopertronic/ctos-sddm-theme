# Maintainer: Matthew Phillip Cooper <matthew@coopertronic.co.uk>
pkgname=ctos-sddm-theme
_destname1="/usr"
pkgver=1.r3.4712599
pkgrel=1
pkgdesc="This installs the SDDM theme for KDE plasma by Matthew Phillip Cooper."
arch=('any')
url="https://github.com/Coopertronic/ctos-sddm-theme.git"
license=('GPL3')
makedepends=('git')
depends=()
conflicts=()
provides=("${pkgname}")
options=(!strip !emptydirs)
source=("git+$url")
sha256sums=('SKIP')

pkgver() {
    printf "1.r%s.%s" "$(git rev-list --count HEAD)" "$(git rev-parse --short HEAD)"
}

package() {
	install -dm755 ${pkgdir}${_destname1}
	cp -r ${srcdir}/${pkgname}${_destname1}/* ${pkgdir}${_destname1}
}
