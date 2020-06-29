---
title: Notes
---

## Chocolatey
In an administrative Powershell console:  
`Set-ExecutionPolicy Bypass -Scope Process -Force; [System.Net.ServicePointManager]::SecurityProtocol = [System.Net.ServicePointManager]::SecurityProtocol -bor 3072; iex ((New-Object System.Net.WebClient).DownloadString('https://chocolatey.org/install.ps1'))`

Then from the same console run:  
`choco install chocolateygui`

## msys2
Install msys2 via [Chocolatey](https://chocolatey.org/)  
Goto `C:\tools\msys64` and run `msys2.exe`

* Update installed packages `pacman -Syu`
* Searching for packages `pacman -Ss _package_`
* Installing a package `pacman -S _package_`

Install GCC stuff  
`pacman -S mingw-w64-x86_64-toolchain`

## Ansible
* [Ansible on Windows msys2 script](https://gist.github.com/DaveB93/db94a6b310e08c928c0778f766562ab0#file-python3-install-ansible-on-msys2-sh)
* [Update Powershell & .NET framework](https://docs.ansible.com/ansible/latest/user_guide/windows_setup.html#upgrading-powershell-and-net-framework)
* create `/etc/ansible/hosts` and add `localhost`
* `ansible all -m ping`

## git
Set your username and email address  
`git config --global user.name "Andrew Beacock"`
`git config --global user.email "email@address"`

Save credentials locally  
`git config credential.helper store`

## vim
Add to .bash_profile `alias vi=vim`  
Install vim-go plugin
* `git clone https://github.com/fatih/vim-go.git ~/.vim/pack/plugins/start/vim-go`
* start vim
* `:GoInstallBinaries`
