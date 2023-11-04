# php5-aur
a php 5.6 arch linux aur repository

sudo pacman -S base-devel git

git clone --recursive https://aur.archlinux.org/c-client

cd c-client/

makepkg -g >> PKGBUILD

makepkg -si

cd ..

git clone --recursive https://github.com/a950216t/php5-aur

cd php5-aur/

sudo pacman -S --needed procps-ng acl libtool autoconf automake patchelf gawk sed bash python libxml2 pam krb5 zlib libedit smtp-forwarder pcre apache ncurses libxcrypt systemd systemd-libs coreutils findutils libxslt e2fsprogs openssl db5.3 postgresql-libs unixodbc libfbclient freetds sqlite libvpx gd tidy gmp libzip recode aspell enchant libvoikko hspell hunspell nuspell aspell icu curl net-snmp libsasl libldap pam libmcrypt

makepkg -g >> PKGBUILD

makepkg -si

pacman -U "builded package name"
