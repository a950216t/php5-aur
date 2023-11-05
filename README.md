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

makepkg -g >> PKGBUILD

makepkg -si

pacman -U "builded package name"
