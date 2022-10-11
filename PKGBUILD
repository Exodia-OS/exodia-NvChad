#
# Maintainer: Mahmoud Mohamed (Ozil) <mmsaeed509@gmail.com> , <https://github.com/mmsaeed509>
#
# Developer : siduck76 <https://github.com/siduck76>
#

pkgname=exodia-NvChad
pkgver=1.0
pkgrel=6
pkgdesc="NvChad : the ultimate neovim configuration"
arch=('any')
url='https://github.com/NvChad/NvChad'
license=('GPL')
depends=(

	'neovim'
	'lua'
	'ripgrep'

)
makedepends=('git')
optdepends=()
groups=(

	'exodia-os-skeleton'
	'exodia-text-editors'

)

source=(

	'nvim-config.tar.gz'
	'nvim-plugins.tar.gz'

)

sha256sums=(

	'ec5ab25e66ddeadb0742eb6af6f213a73e9b36fd07c526c1708c4a844ae41d2c'
    'a0f71e2d3f3ac554fc49c5c8144b43203347466de22647f4cf1224b0a70df170'

)

package() {

	mkdir -p ${pkgdir}/etc/skel/.config
	mkdir -p ${pkgdir}/etc/skel/.local/share/nvim

	cp -rf ${srcdir}/nvim ${pkgdir}/etc/skel/.config/nvim
	cp -rf ${srcdir}/nvim-plugins/* ${pkgdir}/etc/skel/.local/share/nvim

}
