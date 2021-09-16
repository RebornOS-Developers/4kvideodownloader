# Maintainer: Rafael <rafael@rebornos.org>
# v:4.18.0.4480

pkgname=4kvideodownloader
pkgver=4.18.0
pkgrel=1
pkgdesc="Enjoy videos anywhere, anytime regardless of whether you are offline."
arch=('any')
url="https://dl.4kdownload.com/app"
license=('Custom')
makedepends=('make')
provides=(${pkgname})
conflicts=(${pkgname})
source=(${url}/${pkgname}_${pkgver}-${pkgrel}_amd64.deb)
sha512sums=('a6808feee5803d697774d942d545ab585593d1c5ba1cae64831b8757c41ba42b0052a2c9f95e047e0d52f7c2422cec9931def855d736b9467e665031840d2d72')

package() {
           mkdir -p ${pkgdir}/usr/bin
           tar -xvf ${srcdir}/data.tar.xz
           cp -r ${srcdir}/usr/* ${pkgdir}/usr/
           cp ${pkgdir}/usr/lib/${pkgname}/${pkgname}.sh ${pkgdir}/usr/bin/${pkgname}
}

