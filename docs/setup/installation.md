# This will have info on OS setup

## Windows (WSL)
Technically, MOOS won't really run in Windows, so you'll need to somehow utilise Linux within Windows.  Windows Subsystem for Linux (WSL) allows you to use a Unix terminal within Windows in order to run Linux-specific programs and software with a compatibility layer. To do this, open Powershell with admin privileges and run the following command:

    dism.exe /online /enable-feature /featurename:Microsoft-Windows-Subsystem-Linux /all /norestart

If you have Windows 10 Version 2004 or newer (ignore if you do not), also enter:

    dism.exe /online /enable-feature /featurename:VirtualMachinePlatform /all /norestart 

Afterwards, restart your machine. If you have Windows 10 Version 2004 or newer (ignore if you do not), open Powershell with admin privileges again, and enter:

    wsl --set-default-version 2

Once those commands are run, then you need install a distro from the Windows Store. Any should work fine, but for the purposes of these labs, we will be using Ubuntu 20.04, which you can find here: https://www.microsoft.com/en-us/p/ubuntu-2004-lts/9n6svws3rx71. After installing your distro, run it and create a username and password. You're good after that!
