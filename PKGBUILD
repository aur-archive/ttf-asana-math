# Maintainer: GordonGR <gordongr@freemail.gr>
pkgname=ttf-asana-math
pkgver=000.954
pkgrel=1
license=('Custom: OFL')
depends=('fontconfig' 'xorg-font-utils')
pkgdesc="A font to typeset maths in Xe(La)TeX and Lua(La)TeX by Apostolos Syropoulos"
arch=('any')
url="http://www.ctan.org/pkg/asana-math"
source=("ftp://ftp.rrzn.uni-hannover.de/pub/mirror/tex-archive/fonts/Asana-Math/Asana-Math.ttf" 
"http://scripts.sil.org/cms/scripts/render_download.php?&format=file&media_id=OFL_plaintext&filename=OFL.txt")
md5sums=('acc1721727c225b31aa0b9857b6ccd76'
         '6ed93967ff0dc6dd9c8d31c17f817a06')
install=$pkgname.install

package()
{
mkdir -p $pkgdir/usr/share/fonts/TTF
cp *.ttf $pkgdir/usr/share/fonts/TTF
mkdir -p $pkgdir/usr/share/licenses/custom/ttf-asana-math/
mv 'render_download.php?&format=file&media_id=OFL_plaintext&filename=OFL.txt' LICENSE
cp LICENSE $pkgdir/usr/share/licenses/custom/ttf-asana-math/
}
