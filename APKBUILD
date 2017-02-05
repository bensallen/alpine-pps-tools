# Contributor:
# Maintainer:
_gitver=47333f24af878f67ce48022e8af16419713aa1ac
pkgname=pps-tools
pkgver=20170205.g${_gitver:0:7}
pkgrel=0
pkgdesc="User-space tools for LinuxPPS"
url="https://github.com/ago/pps-tools"
arch="all"
license="GPL2"
depends=""
makedepends=""
install=""
subpackages="$pkgname-dev"
source="$pkgname-$_gitver.tar.gz::https://github.com/ago/pps-tools/archive/$_gitver.tar.gz"

builddir="$srcdir/$pkgname-$_gitver"

build() {
	cd "$builddir"
	make
}

package() {
	cd "$builddir"
	install -d $pkgdir/usr/bin
	install -d $pkgdir/usr/include/sys
	make DESTDIR=$pkgdir install
}

md5sums="2c3f4bbb7a1461d969be4febf2689e42  pps-tools-47333f24af878f67ce48022e8af16419713aa1ac.tar.gz"
sha256sums="eee0a76118cf11d94f575ee43804a6991379f2c734b400ba01ac4811d0498e97  pps-tools-47333f24af878f67ce48022e8af16419713aa1ac.tar.gz"
sha512sums="06373cf6e1b599be020c56ef81324ff9d622eb9b5235c6e5cb79765f7c617528aedff3e2da9d58f070faf5e5a68df7e50f0f9ad50d76a5a5ec0cd007f5dbcef3  pps-tools-47333f24af878f67ce48022e8af16419713aa1ac.tar.gz"
