#Maintainer: Jove Yu <yushijun110 [at] gmail.com>

pkgname=wine-qq
pkgver=20121130
pkgrel=4
pkgdesc='wine version of QQ client,made by Longene Team.'
arch=('i686' 'x86_64')
url='http://www.longene.org/'
license=('Other')
source=("http://www.longene.org/download/WineQQ2012-20121130-Longene.deb")
md5sums=('00e31d228458c8096df97e0d8c94f60c')
if [ "$CARCH" = "i686" ]; then
depends=('gtk2' 'lcms' 'ncurses' 'alsa-plugins' 'libsm' 'libpng12')
elif [ "$CARCH" = "x86_64" ]; then
depends=('lib32-gtk2' 'lib32-lcms' 'lib32-ncurses' 'lib32-alsa-plugins' 'lib32-libsm' 'lib32-libpng12')
fi

package()
{
	tar xzvf ${srcdir}/data.tar.gz -C ${pkgdir}/
	chmod -R 755 ${pkgdir}/opt/longene
}
