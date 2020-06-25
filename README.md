# phpbrew_sample
phpbrew installation command

## OSX
` brew install zlib bzip2 libiconv curl `
` shell
  phpbrew install 7.4.7 \
    +default \
    +mysql \
    +iconv="$(brew --prefix libiconv)" \
    +bz2="$(brew --prefix bzip2)" \
    +zlib="$(brew --prefix zlib)" \
    +fpm \
    +gd \
    +exif \
`
