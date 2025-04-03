# soyraiz1 Distrolabs
Distrolabs is a sub-project/brand of soyraiz1 and Icycoide. This is made specifically to serve projects related to OS development et cetera.

- [TyrianOS](#get-tyrianos)
- [XBRS](#get-xbrs-recovery)
- [TylkoLinux](#get-tylkolinux)
- [ElemintOS](#get-elemintos)

## Get TyrianOS
[Repository (GitHub)](https://github.com/Icycoide/TyrianOS/blob/main/README.md)
### 1. Rebase to the unsigned variant of the image
```bash
rpm-ostree rebase ostree-unverified-registry:ghcr.io/icycoide/tyrianos:latest
```
Reboot:
```
systemctl reboot
```
### 2. Rebase to the signed variant of the image you chose
```bash
rpm-ostree rebase ostree-image-signed:docker://ghcr.io/icycoide/tyrianos:latest
```
Reboot:
```
systemctl reboot
```
### 3. Nvidia GPU Configuration (Nvidia-only)
Run this ujust command to setup the required kernel arguments:
```
ujust configure-nvidia
```
Reboot:
```
systemctl reboot
```
### Optimus laptops only
For Optimus laptops, run this command:
```
ujust configure-nvidia-optimus
```
Reboot:
```
systemctl reboot
```
This configures Optimus laptops.

## Get XBRS Recovery
### [↓ Download](https://repo.rootsource.cc/iso/XBRS/OPW-v9/ingyteXBRSv0.1.iso)
<small>MD5 Hash: `9cc42f437700a9e9e76cf90e81b8ff61  ingyteXBRSv0.1.iso`</small>
## Get TylkoLinux
```bash
git clone https://github.com/kevadesu/TylkoLinux
git checkout delirium
```
[Follow the guide here](https://rootsource.cc/Articles/tylkolinux-installation/)

[Source code for scripts](https://github.com/distrolabs/TylkoLinux)

## Get ElemintOS
[Click here to be redirected](https://icycoide.github.io/ElemintOS)


-----


That's it...maybe check out our other websites?

[Icycoide](https://icycoide.github.io) - [RootSourceCC](https://rootsource.cc) - [soyraiz1](https://raiz1.noho.st)
