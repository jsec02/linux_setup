### setup_script

Automates post-installation environment replication across WSL, Raspberry Pi, and Kali Linux. Restores packages, dotfiles, databases, services, and configuration from Restic backups.

### Usage

This script assumes a user account is setup and logged in, as well as curl being installed.

```sh
bash <(curl -sSL https://raw.githubusercontent.com/jsec02/setup_script/master/linux_setup)
```

On WSL, no installer is run first so we manually create a user and configure sudo before running.

```sh
pacman -Sy sudo
useradd -m -G wheel master
passwd master
sed -i 's/^# %wheel ALL=(ALL:ALL) ALL/%wheel ALL=(ALL:ALL) ALL/' /etc/sudoers
su master
cd $HOME
bash <(curl -sSL https://raw.githubusercontent.com/jsec02/setup_script/master/linux_setup)
```

<!-- CODE_STATISTICS_START -->

### Code Statistics

```
--------------------------------------------------------------------------------
Language                      files          blank        comment           code
--------------------------------------------------------------------------------
Bourne Again Shell                1             90             24            374
Markdown                          1             13              4             35
--------------------------------------------------------------------------------
SUM:                              2            103             28            409
--------------------------------------------------------------------------------
```
<!-- CODE_STATISTICS_END -->

<!-- PROJECT_STRUCTURE_START -->

### Project Structure

```
setup_script
├── README.md
└── setup

1 directory, 2 files
```
<!-- PROJECT_STRUCTURE_END -->
