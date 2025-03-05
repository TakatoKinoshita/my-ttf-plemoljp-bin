# Maintainer: Shohei Maruyama <cheat.sc.linux@outlook.com>

pkgname=ttf-plemoljp-bin
pkgver=2.0.3
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
	'9a95404b4dea7adf77e3b487f41d6914e3de594cb38e3abd6547c587a18b6a6b'
	'cc1496750d14c0e113019b3da00e5f11a97f6de20a025ca69242a5127970a2ff'
	'6520a6b52d3943370683e13357ce8e54e7342bd29c7358497d6ec9ea8c8e9256'
	'52bbb5e729acc62435831d20641ece6a919e610100285ba183ef4d7233fb1e9a'
)

package() {
	find . -type f -name '*.ttf' -exec install -Dm644 {} -t "${pkgdir}/usr/share/fonts/PlemolJP" \;
	install -Dm644 LICENSE -t "${pkgdir}/usr/share/licenses/${pkgname}"
}
