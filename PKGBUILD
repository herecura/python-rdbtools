pkgname=python-rdbtools
pkgver=0.1.14
pkgrel=1
pkgdesc='tools for redis'
arch=('any')
url="https://github.com/sripathikrishnan/redis-rdb-tools"
license=('MIT')
depends=('python')
options=(!emptydirs)
source=("https://github.com/sripathikrishnan/redis-rdb-tools/archive/rdbtools-$pkgver.tar.gz")
sha512sums=('5de60bdcc1a3ce1c39e0267bd1f23909b25db8e8d90e53a119d94956b602e40ded361caa6a5da89fed9bb31cc9ee7662e6dc30207c0186f961e8f59e3cae7084')

package() {
  cd redis-rdb-tools-rdbtools-$pkgver
  python setup.py install --root="$pkgdir" --optimize=1
  install -D -m644 LICENSE "$pkgdir/usr/share/licenses/$pkgname/LICENSE"
}
