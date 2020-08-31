# phpbrew_sample
phpbrew installation command

## OSX
- **php7.4**
```shell
brew install zlib bzip2 libiconv curl
phpbrew install 7.4.7 \
    +default \
    +mysql \
    +iconv="$(brew --prefix libiconv)" \
    +bz2="$(brew --prefix bzip2)" \
    +zlib="$(brew --prefix zlib)" \
    +fpm \
    +gd \
    +exif
```
- **php5.6**
```shell
phpbrew ext install https://github.com/php-memcached-dev/php-memcached 2.2.0 -- --disable-memcached-sasl --with-zlib-dir="$(brew --prefix zlib)"
```
