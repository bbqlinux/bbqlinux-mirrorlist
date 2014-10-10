# Maintainer: Daniel Hillenbrand <codeworkx [at] bbqlinux [dot] org>

pkgname=bbqlinux-mirrorlist
pkgver=20141010
pkgrel=1
pkgdesc="BBQLinux mirrorlist for use by pacman"
arch=('any')
url="https://github.com/bbqlinux/bbqlinux-mirrorlist"
license=('GPL')
backup=(etc/pacman.d/bbqlinux-mirrorlist)

build() {
    cd "$srcdir"

    rm -f bbqlinux-mirrorlist
    curl -o bbqlinux-mirrorlist http://mirrorlist.bbqlinux.org
}

package() {
    cd "$pkgdir"

    mkdir -p $pkgdir/etc/pacman.d
    install -m644 $srcdir/bbqlinux-mirrorlist $pkgdir/etc/pacman.d/
}
