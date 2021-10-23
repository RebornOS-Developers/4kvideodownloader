# Maintainer: Rafael <rafael@rebornos.org>
# v:4.18.2.4520

pkgname=4kvideodownloader
pkgver=4.18.2
pkgrel=1
pkgdesc="Enjoy videos anywhere, anytime regardless of whether you are offline."
arch=('any')
url="https://dl.4kdownload.com/app"
license=('Custom')
makedepends=('make')
provides=(${pkgname})
conflicts=(${pkgname})
source=(${url}/${pkgname}_${pkgver}-${pkgrel}_amd64.deb)
sha512sums=('499c6deee470684ffa98fb54adf58020123ef111c7bc44cc88cf3a97c60c605b872e055a15cfe60a25dc9f9f392924f95ec0b8363ae97c641bdffc8231523e59')

package() {
           mkdir -p ${pkgdir}/usr/bin
           tar -xvf ${srcdir}/data.tar.xz
           cp -r ${srcdir}/usr/* ${pkgdir}/usr/
           cp ${pkgdir}/usr/lib/${pkgname}/${pkgname}.sh ${pkgdir}/usr/bin/${pkgname}
}

