# Contributor: Elia Notarangelo < elia dot notarangelo at gmail dot com>
# Contributor: paky <pascoc at tiscali dot it>
# Manteiner: ale_xiovk < alexiobash at gmail dot com >

pkgname=sysinfo-sui
pkgver=0.2
pkgrel=1
pkgdesc="a shell user interface for system informations"
arch=('any')
url="http://www.xfce-italia.it/index.php?topic=952.0"
license=('GPL')
depends=('sudo' 'lshw' 'xorg-xrandr')
source=("http://master.dl.sourceforge.net/project/archmind/sysinfo-sui/$pkgname-$pkgver.tar.gz")


build() {
	cd ${srcdir}/${pkgname}-${pkgver}

	CONFIG_DIR=${pkgdir}/usr/share/${pkgname}
	BIN_DIR=${pkgdir}/usr/bin
	DOC_DIR=${pkgdir}/usr/share/doc/${pkgname}
	DESK_DIR=${pkgdir}/usr/share/applications
	ICON_DIR=${pkgdir}/usr/share/pixmaps
	MAN_DIR=${pkgdir}/usr/share/man/it/man1	

	install -d ${CONFIG_DIR} ${BIN_DIR} ${DOC_DIR} ${ICON_DIR} ${DESK_DIR} ${MAN_DIR}


	install -D logo ${CONFIG_DIR}
	install -D sysinfo-sui ${BIN_DIR}
	install -D copyright ${DOC_DIR}
	install -D sysinfo-sui.desktop ${DESK_DIR}
	install -D sysinfo-sui.png ${ICON_DIR}
	install -D sysinfo-sui.1x.gz ${MAN_DIR}	
}

md5sums=('b98a0e83eca166c651fdd40d03ce3db3')
