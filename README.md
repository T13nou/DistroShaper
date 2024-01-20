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


- [x] Create_Users: Handles the creation of user accounts on the system.
- [x] Flatpak_Core: Installs the core components required for Flatpak, a universal software deployment and package management system.
- [x] Flatpak_Softwares: Installs specific Flatpak applications, extending the software availability on the system.
- [x] KDE_Theme: Configures the KDE desktop environment's theme to enhance the visual experience.
- [x] NFS_Mount: Sets up and mounts Network File System (NFS) shares, facilitating file sharing across a network.
- [x] NumLock_On/tasks: Ensures NumLock is turned on by default for improved user convenience.
- [x] System_Update: Updates the system using the Pacman package manager, ensuring software packages are up-to-date.
- [x] amd_drivers: Installs AMD graphics drivers for optimal performance on AMD hardware.
- [x] base_software: Installs essential base software required for a functional and productive system.
- [x] bluetooth: Configures Bluetooth settings, providing seamless connectivity for Bluetooth devices.
- [x] game_compatibility: Installs components to enhance game compatibility on the system.
- [x] kde_software: Installs additional software packages for the KDE desktop environment.
- [x] pacman_optimization: Optimizes the Pacman package manager for improved efficiency and performance.
- [ ] Floorp_Browser: Installs the Floorp browser, providing users with an alternative web browsing option.
- [ ] fish_terminal: Sets up the Fish terminal, a user-friendly and feature-rich command-line interface.
