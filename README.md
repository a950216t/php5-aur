# php5-aur
a php 5.6 arch linux aur repository

pacman -S base-devel

git clone --recursive https://github.com/a950216t/php5-aur

cd php5-aur/

gpg --recv-keys --keyserver pgp.mit.edu C2BF0BC433CFC8B3

makepkg -g >> PKGBUILD

makepkg -si

pacman -U "builded package name"
