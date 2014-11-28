## Arch Linux 安装指南

archlinux 用户下载 PKGBUILD 文件夹，进入目录在终端下 makepkg 生成安装包，生成后终端下：pacman -U 这个包就可以安装了！

-----

## Debian 安装指南

Debian 及基于 Debian 的发行版 (如ubuntu, linuxmint) 请直接下载 mvgather-x.x.x.deb , 然后双击 deb 包就能安装了;

有些用户并没有安装 apt 包管理器的 GUI 界面, 也可以在终端里面安装:

```
$ sudo dpkg -i mvgather-x.x.x.deb
$ sudo apt-get -f install
```

-----

## Fedora 安装指南

mvgather rpm 包由 @1dot75cm 维护, 目前支持 el7, fc19, fc20, fc21, fc22。

fc19, fc20, fc21, fc22 执行以下命令进行安装:

```
# yum install dnf-plugins-core http://download1.rpmfusion.org/free/fedora/rpmfusion-free-release-$(rpm -E %fedora).noarch.rpm http://download1.rpmfusion.org/nonfree/fedora/rpmfusion-nonfree-release-$(rpm -E %fedora).noarch.rpm
# dnf copr enable mosquito/myrepo
# dnf copr enable mosquito/myrepo-testing
# dnf install mvgather
```

更多其他软件，请访问 [myrepo](https://copr.fedoraproject.org/coprs/mosquito/myrepo) 。

-----

## RHEL 7 安装指南

el7 执行以下命令安装:

```
# yum-config-manager --add-repo=https://copr.fedoraproject.org/coprs/mosquito/myrepo/repo/epel-$(rpm -E %?rhel)/mosquito-myrepo-epel-$(rpm -E %?rhel).repo
# yum-config-manager --add-repo=https://copr.fedoraproject.org/coprs/mosquito/myrepo-testing/repo/epel-$(rpm -E %?rhel)/mosquito-myrepo-testing-epel-$(rpm -E %?rhel).repo
# yum install epel-release http://li.nux.ro/download/nux/dextop/el$(rpm -E %rhel)/x86_64/nux-dextop-release-0-2.el$(rpm -E %rhel).nux.noarch.rpm
# yum install mvgather
```

更多其他软件，请访问 [myrepo](https://copr.fedoraproject.org/coprs/mosquito/myrepo) 。
