<img src=https://github.com/T13nou/Archible/blob/main/images/t13nou_Arch_Linux_Terraforming_Ansible_with_text_Archible_930879c2-0545-4c05-9996-286f5f4f803d.png width="1000" height="100">

#  DistroShaper

This Ansible script is designed to automate the customization of a freshly installed Linux distribution (Arch/Ubuntu/OpenSuseTW), streamlining the setup process for users. The script is organized into various roles, each responsible for specific aspects of system configuration and software installation. By executing this script, users can effortlessly apply a set of predefined configurations and install a curated collection of software tailored to enhance the EndeavourOS experience.

Feel free to clone this repository and tweak playbook to your needs :)

The following command installs ansible, clones this repository and lauches the ansible playbook.


## Arch & derivatives
```
yay -S ansible --noconfirm && git clone https://github.com/T13nou/Archible.git && cd Archible && ansible-playbook -K playbook.yml
```

## Ubuntu & derivatives
```
sudo apt install ansible git && git clone https://github.com/T13nou/Archible.git && cd Archible && ansible-playbook -K playbook.yml
```

## OpenSuse Tumbleweed
```
sudo zypper install ansible git-core && git clone https://github.com/T13nou/Archible.git && cd Archible && ansible-playbook -K playbook.yml
```


# Roles available


| Role/Feature  | Description | Arch Linux | Debian | Ubuntu | OpenSuse |
| ------------- | ------------- |      :---:       |      :---:       |      :---:       |      :---:       |
| Create_Users | Handles the creation of user accounts on the system  | <img src=/images/checked.png width="30" height="30"> | <img src=/images/checked.png width="30" height="30"> | <img src=/images/checked.png width="30" height="30"> | <img src=/images/checked.png width="30" height="30"> |
| Drivers_AMD | Installs Flatpak and Flathub repository  | <img src=/images/checked.png width="30" height="30">  |  |  | <img src=/images/checked.png width="30" height="30"> |
| Flatpak_Core | Installs Flatpak and Flathub repository  | <img src=/images/checked.png width="30" height="30">  |  |  |  |
| Flatpak_Softwares  | Installs specific Flatpak applications | <img src=/images/checked.png width="30" height="30">  | <img src=/images/checked.png width="30" height="30"> | <img src=/images/checked.png width="30" height="30"> | <img src=/images/checked.png width="30" height="30"> |
| KDE_Theme  | Uses Konsave to restore KDE environment | <img src=/images/checked.png width="30" height="30"> |  |  |  |
| NeoFetch_Customization | Adds disk info & local IP to Neofetch | <img src=/images/checked.png width="30" height="30"> | <img src=/images/checked.png width="30" height="30"> | <img src=/images/checked.png width="30" height="30"> | <img src=/images/checked.png width="30" height="30"> |
| NFS_Mount  | Sets up and mounts Network File System (NFS) shares | <img src=/images/checked.png width="30" height="30"> | <img src=/images/checked.png width="30" height="30"> | <img src=/images/checked.png width="30" height="30"> | <img src=/images/checked.png width="30" height="30"> |
| NumLock_On/tasks  | Ensures NumLock in SDDM | <img src=/images/checked.png width="30" height="30"> | <img src=/images/checked.png width="30" height="30"> |  |  |
| System_Update | Updates the system using the distro package manager | <img src=/images/checked.png width="30" height="30"> | <img src=/images/checked.png width="30" height="30"> | <img src=/images/checked.png width="30" height="30"> | <img src=/images/checked.png width="30" height="30"> |
| amd_drivers | Installs AMD graphics drivers | <img src=/images/checked.png width="30" height="30"> | <img src=/images/checked.png width="30" height="30"> |  |  |
| base_software | Installs essential base software | <img src=/images/checked.png width="30" height="30"> | <img src=/images/checked.png width="30" height="30"> |  | <img src=/images/checked.png width="30" height="30"> |
| bluetooth | Installs Bluetooth and enables it | <img src=/images/checked.png width="30" height="30"> |  |  |  |
| kde_software | Installs additional software packages for the KDE desktop environment | <img src=/images/checked.png width="30" height="30"> |  |  |  |
| pacman_optimization | Optimizes the Pacman package manager | <img src=/images/checked.png width="30" height="30"> |  |  |  |
| Floorp_Browser | Installs the Floorp browser, providing users with an alternative web browsing option. | <img src=/images/work-in-progress.png width="30" height="30"> |  |  |  |
| fish_terminal | Sets up the Fish terminal, a user-friendly and feature-rich command-line interface. | <img src=/images/work-in-progress.png width="30" height="30"> |  |  |  |



