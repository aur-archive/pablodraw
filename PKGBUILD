pkgname=pablodraw
pkgver=3.2.1
pkgrel=1
pkgdesc='An Ansi/Ascii text and RIPscrip vector graphic art editor/viewer with multi-user capabilities'
arch=('any')
url='http://picoe.ca/products/pablodraw/'
license=('unknown')
depends=('mono>=2.8' 'gtk-sharp-2')

source=("http://download.picoe.ca/pablodraw/3.2/PabloDraw-$pkgver.zip"
        'pablodraw'
        'pablodraw.desktop')

package() {
  cd "$srcdir"

  install -dm755 "$pkgdir"/usr/bin

  install -Dm755 pablodraw "$pkgdir"/usr/bin/pablodraw
  install -Dm755 PabloDraw.exe "$pkgdir"/usr/share/pablodraw/PabloDraw.exe
  install -Dm644 pablodraw.desktop "$pkgdir"/usr/share/applications/pablodraw.desktop
}

md5sums=('628df8bb1db90034f67c59937aa071d8'
         'e6abdd467db9436e1fc257733653c82b'
         '169c72b2d56a86524c1bd260b3eda0a1')
