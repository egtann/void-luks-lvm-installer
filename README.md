Voidlinux LUKS + LVM installer
------------------------------

Basic install script that replaces completely the standard VoidLinux installer.  

### Features

- Full Disk Encryption for both `boot` and `root` partitions
- Detects UEFI mode and creates partitions accordingly
- Set options from a config file
- Let's you define your LVs from config file
- Supports execution of custom scripts inside install chroot for easy customization
- Optionally add swap

### Usage

- Boot a VoidLinux LiveCD
- Setup your network
- Install wget and unzip

Then:

```
wget https://github.com/egtann/void-luks-lvm-installer/archive/master.zip
unzip master.zip
cd void-luks-lvm-installer
```
Edit `config` to your taste.  
If needed put your `.sh` scripts in custom dir - see examples - before running `install.sh`  
```
./install.sh
```
