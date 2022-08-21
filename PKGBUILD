#
# Maintainer: Mahmoud Mohamed (Ozil) <mmsaeed509@gmail.com> , <https://github.com/mmsaeed509>
#
# Developer : siduck76 <https://github.com/siduck76>
#

pkgname=exodia-NvChad
pkgver=1.0
pkgrel=1
pkgdesc="NvChad : the ultimate neovim configuration"
arch=('any')
url='https://github.com/NvChad/NvChad'
license=('GPL')
depends=('neovim')
makedepends=('git')
optdepends=()

source=('nvim-config.tar.gz' 'nvim-plugins.tar.gz')

sha256sums=('f6854b7ee402dc425c7deb444c472db9eff9c4b18d401ecebf8b9ce7419fcbee'
            'b8d5422fb51d53f0f7eef90be18d16e5f3c3ee258551dc2798e071dd3b396a20')

package() {
	mkdir -p ${pkgdir}/etc/skel/.config
	mkdir -p ${pkgdir}/etc/skel/.local/share/nvim

	cp -rf ${srcdir}/nvim ${pkgdir}/etc/skel/.config/nvim
	cp -rf ${srcdir}/nvim-plugins/* ${pkgdir}/etc/skel/.local/share/nvim
}
