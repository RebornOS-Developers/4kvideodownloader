# Maintainer: Rafael <rafael@rebornos.org>
# v:4.18.3.4530

pkgname=4kvideodownloader
pkgver=4.18.3
pkgrel=1
pkgdesc="Enjoy videos anywhere, anytime regardless of whether you are offline."
arch=('any')
url="https://dl.4kdownload.com/app"
license=('Custom')
makedepends=('make')
provides=(${pkgname})
conflicts=(${pkgname})
source=(${url}/${pkgname}_${pkgver}-${pkgrel}_amd64.deb)
sha512sums=('4fd235db07c56748fee8b8a4117baa6469356dd59e55fa3e91a5cab46ef4ca69b1680532345538e9bffcb6130c96622f41f31ed2634012f5dcd44f4f718c88cd')

package() {
           mkdir -p ${pkgdir}/usr/bin
           tar -xvf ${srcdir}/data.tar.xz
           cp -r ${srcdir}/usr/* ${pkgdir}/usr/
           cp ${pkgdir}/usr/lib/${pkgname}/${pkgname}.sh ${pkgdir}/usr/bin/${pkgname}
}

