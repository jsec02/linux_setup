### setup_script

Automates post-installation environment replication across WSL, Raspberry Pi, and Kali Linux. Restores packages, dotfiles, databases, services, and configuration from Restic backups.

### Usage

This script assumes a user account is setup and logged in, as well as curl being installed.

```sh
bash <(curl -sSL https://raw.githubusercontent.com/jb49088/setup_script/master/setup)
```

<!-- CODE_STATISTICS_START -->

### Code Statistics

```
--------------------------------------------------------------------------------
Language                      files          blank        comment           code
--------------------------------------------------------------------------------
Bourne Again Shell                1             72             19            322
Markdown                          1             11              4             25
--------------------------------------------------------------------------------
SUM:                              2             83             23            347
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
