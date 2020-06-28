pkgname=python-rdbtools
pkgver=0.1.15
pkgrel=1
pkgdesc='tools for redis'
arch=('any')
url="https://github.com/sripathikrishnan/redis-rdb-tools"
license=('MIT')
depends=('python')
options=(!emptydirs)
source=("https://github.com/sripathikrishnan/redis-rdb-tools/archive/rdbtools-$pkgver.tar.gz")
sha512sums=('226f94730de62e0fdc98f58936d4ccfd84cfcc9c0995dc16e3842cf8a52d75e9174a0da430c26cf98320edec67318cf6fbc805f8f61667bde074c109f173ef3b')

package() {
  cd redis-rdb-tools-rdbtools-$pkgver
  python setup.py install --root="$pkgdir" --optimize=1
  install -D -m644 LICENSE "$pkgdir/usr/share/licenses/$pkgname/LICENSE"
}
