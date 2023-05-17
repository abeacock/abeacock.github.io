---
title: Notes
---

## Chocolatey

In an administrative Powershell console:  
`Set-ExecutionPolicy Bypass -Scope Process -Force; [System.Net.ServicePointManager]::SecurityProtocol = [System.Net.ServicePointManager]::SecurityProtocol -bor 3072; iex ((New-Object System.Net.WebClient).DownloadString('https://chocolatey.org/install.ps1'))`

Then from the same console run:  
`choco install chocolateygui`

To import an existing chocolatey.config file:  
`choco install chocolatey.config`

## git

Set your username and email address  
`git config --global user.name "Andrew Beacock"`  
`git config --global user.email "email@address"`

Save credentials locally  
`git config credential.helper store`

Reset local to be same as remote
`git fetch origin`
`git reset --hard origin/master`

## vim

Add to .bash_profile `alias vi=vim`  
Install vim-go plugin

- `git clone https://github.com/fatih/vim-go.git ~/.vim/pack/plugins/start/vim-go`
- start vim
- `:GoInstallBinaries`
