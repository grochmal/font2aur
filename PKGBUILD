pkgname=random-font-collection
pkgver=1.1
pkgrel=1
pkgdesc="My favourite (mostly) open source fonts"
arch=(any)
url="https://github.com/grochmal/font2aur"
license=('APACHE'
         'OFL')
depends=(fontconfig xorg-font-utils)
source=('AmaticSC-Bold.ttf'
        'AmaticSC-Regular.ttf'
        'Augie.ttf'
        'GreatVibes.ttf'
        'HomemadeApple.ttf'
        'NovaMono.ttf'
        'PermanentMarker.ttf'
        'RockSalt.ttf'
        'Starcraft.ttf'
        'Tangerine-Bold.ttf'
        'Tangerine-Regular.ttf')
sha1sums=('fcdeb8beb050eeb17b8fb422b55337ac7c6c0e0c'
          'd40486af52c983f5b1ad3eb66b523081c1f43a88'
          '997153bde1656c1099207c390234b399e0bd5bbe'
          '9f33c7ff09497f02b1631e572305fd412821c624'
          'f70eebf7d904ded8ea79117e566a4ad60c5b8c0d'
          'dfd7d60609fcd7c6d7a7b372d2ec1f91b3cab650'
          '35ba32900c9b7f6114ce074799e0c482e1cb2cab'
          'af6a5148c0cccede730822ab7ddbd2dcb3c94687'
          '246bfcbb178628dd2f0268f5ac9f9dec1e6424c9'
          '6da2d73fd60203178d6c2ca76d490c385dc823a1'
          '6ca88897f69c3787e8517cdee220f73cb1bf71c2')
install=$pkgname.install

package() {
  for font in ${source[@]}; do
    echo will install $font  # makepkg debug
    install -Dm644 $font "$pkgdir/usr/share/fonts/TTF/$font"
  done
}

