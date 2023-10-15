# Maintainer: Bouteiller a2n Alan <a2n.dev@pm.me>

pkgname=dracut-numlock
pkgver=1.0.0
pkgrel=1
pkgdesc="A dracut module which enables numlock in the early boot"
arch=('any')
url="https://github.com/bouteillerAlan/dracut-numlock/tree/v1.0.0"
license=('MIT')
source=("https://github.com/bouteillerAlan/${pkgname}/archive/refs/tags/v${pkgver}.tar.gz")
sha256sums=('3c25ea9ae560a71655b422b8f343c0865dcae1564a20c2824295f6b7a5d2587d')

package() {
  cd "${pkgname}-${pkgver}"
  install -Dm 644 50numlock/module-setup.sh "${pkgdir}"/usr/lib/dracut/modules.d/50numlock/module-setup.sh
  install -Dm 644 50numlock/numlock.sh "${pkgdir}"/usr/lib/dracut/modules.d/50numlock/numlock.sh
}

