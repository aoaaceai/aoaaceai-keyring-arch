pkgname=aoaaceai-keyring
pkgver=2021080701
pkgrel=1
pkgdesc='PGP keyring for aoaaceai arch repo'
arch=('any')
license=('GPL')
url='https://github.com/aoaaceai/aoaaceai-keyring'
source=("$url/archive/refs/tags/$pkgver.tar.gz")
install="$pkgname".install
sha256sums=('d1072292beb4b071ecc1553289b2376b4a3565e185a34e58da80975a6451bfe3')

package() {
    cd "$pkgname-$pkgver"

    install -Dm644 aoaaceai.gpg $pkgdir/usr/share/pacman/keyrings/aoaaceai.gpg
    install -Dm644 aoaaceai-revoked $pkgdir/usr/share/pacman/keyrings/aoaaceai-revoked
    install -Dm644 aoaaceai-trusted $pkgdir/usr/share/pacman/keyrings/aoaaceai-trusted

}
