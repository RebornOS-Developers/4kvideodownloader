# Maintainer: Rafael <rafael@rebornos.org>
# v: 4.17.2.4460

pkgname=4kvideodownloader
pkgver=4.17.2
pkgrel=1
pkgdesc="Enjoy videos anywhere, anytime regardless of whether you are offline."
arch=('any')
url="https://dl.4kdownload.com/app"
license=('Custom')
makedepends=('make')
provides=(${pkgname})
conflicts=(${pkgname})
source=(${url}/${pkgname}_${pkgver}-${pkgrel}_amd64.deb)
sha512sums=('cd21e005988a00894459b12f46cc5b56601da3db851ef85934fee7d19d385d7cd660117142c8b2cc563662b090b11b2e28d876bac8e23ca580f4471b6a6d65ae')

package() {
           mkdir -p ${pkgdir}/usr/bin
           tar -xvf ${srcdir}/data.tar.xz
           cp -r ${srcdir}/usr/* ${pkgdir}/usr/
           cp ${pkgdir}/usr/lib/${pkgname}/${pkgname}.sh ${pkgdir}/usr/bin/${pkgname}
}

