# Maintainer: Stas Solovey <whats_up@tut.by>
pkgname=hunspell-be
pkgver=0.56
pkgrel=2
pkgdesc="Belarusian hunspell dictionaries"
arch=(any)
url="http://sourceforge.net/projects/spell-be/"
license=('CC-BY-SA 3.0')
depends=('hunspell')
makedepends=()
source=(http://downloads.sourceforge.net/project/spell-be/hunspell-be-0.56.zip)
sha1sums=('326108ccd3d78d5ee86facab5d347146b9a61220')

build() {
 /bin/true
}

package() {
cd "$srcdir"

install -dm755 ${pkgdir}/usr/share/hunspell
install -m644 be_BY.dic be_BY.aff $pkgdir/usr/share/hunspell

install -dm755 ${pkgdir}/usr/share/myspell/dicts
ln -s /usr/share/hunspell/be_BY.dic $pkgdir/usr/share/myspell/dicts/be_BY.dic
ln -s /usr/share/hunspell/be_BY.aff $pkgdir/usr/share/myspell/dicts/be_BY.aff
}
