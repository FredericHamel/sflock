pkgname=sflock
pkgver=1.0.0
pkgrel=0
pkgdesc="A secure lock screen for X11"
arch=('i686' 'x86_64')
license=('MIT')
depends=('libx11')

source=(https://github.com/FredericHamel/sflock/archive/1.0.0.tar.gz)

md5sums=('3f0854988a66e0c3b45a0ef2fc23fd5f')

build() {
  cd $srcdir/$pkgname-$pkgver
  make
}

package() {
  cd $srcdir/$pkgname-$pkgver
  make PREFIX=/usr DESTDIR=$pkgdir install
}


