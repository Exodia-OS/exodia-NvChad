#
# Maintainer: Mahmoud Mohamed (Ozil) <mmsaeed509@gmail.com> , <https://github.com/mmsaeed509>
#
# Developer : siduck76 <https://github.com/siduck76>
#

pkgname=exodia-NvChad
pkgver=1.0
pkgrel=7
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
	'Exodia-TUI-Apps'

)

prepare() {

	cp -af ../nvim-config ${srcdir}
	cp -af ../nvim-plugins ${srcdir}

}

package() {

	CONFIG_DIR=${pkgdir}/etc/skel/.config/nvim
	PLUGINS_DIR=${pkgdir}/etc/skel/.local/share/nvim
	mkdir -p $CONFIG_DIR $PLUGINS_DIR

	cp -rf ${srcdir}/nvim-config/*  $CONFIG_DIR
	cp -rf ${srcdir}/nvim-plugins/* $PLUGINS_DIR

}
