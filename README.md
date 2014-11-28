Arch Linux 安装指南

archlinux用户下载PKGBUILD文件夹，然后进入目录在终端下makepkg生成安装包，生成后终端下：pacman -U 这个包就可以安装了！
Debian 安装指南

Debian及基于Debian的发行版(比如ubuntu, linuxmint)请直接下载 mvgather-x.x.x.deb这个包, 然后双击deb包就能安装了;

有些用户并没有安装apt包管理器的GUI界面, 也可以在终端里面安装:

$ sudo dpkg -i mvgather-x.x.x.deb
$ sudo apt-get -f install
