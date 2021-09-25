# Maintainer: Rafael <rafael@rebornos.org>
# v:4.18.1.4500

pkgname=4kvideodownloader
pkgver=4.18.1
pkgrel=1
pkgdesc="Enjoy videos anywhere, anytime regardless of whether you are offline."
arch=('any')
url="https://dl.4kdownload.com/app"
license=('Custom')
makedepends=('make')
provides=(${pkgname})
conflicts=(${pkgname})
source=(${url}/${pkgname}_${pkgver}-${pkgrel}_amd64.deb)
sha512sums=('6eac5f37358e2ef068882bf250440a9e75c9f8ae903d510ca314f56449bb180b3575d07f594f1871ad4b97261af348724b6f3a7d2d500dcfb522f1c35d351374')

package() {
           mkdir -p ${pkgdir}/usr/bin
           tar -xvf ${srcdir}/data.tar.xz
           cp -r ${srcdir}/usr/* ${pkgdir}/usr/
           cp ${pkgdir}/usr/lib/${pkgname}/${pkgname}.sh ${pkgdir}/usr/bin/${pkgname}
}

