
pkgname=bootnext
pkgver=1
pkgrel=1
pkgdesc="Shell script for setting next efiboot option"
arch=('any')
url="https://github.com/dominicdoty/efibootmgr_bootnext.git"
license=(	'GPLv3')
depends=(	'efibootmgr')
source=(	'bootnext'
		'LICENSE')
md5sums=(	'6dd69c5676a9586e4ff79d219a9366db'
		'1ebbd3e34237af26da5dc08a4e440464')
package() {
	install -D $srcdir/bootnext $pkgdir/usr/bin/$pkgname
	install -D -m644 $srcdir/LICENSE $pkgdir/usr/share/licenses/$pkgname/LICENSE
}
