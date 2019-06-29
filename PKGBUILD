# Maintainer: Adolfo silerio
# Maintainer: Duvan Felipe Suarez <duvanera@gmail.com>
# Maintainer: Francisco Javier Ospina <francisco.ospina@gmail.com>
# Maintainer: Zechariah Thurman get@meongithub zthurman

pkgname=oranchelo-icon-theme
pkgver=0.7
pkgrel=1
pkgdesc='Oranchelo is a flat-design icon theme for XFCE4 based on Super Flat Remix and inspired by "Corny icons" by Patryk Goworowski.'
arch=(any)
depends=('git')
makedepends=('git')
url='https://github.com/OrancheloTeam/oranchelo-icon-theme.git'
license=('GPL3')
groups=('gnome' 'xfce')
conflicts=('oranchelo-icon-theme')
provides=('oranchelo-icon-theme')
source=('git+https://github.com/OrancheloTeam/oranchelo-icon-theme.git')
md5sums=('SKIP')

package() {

  install -d -m 755 "${pkgdir}/usr/share/icons/Oranchelo"
  install -d -m 755 "${pkgdir}/usr/share/icons/Oranchelo-Green"
  

  cd "${srcdir}/${pkgname}/Oranchelo"
  cp -r . "${pkgdir}/usr/share/icons/Oranchelo/"
  cd "${srcdir}/${pkgname}/Oranchelo-Green"
  cp -r . "${pkgdir}/usr/share/icons/Oranchelo-Green/"
}
