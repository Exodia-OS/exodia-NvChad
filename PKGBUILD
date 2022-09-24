#
# Maintainer: Mahmoud Mohamed (Ozil) <mmsaeed509@gmail.com> , <https://github.com/mmsaeed509>
#
# Developer : siduck76 <https://github.com/siduck76>
#

pkgname=exodia-NvChad
pkgver=1.0
pkgrel=4
pkgdesc="NvChad : the ultimate neovim configuration"
arch=('any')
url='https://github.com/NvChad/NvChad'
license=('GPL')
depends=('neovim' 'lua'
		 'ripgrep:  required for grep searching with Telescope')
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
	'60de4f04fb6fcf3478e0769d5d21fcc064a1eb287fa2f8334ef5496abfd62d94'
    '46a6b315e700ab2f3b13b35e6b547dcf410dd9e00640132fef9726a32a1011d1'
)

package() {
	mkdir -p ${pkgdir}/etc/skel/.config
	mkdir -p ${pkgdir}/etc/skel/.local/share/nvim

	cp -rf ${srcdir}/nvim ${pkgdir}/etc/skel/.config/nvim
	cp -rf ${srcdir}/nvim-plugins/* ${pkgdir}/etc/skel/.local/share/nvim
}
