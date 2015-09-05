# -*- mode:shell-script -*-
# This is an example PKGBUILD file. Use this as a start to creating your own,
# and remove these comments. For more information, see 'man PKGBUILD'.
# NOTE: Please fill out the license field for your package! If it is unknown,
# then please put 'unknown'.

# Maintainer: Your Name <youremail@domain.com>
pkgname=redpen
pkgver=1.3
pkgrel=0
epoch=
pkgdesc="A proofreading tool to help writers or programmers."
arch=(any)
url="http://redpen.cc"
license=('Apache')
groups=()
depends=("jre8-openjdk")
makedepends=()
checkdepends=()
optdepends=()
provides=()
conflicts=()
replaces=()
backup=()
options=()
install=
changelog=
source=(https://github.com/recruit-tech/redpen/releases/download/v$pkgver.$pkgrel/$pkgname-$pkgver.$pkgrel.tar.gz)
noextract=()
md5sums=(e9dfc9d2bb6f2e7cc30bf00bb6debdce)
validpgpkeys=()

package() {
    mkdir -p $pkgdir/usr/share/java
    mkdir -p $pkgdir/usr/bin
    cp -r $srcdir/$pkgname-distribution-$pkgver $pkgdir/usr/share/java/$pkgname
    ln -s $pkgdir/usr/share/java/$pkgname/bin/redpen $pkgdir/usr/bin/redpen
}

