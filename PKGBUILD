# Maintainer: Alvin Alvarado <alvin@striczkof.io>
exit 1 # Not working yet, don't use.
pkgname=striczkofs-archscripts-git
pkgver='0.1'
pkgrel=1
pkgdesc="Personal scripts for Arch Linux."
arch=('any')
url='https://github.com/striczkof/striczkofs-archscripts'
license=('GPLv3')
depends=()
makedepends=()
checkdepends=()
optdepends=('systemd: for systemd services'
            'openrc: for OpenRC boot scripts')
conflicts=()
replaces=()
backup=()
options=()
changelog='Initial git release.'
source=("$pkgname-$pkgver.tar.gz")
noextract=()
sha256sums=()
validpgpkeys=()


check() {
	cd "$pkgname-$pkgver"
	make -k check
}

package() {
	cd "$pkgname-$pkgver"
	make DESTDIR="$pkgdir/" install
}
