# Contributor: MeMi69 <lumpilou@gmail.com>
pkgname=mpd-add-similar  
pkgver=0.1.6
pkgrel=3
pkgdesc="Adds similar tracks to your MPD playlist"
arch=('i686' 'x86_64')
url="https://launchpad.net/mpd-add-similar"
license=('GPL')
depends=('mpd' 'python2-mpd' 'python2' 'python2-pylast')
source=("http://launchpad.net/mpd-add-similar/trunk/0.1.6/+download/mpd-add-similar-0.1.6.tar.gz")
md5sums=('decde5ac36381fd87e30e2a73f578d8c')

build() {
  cd $srcdir/$pkgname-$pkgver

}
package() {
  cd $pkgname-$pkgver
  #make DESTDIR="$pkgdir" install
  python2 setup.py install --root=$pkgdir || return 1
}
# vim:syntax=sh
