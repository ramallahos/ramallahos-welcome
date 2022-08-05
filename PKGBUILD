# Maintainer: Safwan Nayeem Yousuf <safwannayeemyousuf.com>
pkgname=ramallahos-welcome
pkgver=1
pkgrel=1
pkgdesc="Welcome app for RamallahOS"
arch=('any')
url="https://github.com/ramallahos/$pkgname"
license=('GPL')
depends=('yad' 'ramallahos-about' 'ramallahos-help' 'ramallahos-tweaks' 'ramallahos-calamares')
makedepends=('coreutils')
source=("$pkgname::git+$url.git")
sha256sums=('SKIP')

package() {
    cd "$pkgname"
    install -d "$pkgdir/usr/bin/$pkgname-resources/"
    install -Dm755 "$pkgname" "$pkgdir/usr/bin/$pkgname"
    install -Dm755 hello.gif "$pkgdir/usr/bin/$pkgname-resources/hello.gif"
    install -Dm755 welcome.html "$pkgdir/usr/bin/$pkgname-resources/welcome.html"
    install -Dm755 "$pkgname.desktop" "$pkgdir/usr/share/applications/$pkgname.desktop"
    install -Dm644 LICENSE.md "$pkgdir/usr/share/licenses/$pkgname/LICENSE"
}
