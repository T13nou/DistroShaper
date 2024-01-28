<img src=https://github.com/T13nou/Archible/blob/main/images/t13nou_Arch_Linux_Terraforming_Ansible_with_text_Archible_930879c2-0545-4c05-9996-286f5f4f803d.png width="1000" height="100">

#  DistroShaper

This Ansible script is designed to automate the customization of a freshly installed Linux distribution (Arch/Ubuntu/OpenSuseTW), streamlining the setup process for users. The script is organized into various roles, each responsible for specific aspects of system configuration and software installation. By executing this script, users can effortlessly apply a set of predefined configurations and install a curated collection of software tailored to enhance the Linux experience.

Feel free to clone this repository and tweak playbook to your needs :)

The following command installs ansible, clones this repository and lauches the ansible playbook.

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


| Role/Feature  | Description | Arch Linux | Debian | Ubuntu | OpenSuse |
| ------------- | ------------- |      :---:       |      :---:       |      :---:       |      :---:       |
| Ansible_Dependancies | <img src=/images/checked.png width="30" height="30"> | <img src=/images/checked.png width="30" height="30"> | <img src=/images/checked.png width="30" height="30"> | <img src=/images/checked.png width="30" height="30"> |
| Ansible_Facts | <img src=/images/checked.png width="30" height="30"> | <img src=/images/checked.png width="30" height="30"> | <img src=/images/checked.png width="30" height="30"> | <img src=/images/checked.png width="30" height="30"> |
| Drivers_AMD | <img src=/images/checked.png width="30" height="30"> | <img src=/images/checked.png width="30" height="30"> | <img src=/images/checked.png width="30" height="30"> | <img src=/images/checked.png width="30" height="30"> |
| Drivers_Bluetooth | <img src=/images/checked.png width="30" height="30"> | <img src=/images/checked.png width="30" height="30"> | <img src=/images/checked.png width="30" height="30"> | <img src=/images/checked.png width="30" height="30"> |
| Flatpak_Core | <img src=/images/checked.png width="30" height="30"> | <img src=/images/checked.png width="30" height="30"> | <img src=/images/checked.png width="30" height="30"> | <img src=/images/checked.png width="30" height="30"> |
| Share_Mount | <img src=/images/checked.png width="30" height="30"> | <img src=/images/checked.png width="30" height="30"> | <img src=/images/checked.png width="30" height="30"> | <img src=/images/checked.png width="30" height="30"> |
| Software_Fish_Install | 
| Software_Floorp_Install | 
| Software_My_Applications | <img src=/images/checked.png width="30" height="30"> | <img src=/images/checked.png width="30" height="30"> | <img src=/images/checked.png width="30" height="30"> | <img src=/images/checked.png width="30" height="30"> |
| Software_My_Flatpaks | <img src=/images/checked.png width="30" height="30"> | <img src=/images/checked.png width="30" height="30"> | <img src=/images/checked.png width="30" height="30"> | <img src=/images/checked.png width="30" height="30"> |
| System_Update | <img src=/images/checked.png width="30" height="30"> | <img src=/images/checked.png width="30" height="30"> | <img src=/images/checked.png width="30" height="30"> | <img src=/images/checked.png width="30" height="30"> |
| Tweak_Game_Compatibility | 
| Tweak_Neofetch_Customization | <img src=/images/checked.png width="30" height="30"> | <img src=/images/checked.png width="30" height="30"> | <img src=/images/checked.png width="30" height="30"> | <img src=/images/checked.png width="30" height="30"> |
| Tweak_NumLock_On | <img src=/images/work-in-progress.png width="30" height="30"> |  |  |  |
| Tweak_PackageMgr_Customization |<img src=/images/work-in-progress.png width="30" height="30"> |  |  |  |
| Users_Create | <img src=/images/checked.png width="30" height="30"> | <img src=/images/checked.png width="30" height="30"> | <img src=/images/checked.png width="30" height="30"> | <img src=/images/checked.png width="30" height="30"> |
| Users_Faces | <img src=/images/checked.png width="30" height="30"> | <img src=/images/checked.png width="30" height="30"> | <img src=/images/checked.png width="30" height="30"> | <img src=/images/checked.png width="30" height="30"> |
| Users_KDE_Theme_Restore | <img src=/images/checked.png width="30" height="30"> | <img src=/images/checked.png width="30" height="30"> | <img src=/images/checked.png width="30" height="30"> | <img src=/images/checked.png width="30" height="30"> |
