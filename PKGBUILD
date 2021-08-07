pkgname=aoaaceai-keyring
pkgver=2021080702
pkgrel=1
pkgdesc='PGP keyring for aoaaceai arch repo'
arch=('any')
license=('GPL')
url='https://github.com/aoaaceai/aoaaceai-keyring'
source=("$url/archive/refs/tags/$pkgver.tar.gz")
install="$pkgname".install
sha256sums=('3fa3a73e118888289a5b945e7227f5d7b43a0d25a5657134ee48537b74d5f487')

package() {
    cd "$pkgname-$pkgver"

    install -Dm644 aoaaceai.gpg $pkgdir/usr/share/pacman/keyrings/aoaaceai.gpg
    install -Dm644 aoaaceai-revoked $pkgdir/usr/share/pacman/keyrings/aoaaceai-revoked
    install -Dm644 aoaaceai-trusted $pkgdir/usr/share/pacman/keyrings/aoaaceai-trusted

}
