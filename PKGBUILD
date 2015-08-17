# Contributor: Vinicius de Avila <vinicius.avila.jorge@gmail.com>
# Update Based on Geoff Teale's PKGBUILD. To support both python2 and python3

pkgname=python-all-odfpy
pkgver=0.9.4
pkgrel=2
pkgdesc="A complete API for OpenDocument in Python. Python 2.x and 3.x support"
arch=('i686' 'x86_64')
url="http://opendocumentfellowship.com/projects/odfpy"
license=('GPL')
depends=('python2' 'python')
conflicts=('odfpy' 'python2-odfpy' 'python3-odfpy')
provides=('python2-odfpy' 'python3-odfpy')
source=("http://pypi.python.org/packages/source/o/odfpy/odfpy-$pkgver.tar.gz")
md5sums=('f5adf8bb439e0c4624d2ef11c69a985b')

build() {
      cd "$srcdir/odfpy-${pkgver}"
      python2 setup.py install --root=${pkgdir}
      python3 setup.py install --root=${pkgdir}
}
