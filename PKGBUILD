# Maintainer: Jan Honnens
# Contributors: Dan Serban, Mark Doe, L42y

pkgname=geierlein
pkgver=0.6.5
pkgrel=1
pkgdesc="Client for german tax statement for ELSTER"
url=http://stesie.github.com/geierlein/
arch=(any)
license=(AGPLv3)
depends=('firefox')
source=("https://github.com/stesie/geierlein/archive/V${pkgver}.zip"
        "geierlein.sh" "geierlein.desktop")


build()
{
    echo ""
}

package ()
{
	mkdir -p ${pkgdir}/opt/geierlein
    cp -r ${srcdir}/${pkgname}-${pkgver}/* ${pkgdir}/opt/geierlein
	mkdir -p ${pkgdir}/usr/local/bin
	mkdir -p ${pkgdir}/usr/share/applications
	install -m 755 geierlein.sh ${pkgdir}/usr/local/bin/geierlein
	install -m 644 geierlein.desktop ${pkgdir}/usr/share/applications/geierlein.desktop
    #sed -i 's/^MaxVersion=31/MaxVersion=32/g' ${pkgdir}/opt/geierlein/application.ini
}
md5sums=('2525ebfaeca5ce2a4fadb2ad20159ba1'
         '4556d0b36a9206e32d8185b84667fd1c'
         '163b30d86dad8a9f00ea8111d7b8fe42')
