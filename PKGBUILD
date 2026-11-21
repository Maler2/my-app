pkgname=my-app
pkgver=1.0.0
pkgrel=1
pkgdesc="my first app"
arch=('x86_64')
license=('MIT')
depends=('gcc-libs')
source=("main.cpp")
sha256sums=('SKIP')

build() {
	g++ -O2 "$srcdir/main.cpp" -o "$srcdir/my-app"
}

package() {
	install -Dm755 "$srcdir/my-app" "$pkgdir/usr/bin/my-app"
}
