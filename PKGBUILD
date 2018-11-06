# Maintainer: Hexchain Tong <i@hexchain.org>
pkgname=git-credential-gnome-keyring
pkgver=2.19.1
pkgrel=1
pkgdesc="Git credential helper using GNOME Keyring"
arch=(i686 x86_64)
url="https://github.com/git/git/tree/master/contrib/credential/gnome-keyring"
license=('GPL')
depends=('git' 'libgnome-keyring')
makedepends=('git')
source=("https://www.kernel.org/pub/software/scm/git/git-$pkgver.tar.xz")

build() {
    cd "$srcdir/git-$pkgver/contrib/credential/gnome-keyring"
    make
}

package() {
    cd "$srcdir/git-$pkgver/contrib/credential/gnome-keyring"
    install -Dm755 git-credential-gnome-keyring -t "$pkgdir/usr/bin"
}
sha256sums=('345056aa9b8084280b1b9fe1374d232dec05a34e8849028a20bfdb56e920dbb5')
