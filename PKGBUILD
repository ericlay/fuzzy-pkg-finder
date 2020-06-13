# Maintainer: Eric Lay <ericlaytm@gmail.com>
pkgname=fuzzy-pkg-finder
pkgver=0.2
pkgrel=1
pkgdesc="Simple cli command for using fzf to search and install packages"
arch=(any)
url="https://github.com/ericlay/$pkgname"
license=('GPL')
depends=('pacman'
    'yay'
    'fzf')
makedepends=('git')
source=("git+https://gitlab.com/airclay/fuzzy-pkg-finder.git#tag=$pkgver")
md5sums=('SKIP')

package() {
	cd "$srcdir"
	install -dm755 $pkgdir/usr/bin
	cp -r $srcdir/$pkgname/fpf $pkgdir/usr/bin/
	chmod a+x $pkgdir/usr/bin/*
	install -dm755 "$pkgdir"/usr/lib/systemd/system/
	install -m644 $srcdir/$pkgname/fpf.{service,timer} "$pkgdir"/usr/lib/systemd/system/

	echo
	echo
	echo -------------------------------------
	echo   'Please start/enable fpf service'
	echo  'See git installation instructions'
	echo -------------------------------------
	echo
	echo
}
