# Maintainer: Your Name <youremail@domain.com>
pkgname=devtunnel-cli
pkgver='8c6af52'
pkgrel=1
epoch=
pkgdesc="Microsoft's Dev tunnel - CLI"
arch=('x86_64')
url="https://github.com/EnityBlackHawk/devtunnel-cli.git"
license=('MIT')
depends=('libsecret')
makedepends=('git')
source=('devtunnel-cli::git://github.com/EnityBlackHawk/devtunnel-cli.git')
md5sums=('SKIP')

pkver(){
	cd "$pkgname"
	printf "%s" "$(git rev-parse --short HEAD)"
}


build() {
	cd "$pkgname"
	./devtunnel.sh
}

package() {
	cd "$pkgname"
	sudo cp ~/bin/devtunnel /usr/local/bin
	sudo chmod 775 /usr/local/bin/devtunnel
	rm ~/bin/devtunnel
}
