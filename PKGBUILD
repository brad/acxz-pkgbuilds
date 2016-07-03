# Maintainer: Anselmo L. S. Melo <anselmo.melo@intel.com>
pkgname=qgroundcontrol
pkgver=2.9.7b
pkgrel=1
pkgdesc="Micro air vehicle ground control station."
arch=('any')
url="http://qgroundcontrol.org/"
license=('GPL3')
conflicts=('qgroundcontrol-git')
depends=(\
  'espeak'  # optional but you have to decide if you want it at built-time\
  'qt5-svg' 'qt5-graphicaleffects' 'qt5-webkit' 'phonon-qt4' 'qt5-serialport'\
  'qt5-quickcontrols')

source=('https://github.com/mavlink/qgroundcontrol/releases/download/v2.9.7b/qgroundcontrol.tar.bz2')
md5sums=('64cad9e9597e2896602c6a1480ff9829')

package() {
  mkdir -p "${pkgdir}/opt" "${pkgdir}/usr/bin"
  cp -R "$srcdir/${pkgname}" "${pkgdir}/opt/qgroundcontrol"
  ln -s "${pkgdir}/opt/qgroundcontrol/qgroundcontrol-start.sh" "${pkgdir}/usr/bin/qgroundcontrol"
}

# vim:set ts=2 sw=2 et:
