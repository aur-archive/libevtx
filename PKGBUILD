# Maintainer: Jeremy M. <jskier at gmail dot com>
# Contributor: Jeremy M. <jskier at gmail dot com>

pkgname=libevtx
pkgver=20140901
pkgrel=1
pkgdesc="Library and tooling to access the Windows XML Event Log (EVTX) format"
url="https://code.google.com/p/libevtx"
license=('Lesser GPL')
arch=('i686' 'x86_64')
depends=('python')
source=(https://googledrive.com/host/0B3fBvzttpiiSRnQ0SExzX3JjdFE/${pkgname}-alpha-${pkgver}.tar.gz)
md5sums=('6d57d120d454274037d9647d639958d7')

build() {
	  cd "$srcdir"/${pkgname}-${pkgver}
	    ./configure --prefix=/usr
	      make
}

package() {
	        cd "$srcdir"/${pkgname}-${pkgver}
		  make DESTDIR="${pkgdir}" install
}
