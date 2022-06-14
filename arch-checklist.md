## Preinstall

- wifi
- fdisk
- luks
- lvm
- pacman: enable parallel

## Install

- packages
```lang bash
pacstrap /mnt linux linux-firmware base base-dev networkmanager pipewire pipewire-pulse pipewire-alsa pipewire-jack wireplumber
phonon-qt5-vlc plasma dolphin ark kitty okular spectacle audacious gwenview htop vim neovim bluedevil keepassxc
kate xf86-video-intel intel-ucode lvm2 kvantum zsh zsh-completions
```

## PostInstall

- efibootmgr
- fstab

## Chroot

- timezone
- locales
- generate locales
- set LANG
- configure pacman (paralel, multilib)
- systemctl enable --user pipewire wireplumber
- systemctl enable NetworkManager bluetooth sddm
- configure initramfs
- 

