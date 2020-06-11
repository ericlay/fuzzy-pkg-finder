# Maintainer: Eric Lay <ericlaytm@gmail.com>
pkgname=fuzzy-pkg-finder
pkgver=0.1
pkgrel=1
pkgdesc="Simple cli command for using fzf to search and install packages"
arch=(any)
url="https://github.com/ericlay/$pkgname"
license=('GPL')
depends=('pacman'
    'yay'
    'fzf')
makedepends=('git')
#install= TODO add post install script to sync pacman file database.
source=("git://github.com/ericlay/$pkgname")
md5sums=('SKIP')

package() {
	cd "$srcdir"
	install -dm755 $pkgdir/usr/bin
	cp -r $scrdir/$pkgname/bin $pkgdir/usr
	chmod a+x $pkgdir/usr/bin/*
}
