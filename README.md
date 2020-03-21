# Dotfiles
This is the repo containing all my config as well as the steps I took to create this installation.

## Manually Installed

| Package | Reason |
| --- | --- |
| firefox | Web Browser |
| pamixer | Pulseaudio CLI Manager, Required by headset |
| pulseaudio | Prefered Audio interface |
| pavucontrol | Pulseaudio GUI Manager |
| gvim | Vim but I can use xclip |
| discord | Discord voice chat |
| steam | ಠ_ಠ |
| wine | For running windows stuff |
| wine-gecko | For running windows stuff |
| wine-mono | For running windows stuff |
| lutris | Wine wrapper manager/game launcher |
| code | VSCode |
| noto-fonts-cjk | Googles Asian fonts |
| noto-fonts | Googles Noto fonts |
| noto-fonts-emoji | Googles Emoji font |
| nvidia-440xx-utils | GTX 1070 Drivers |
| linux419-nvidia-440xx | GTX 1070 Drivers |
| lib32-nvidia-440xx-utils | GTX 1070 Drivers |
| vulkan-icd-loader | Vulkan Drivers |
| lib32-vulkan-icd-loader | Vulkan Drivers |
| xfce4 | XFCE DE |
| xfce4-goodies | XFCE Extras |
| demnu | Dmenu App launcher |
```
pacman -Syu firefox pamixer pulseaudio pavucontrol gvim discord steam wine wine-gecko wine-mono lutris code noto-fonts-cjk noto-fonts noto-fonts-emoji nvidia-440xx-utils linux419-nvidia-440x lib32-nvidia-440xx-utils vulkan-icd-loader lib32-vulkan-icd-loader xfce4-goodies xfce4 dmenu
```

## Manual config
### Nvidia Config
`sudo mhwd --install pci video-nvidia-440xx`  
`sudo nvidia-settings` **Force Full Composition Pipeline** for all displays

### Things to fix

- [X] Headset
- Required `pulseaudio` & `pamixer`
- [X] Grub Boot
- BIOS could only detect one UEFI boot. Had to edit BIOS Settings
- [X] Copy paste from Browser to vim 
- Needed to install `gvim` to allow xclip access
- [X] Storage drive not mounted
- Needed to add entry to `/etc/fstab`
- [ ] Windows dont snap

### Things to customise
- [ ] Notifications are too big
- [ ] Default Polybar is gross
- [ ] Application launcher/bar is gross
- [X] Conky 🤮
