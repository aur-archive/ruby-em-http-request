# Generated by gem2arch (https://github.com/anatol/gem2arch)
# Maintainer: Anatol Pomozov <anatol.pomozov@gmail.com>
# Contributor: eagletmt <eagletmt@gmail.com>

_gemname=em-http-request
pkgname=ruby-$_gemname
pkgver=1.1.2
pkgrel=1
pkgdesc='EventMachine based, async HTTP Request client'
arch=(any)
url='https://github.com/igrigorik/em-http-request'
license=(MIT)
depends=(ruby ruby-addressable ruby-cookiejar ruby-em-socksify ruby-eventmachine ruby-http_parser.rb)
options=(!emptydirs)
source=(https://rubygems.org/downloads/$_gemname-$pkgver.gem)
noextract=($_gemname-$pkgver.gem)
sha1sums=('826562ec11f703fb9ba959446a6881f3e9186d57')

package() {
  local _gemdir="$(ruby -e'puts Gem.default_dir')"
  gem install --ignore-dependencies --no-user-install -i "$pkgdir/$_gemdir" -n "$pkgdir/usr/bin" $_gemname-$pkgver.gem
  rm "$pkgdir/$_gemdir/cache/$_gemname-$pkgver.gem"
}
