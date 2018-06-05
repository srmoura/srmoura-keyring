# Based on the file created for Arch Linux by:
# Gabriel Moura <g@srmoura.com.br>

pkgname=srmoura-keyring
pkgver=20180605
pkgrel=0
pkgdesc='SrMoura PGP keyring'
arch=('any')
url='http:/srmoura.com.br'
license=('GPL')
install="${pkgname}.install"
source=('Makefile'
        'srmoura.gpg'
        'srmoura-revoked'
        'srmoura-trusted')
sha512sums=(

#Makefile
            'ee2be8fcb6b4a3805b2012bb657b72c11d14043afcb0ff0224778766b5c3903bfe24dac0117060db0d2a82eac42b80d2936b2d33d9fc204096895d7e68df019d'

#srmoura.gpg
            '666ca8f031c8994a5c8b18837e8e8bbd822599fab871ea1e3ab1f99aba2555a199b3e6ffd997f78681b7fb01c3f610c85e7edf957b7caeefa5d7004e81ac06d9'

#srmoura-revoked
            'cf83e1357eefb8bdf1542850d66d8007d620e4050b5715dc83f4a921d36ce9ce47d0d13c5d85f2b0ff8318d2877eec2f63b931bd47417a81a538327af927da3e'

#srmoura-trusted
            '22d43d58f1f771097e50553b0aee531145155a18d72aa0c5bd4d228d4ebc7a53600278fbc20f0e326e0fb66844450cf159f554be10ab80ef093b98bd8d9b8019')

package() {
	cd "${srcdir}"
	make PREFIX=/usr DESTDIR=${pkgdir} install
}
