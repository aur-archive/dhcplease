# Maintainer : Igor Duarte Cardoso <igordcard@gmail.com>
# Developer  : Igor Duarte Cardoso <igordcard@gmail.com>
# Changed since 1.0.0-3: Fixed "conflicts".
pkgname=dhcplease
pkgver=1.0.0
pkgrel=4
pkgdesc="dhcplease is an application for GNU/Linux that parses a DHCP (binary) lease file right away. Useful with dhcpcd lease files (/var/lib/dhcpcd/)"
arch=('i686' 'x86_64')
url="https://github.com/igordcard/dhcplease"
license=('GPL3')
depends=()
makedepends=()
provides=('dhcplease')
conflicts=('dhcplease-git')
source=("https://github.com/igordcard/dhcplease/archive/v$pkgver.tar.gz")
md5sums=('f29058660d3a219da41c672d56cb4748')

build() {
  cd "$srcdir/$pkgname-$pkgver"
  gcc $pkgname.c -o $pkgname
}

package() {
  cd "$srcdir/$pkgname-$pkgver"
  mkdir -p $pkgdir/usr/bin
  cp $pkgname $pkgdir/usr/bin/
}