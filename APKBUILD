# Contributor: Matias Insaurralde <matias@insaurral.de>
# Maintainer: Matias Insaurralde <matias@insaurral.de>
pkgname=php-amqp
pkgver=1.6.1
pkgrel=0
pkgdesc="PHP AMQP Binding Library"
url="https://github.com/pdezwart/php-amqp"
arch="all"
license="PHP"
depends="librabbitmq"
depends_dev="librabbitmq-dev"
makedepends="$depends_dev"
install=""
subpackages="$pkgname-dev $pkgname-doc"
source="$pkgname-$pkgver.tar.gz::https://github.com/pdezwart/php-amqp/archive/v$pkgver.tar.gz"

_builddir=
prepare() {
	local i
	cd "$_builddir"
	for i in $source; do
		case $i in
		*.patch) msg $i; patch -p1 -i "$srcdir"/$i || return 1;;
		esac
	done
}

build() {
	cd "$_builddir"
}

package() {
	cd "$_builddir"
}

md5sums="599f83662bb9025d36f6077f935e679e  php-amqp-1.6.1.tar.gz"
sha256sums="5473d18e2662d7b9c93cc9fb4382d0f93abbd90bbf8c4850cf4ed2f7ccb2d48d  php-amqp-1.6.1.tar.gz"
sha512sums="e06df186ccb80431ea6cba2bfb8a24804392616bfd774b18ee5d0d81286ccbc2c7b48c15892bf120b7a1dd9c19461e6ba7e9d3732e642af4f1075b4de3de51ac  php-amqp-1.6.1.tar.gz"
