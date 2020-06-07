# Maintainer: Stefano Capitani <stefanoatmanjarodotorg>
# Maintainer: excalibur1234 @forum.manjaro.org


pkgname=pacui
pkgver=1.14
pkgrel=1
pkgdesc="Bash script providing advanced Pacman and Yay/Pikaur/Aurman/Pakku/Trizen/Pacaur functionality in a simple UI"
arch=(any)
url="https://github.com/excalibur1234/$pkgname"
license=('GPL3')
depends=('pacman-contrib' 'expac' 'sudo' 'fzf')


conflicts=("$pkgname-git")
optdepends=('yay: One AUR helper is needed for AUR support.'
            'pikaur: One AUR helper is needed for AUR support.'
            'aurman: One AUR helper is needed for AUR support.'
            'pakku: One AUR helper is needed for AUR support.'
            'trizen: One AUR helper is needed for AUR support.'
            'pacaur: One AUR helper is needed for AUR support.'
            'pamac-cli: One AUR helper is needed for AUR support.'
            'pacman-mirrors: Needed for Manjaro mirror support'
            'reflector: Needed for Arch Linux mirror support'
            'downgrade: Needed for hidden "downgrade" option.')
source=("$url/archive/$pkgver.tar.gz")
md5sums=('39b177c3ef15601e55b929af10eeaf77')

# how to update md5sum:
#  1. do "updpkgsums" inside the folder with PKGBUILD file
#  2. delete .tar.gz file


package () {
            install -Dm755 "$srcdir/$pkgname-$pkgver/pacui" "$pkgdir/usr/bin/pacui"
}
