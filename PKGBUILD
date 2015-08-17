# Maintainer: James Bulmer <nekinie@gmail.com>

pkgname='python2-pycadf-deb'
pkgver=0.2
pkgrel=1
pkgdesc='Python implementation of DMTF Cloud Audit (CADF) data model'
arch=('i686' 'x86_64')
url='http://packages.ubuntu.com/trusty/all/python-pycadf'
license=('Apache')

depends=(
  'python2'
  'python2-netaddr'
  'python2-six'
  'python2-iso8601'
  'python2-oslo-config'
  'python2-oslo-messaging-deb'
  'python2-babel'
  'python2-pytz'
  'python2-webob'
)

source=('http://archive.ubuntu.com/ubuntu/pool/main/p/python-pycadf/python-pycadf_0.2-1build1_all.deb')
md5sums=('e6dcdcbc594d189dab41a00ced2409aa')

package() {
  cd ${srcdir}
  tar -xJf ${startdir}/src/data.tar.xz
  mv ${srcdir}/usr/lib/python2.7/dist-packages/ ${srcdir}/usr/lib/python2.7/site-packages/
  cp -r ${srcdir}/usr/ ${pkgdir}
  cp -r ${srcdir}/etc/ ${pkgdir}
}