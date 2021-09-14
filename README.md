# post-install

## Adding repositories:
```
sudo pacman -Syu artix-archlinux-support
```

``` bash
echo \
"# ARCH
[extra]
Include = /etc/pacman.d/mirrorlist-arch

[community]
Include = /etc/pacman.d/mirrorlist-arch 

[multilib]
Include = /etc/pacman.d/mirrorlist-arch

[universe]
Server = https://universe.artixlinux.org/$arch
Server = https://mirror1.artixlinux.org/universe/$arch
Server = https://mirror.pascalpuffke.de/artix-universe/$arch
Server = https://artixlinux.qontinuum.space:4443/universe/os/$arch

[omniverse]
Server = http://omniverse.artixlinux.org/$arch"\
 >> /etc/pacman.conf
 ```
 
 ## Adding badram address
 
 REBOOT
 
 ## Essential packages
 ```bash
 sudo pacman -Syu trizen
 trizen -S zsh deja-dup vscodium discord_arch_electron brave konsole dolphin libreoffice-fresh kate neovim wget keepassxc
 ```
 ``` bash
 curl -fsSL https://raw.githubusercontent.com/zimfw/install/master/install.zsh | zsh
 ```
 
 
