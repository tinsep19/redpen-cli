# -*- mode:shell-script -*-
# This is an example PKGBUILD file. Use this as a start to creating your own,
# and remove these comments. For more information, see 'man PKGBUILD'.
# NOTE: Please fill out the license field for your package! If it is unknown,
# then please put 'unknown'.

# Maintainer: Your Name <youremail@domain.com>
pkgname=redpen-cli
pkgver=1.1
pkgrel=2
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
source=(https://github.com/recruit-tech/redpen/releases/download/v$pkgver.$pkgrel/$pkgname-$pkgver.$pkgrel.tar.gz redpen.run)
noextract=()
md5sums=(f90912218bf6207a6dd82808cca6752b 034bb2ae2fe1e4c22796c2aa9507e166)
validpgpkeys=()

package() {
    install -m 755 -D "$srcdir/redpen.run" "$pkgdir/usr/bin/redpen"
    for i in $srcdir/$pkgname-$pkgver/{conf,lib}/*
    do
	f=${i##$srcdir/$pkgname-$pkgver}
	install -D $i $pkgdir/usr/share/java/$pkgname/$f
    done
}

