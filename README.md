<img src=https://github.com/T13nou/Archible/blob/main/images/t13nou_Arch_Linux_Terraforming_Ansible_with_text_Archible_930879c2-0545-4c05-9996-286f5f4f803d.png width="1000" height="100">

#  DistroShaper

This Ansible script is designed to automate the customization of a freshly installed Linux distribution (Arch/Ubuntu/OpenSuseTW), streamlining the setup process for users. The script is organized into various roles, each responsible for specific aspects of system configuration and software installation. By executing this script, users can effortlessly apply a set of predefined configurations and install a curated collection of software tailored to enhance the Linux experience.

Feel free to clone this repository and tweak playbook to your needs :)

https://github.com/T13nou/DistroShaper/assets/64090484/cea5dbc0-8181-46a0-9dff-42d6400b2e32

# Usage 
1. Fork this repository
2. Edit the variables in group_vars/all.yml (Users, Mounts, Softwares to install)
3. Launch the following commands depending on your distro

**Arch & derivatives**
```
yay -S ansible --noconfirm && git clone https://github.com/T13nou/DistroShaper.git && cd DistroShaper && ansible-playbook -K playbook.yml
```

**Ubuntu & derivatives**
```
sudo apt install ansible git && git clone https://github.com/T13nou/DistroShaper.git && cd DistroShaper && ansible-playbook -K playbook.yml
```

**OpenSuse Tumbleweed**
```
sudo zypper install ansible git-core && git clone https://github.com/T13nou/DistroShaper.git && cd DistroShaper && ansible-playbook -K playbook.yml
```
4. Enter your root password and let the playbook run

# Roles available


| Role/Feature  | Description | Need variables edit | Arch | Ubuntu | OpenSuseTW |
| ------------- | ------------- |      :---:       |      :---:       |      :---:       |      :---:       |
| Ansible_Dependancies | Installs some ansible dependancies for the paybook to run properly | No | <img src=/images/checked.png width="30" height="30"> | <img src=/images/checked.png width="30" height="30"> | <img src=/images/checked.png width="30" height="30"> |
| Ansible_Facts | Displays ansible facts (for debug only) | No | <img src=/images/checked.png width="30" height="30"> | <img src=/images/checked.png width="30" height="30"> | <img src=/images/checked.png width="30" height="30"> |
| Drivers_AMD | Installs AMD Drivers | No | <img src=/images/checked.png width="30" height="30"> | <img src=/images/checked.png width="30" height="30"> | <img src=/images/checked.png width="30" height="30"> |
| Drivers_Bluetooth | Installs and enables bluetooth | No| <img src=/images/checked.png width="30" height="30"> | <img src=/images/checked.png width="30" height="30"> | <img src=/images/checked.png width="30" height="30"> |
| Flatpak_Core | Installs flatpak bin and flathub repo | No | <img src=/images/checked.png width="30" height="30"> | <img src=/images/checked.png width="30" height="30"> | <img src=/images/checked.png width="30" height="30"> |
| Share_Mount | Mounts shares (nfs/smb) | Yes | <img src=/images/checked.png width="30" height="30"> | <img src=/images/checked.png width="30" height="30"> | <img src=/images/checked.png width="30" height="30"> |
| Software_Fish_Install | | No |  <img src=/images/work-in-progress.png width="30" height="30"> | <img src=/images/work-in-progress.png width="30" height="30"> | <img src=/images/work-in-progress.png width="30" height="30"> |
| Software_Floorp_Install | | No |  <img src=/images/work-in-progress.png width="30" height="30"> | <img src=/images/work-in-progress.png width="30" height="30"> | <img src=/images/work-in-progress.png width="30" height="30"> |
| Software_ArchUpdate_Install | | No | <img src=/images/checked.png width="30" height="30"> |  |  |
| Software_My_Applications | Installs apps of your choice | Yes | <img src=/images/checked.png width="30" height="30"> | <img src=/images/checked.png width="30" height="30"> | <img src=/images/checked.png width="30" height="30"> |
| Software_My_Flatpaks | Installs flatpaks of your choice | Yes | <img src=/images/checked.png width="30" height="30"> | <img src=/images/checked.png width="30" height="30"> | <img src=/images/checked.png width="30" height="30"> |
| System_Update | Performs full system update/upgrade | No | <img src=/images/checked.png width="30" height="30"> | <img src=/images/checked.png width="30" height="30"> | <img src=/images/checked.png width="30" height="30"> | <img src=/images/checked.png width="30" height="30"> |
| Tweak_Game_Compatibility | Increases vm.max_map_count value to help games running | No | <img src=/images/checked.png width="30" height="30"> | <img src=/images/checked.png width="30" height="30"> | <img src=/images/checked.png width="30" height="30"> | <img src=/images/checked.png width="30" height="30"> |
| Tweak_Neofetch_Customization | Adds Disks and IP info | No | <img src=/images/checked.png width="30" height="30"> | <img src=/images/checked.png width="30" height="30"> | <img src=/images/checked.png width="30" height="30"> | <img src=/images/checked.png width="30" height="30"> |
| Tweak_NumLock_On | Turns on Numlock on SDDM | No | <img src=/images/checked.png width="30" height="30"> | <img src=/images/checked.png width="30" height="30"> | <img src=/images/checked.png width="30" height="30"> | <img src=/images/checked.png width="30" height="30"> |
| Tweak_PackageMgr_Customization | Optimizes packet manager | No | <img src=/images/checked.png width="30" height="30"> | <img src=/images/checked.png width="30" height="30"> | <img src=/images/checked.png width="30" height="30"> | <img src=/images/checked.png width="30" height="30"> |
| Users_Create | Creates users with homes and password | Yes | <img src=/images/checked.png width="30" height="30"> | <img src=/images/checked.png width="30" height="30"> | <img src=/images/checked.png width="30" height="30"> | <img src=/images/checked.png width="30" height="30"> |
| Users_Faces | Restore saved profile pictures | Yes | <img src=/images/checked.png width="30" height="30"> | <img src=/images/checked.png width="30" height="30"> | <img src=/images/checked.png width="30" height="30"> | <img src=/images/checked.png width="30" height="30"> |
| Users_KDE_Theme_Restore | Uses konsave plugin to restore a saved KDE profile | Yes | <img src=/images/checked.png width="30" height="30"> | <img src=/images/checked.png width="30" height="30"> | <img src=/images/checked.png width="30" height="30"> | <img src=/images/checked.png width="30" height="30"> |
