# Maintainer: Shohei Maruyama <cheat.sc.linux@outlook.com>

pkgname=ttf-plemoljp-bin
pkgver=2.0.2
pkgrel=1
pkgdesc='Plex Mono Language JP'
arch=('any')
url='https://github.com/yuru7/PlemolJP'
license=('custom:OFL')
provides=('ttf-font')
makedepends=()
conflicts=('ttf-plemoljp')
source=(
	"PlemolJP_v${pkgver}.zip::https://github.com/yuru7/PlemolJP/releases/download/v${pkgver}/PlemolJP_v${pkgver}.zip"
	"PlemolJP_NF_v${pkgver}.zip::https://github.com/yuru7/PlemolJP/releases/download/v${pkgver}/PlemolJP_NF_v${pkgver}.zip"
	"PlemolJP_HS_v${pkgver}.zip::https://github.com/yuru7/PlemolJP/releases/download/v${pkgver}/PlemolJP_HS_v${pkgver}.zip"
	"LICENSE::https://github.com/yuru7/PlemolJP/raw/v${pkgver}/LICENSE"
)
sha256sums=(
	'a1767a4e527a0a2e9b143acbe2074aace98c9985cb21cb84801fed4a7ce7599f'
	'9f41c4928f1f18b996fd998af9c474bc521703c3a83c01ec0fc014cc1d9640f7'
	'1f309e1247609d116f5cbc2ed01b1a269b4642105798f6507fa4e09a1844483d'
	'52bbb5e729acc62435831d20641ece6a919e610100285ba183ef4d7233fb1e9a'
)

package() {
	find . -type f -name '*.ttf' -exec install -Dm644 {} -t "${pkgdir}/usr/share/fonts/PlemolJP" \;
	install -Dm644 LICENSE -t "${pkgdir}/usr/share/licenses/${pkgname}"
}
