# Maintainer: Daniel Hillenbrand <codeworkx [at] bbqlinux [dot] org>

pkgname=bbqlinux-mirrorlist
pkgver=20141008
pkgrel=2
pkgdesc="BBQLinux mirrorlist for use by pacman"
arch=('any')
url="https://github.com/bbqlinux/bbqlinux-mirrorlist"
license=('GPL')
backup=(etc/pacman.d/bbqlinux-mirrorlist)

package() {
  cd "$pkgdir"

  mkdir -p $pkgdir/etc/pacman.d
  install -m644 $srcdir/bbqlinux-mirrorlist $pkgdir/etc/pacman.d/
}
