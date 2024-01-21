<img src=https://github.com/T13nou/Archible/blob/main/images/t13nou_Arch_Linux_Terraforming_Ansible_with_text_Archible_930879c2-0545-4c05-9996-286f5f4f803d.png width="1000" height="100">

# Archible

This Ansible script is designed to automate the customization of a freshly installed EndeavourOS distribution, streamlining the setup process for users. The script is organized into various roles, each responsible for specific aspects of system configuration and software installation. By executing this script, users can effortlessly apply a set of predefined configurations and install a curated collection of software tailored to enhance the EndeavourOS experience.

Feel free to clone this repository and tweak playbook to your needs :)

The following command installs ansible, clones this repository and lauches the ansible playbook.

```
yay -S ansible --noconfirm && git clone https://github.com/T13nou/Archible.git && cd Archible && ansible-playbook -K playbook.yml
```

# Roles available

```
- [x] Working and tested
- [ ] Under testing
```

| Role/Feature  | Arch Linux | Debian | Ubuntu | OpenSuse |
| ------------- | ------------- | ------------- | ------------- | ------------- |
| Content Cell  | Content Cell  | Content Cell  | Content Cell  | Content Cell  |
| Content Cell  | Content Cell  | Content Cell  | Content Cell  | Content Cell  |

- [x] Create_Users: Handles the creation of user accounts on the system
- [x] Flatpak_Core: Installs Flatpak and Flathub repository
- [x] Flatpak_Softwares: Installs specific Flatpak applications
- [x] KDE_Theme: Uses Konsave to restore KDE environment
- [x] NFS_Mount: Sets up and mounts Network File System (NFS) shares
- [x] NumLock_On/tasks: Ensures NumLock in SDDM
- [x] System_Update: Updates the system using the Pacman package manager
- [x] amd_drivers: Installs AMD graphics drivers
- [x] base_software: Installs essential base software
- [x] bluetooth: Installs Bluetooth and enables it
- [x] game_compatibility: Tweaks system
- [x] kde_software: Installs additional software packages for the KDE desktop environment
- [x] pacman_optimization: Optimizes the Pacman package manager
- [ ] Floorp_Browser: Installs the Floorp browser, providing users with an alternative web browsing option.
- [ ] fish_terminal: Sets up the Fish terminal, a user-friendly and feature-rich command-line interface.
