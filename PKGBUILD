# Maintainer: Eric Lay <ericlaytm@gmail.com>
pkgname=fuzzy-pkg-finder
pkgver=0.8
pkgrel=1
pkgdesc="Simple cli command for using fzf to search and install packages"
arch=(any)
url="https://github.com/ericlay/$pkgname"
license=('GPL')
depends=('pacman'
    'yay'
    'fzf')
makedepends=('git')
source=("git+https://gitlab.com/airclay/fuzzy-pkg-finder.git#tag=v$pkgver")
md5sums=('SKIP')

package() {
	cd "$srcdir"
	install -dm755 $pkgdir/usr/bin
	cp -r $srcdir/$pkgname/fpf $pkgdir/usr/bin/
	chmod a+x $pkgdir/usr/bin/*
}
