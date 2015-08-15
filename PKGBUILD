# Maintainer: Custom Processing Unlimited <cpunltd[at]gmail[dot]com>
# Contributors: Wey (Archlinux forum user)
pkgname=cafepilot-client
pkgname1=CafePilot_Client
pkgver=2.1.0
pkgrel=3
pkgdesc="CafePilot is a cross-platform (Windows and Linux) client/server software suite that makes managing an Internet cafe of any size a breeze. This is the client program."
url="http://www.cafepilot.com"
arch=('any')
license=('GPL')
depends=('java-runtime')
# optdepends=('*')
# makedepends=()
# conflicts=()
# replaces=()
# backup=()
# install='*.install'
source=("http://sourceforge.net/projects/cafepilot/files/CafePilot/CafePilot%20Server%20and%20Client/CafePilot_Client.zip/download"
        "cafepilot-client.sh")
md5sums=('dced5ab343d52ea562f1ed889a35211a'
         'd0ebaad0a19f73ff1ca99a218d79da5d')

package() {
  cd "${srcdir}"
  install -Dm755 $pkgname.sh $pkgdir/usr/bin/$pkgname.sh
  install -Dm644 $pkgname1.jar $pkgdir/opt/$pkgname1/$pkgname1.jar
  cp -r "$srcdir"/lib/ "$pkgdir"/opt/$pkgname1/
}

# vim:set ts=2 sw=2 et:
