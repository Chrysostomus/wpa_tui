# Maintainer: Chrysostomus @forum.manjaro.org
pkgname=wpa_tui
pkgver=0.1
pkgrel=1
pkgdesc="systemd hook to hibernate suspended system after a delay"
arch=(any)
url="https://github.com/Chrysostomus/$pkgname"
license=("MIT")
depends=('systemd'
		'wpa_supplicant'
		'bash')
makedepends=('git')
source=("git://github.com/Chrysostomus/$pkgname")
md5sums=('SKIP')

package () {
  cd "$srcdir"
  install -Dm644 "srcdir/$pkgname/wireless.network" "$pkgdir/usr/share/wpa_tui/wireless.network"
  install -Dm644 "$srcdir/$pkgname/wired.network" "$pkgdir/usr/share/wp_tui/wired.network"
  install -Dm755 "$srcdir/$pkgname/wpa_tui" "$pkgdir/usr/bin/wpa_tui"
  
  install -Dm644 "$srcdir/$pkgname/wpa_supplicant-interface.conf" "$pkgdir/etc/wpa_supplicant/wpa_supplicant-interface.conf"
}
