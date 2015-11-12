 # Maintainer: Adolfo silerio

pkgname=oranchelo-icon-theme
pkgver=5.0
pkgrel=1
pkgdesc="XFCE and GNOME flat icons"
arch=(any)
depends=()
makedepends=('git')
url="https://github.com/Madh93/oranchelo-icon-theme.git"
license=('GPL3')
groups=('gnome' 'xfce')
conflicts=('oranchelo-icon-theme')
provides=("oranchelo-icon-theme")
source=('git+https://github.com/Madh93/oranchelo-icon-theme.git')
md5sums=('SKIP')

pkgver() {
cd $srcdir/$_pkgname
echo $(git rev-list --count HEAD).$(git rev-parse --short HEAD)
}

package() {

install -d -m 755 "$pkgdir"/usr/share/icons/Oranchelo
install -d -m 755 "$pkgdir"/usr/share/icons/Oranchelo-Green


cd $srcdir/Oranchelo
cp -r . "$pkgdir"/usr/share/icons/Oranchelo/
cd $srcdir/Oranchelo-Green
cp -r . "$pkgdir"/usr/share/icons/Oranchelo-green/

}
