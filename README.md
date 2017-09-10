# packer

## Preconditon
- Install packer (using Homebrew etc).
- [VBoxGuestAdditions.iso] is located on the current directory(centos7).

[VBoxGuestAdditions.iso]: http://download.virtualbox.org/virtualbox/5.1.0_RC1/

## Directory Configuration
    centos7
    ├── VBoxGuestAdditions.iso
    ├── http
    │   └── ks.cfg
    ├── scripts
    │   ├── VBoxGuestAdditions.sh
    │   ├── clean.sh
    │   ├── os.sh
    │   └── vagrant.sh
    └── virtualbox.json

## Execute Commands
1. `packer build -only=virtualbox-iso virtualbox.json`
 - Output: **CentOS-7-x86_64-Minimal-1611.box.**


