packer-archlinux
===

These are [Packer](https://www.packer.io/) VirtualBox templates for building ArchLinux for x32 and x64 systems.

These are based on [@kaorimatz](https://github.com/kaorimatz/packer-templates) work with some stuff that I didn't need stripped out. This has only VirtualBox builder.

## Dependencies

Download and install [VirtualBox](https://www.virtualbox.org/) and [Packer](https://www.packer.io/)

i.e. Mac 

```brew install packer```

## Build 

```
git clone https://github.com/karolistamutis/packer-archlinux

cd packer-archlinux

packer build archlinux{32,64}.json
```

## Use

```
vagrant box add archbox32 archlinux32.box
vagrant init archbox32
vagrant up
vagrant status
vagrant ssh
....
vagrant destroy
```