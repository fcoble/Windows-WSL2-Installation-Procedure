# WSL2 Webserver

This repository provides general instructions for the installation of WSL2 (Windows Subsystem for Linux) on a Windows 10 or 11 machine.

Although WSL is now and industry standard option and well documented on the web, **no warranty is provided** for these instructions. _Install WSL or any other Windows Updates at your own risk_.

## Install the Windows Subsystem for Linux

Before installing any Linux distributions on Windows, you must enable the “Windows Subsystem for Linux” optional feature.

### Open PowerShell as Administrator and run:

`dism.exe /online /enable-feature /featurename:Microsoft-Windows-Subsystem-Linux /all /norestart
`

Restart your machine (required).  Move on to update to WSL 2.

 ## Update to WSL 2

 To update to WSL 2, you must meet the follow criteria:

- Running Windows 10, updated to version 2004, Build 19041 or higher.
- Enable the ‘Virtual Machine Platform’ optional component

### Open PowerShell as Administrator and run:

`dism.exe /online /enable-feature /featurename:VirtualMachinePlatform /all /norestart
`
Restart your machine to complete the WSL install and update to WSL 2.

## Set WSL 2 as the Default Version

Run the following command in Powershell to set WSL 2 as the default version when installing a new Linux distribution:

`wsl --set-default-version 2
`
## Install the Linux Distribution of Your Choice

Open the Microsoft Store and install your favorite Linux distribution. The most current version of Ubuntu may be a good choice. Fedora (Redhat) is available, but is not free.

## Start the Linux Subsystem

Click the Application icon for your distribution from Windows Apps, or type wsl.exe from cmd.exe. You will be prompted to create an account upon the first lauch of your distro. 



