# Windows 10 Commands Cheat Sheet
A list of helpful Windows 10 Commands

## Add Windows Terminal to Explorer Context Menu
https://github.com/BroJenuel/Explorer-Context-Menu-Integration-for-windows-terminal

## System File
If some Windows functions aren't working or Windows crashes, use the System File Checker to scan Windows and restore your files.

Terminal: *PowerShell*
    
    * DISM.exe /Online /Cleanup-image /Restorehealth
    * sfc /scannow

**observation:** It's recommended to restart your system and run the commands again

reference: [https://support.microsoft.com/en-us/help/929833/use-the-system-file-checker-tool-to-repair-missing-or-corrupted-system]

## WSL

    Set WSL 2 as default
    wsl --set-default-version 2
    
    Convert Ubuntu on WSL 1 to WSL 2
    wsl.exe --set-version Ubuntu 2

## WSL2 Kernel Update
https://wslstorestorage.blob.core.windows.net/wslblob/wsl_update_x64.msi



# Motherboard MAX RAM
wmic memphysical get maxcapacity


# Add Git Bash to Windows Terminal
```
{
    "guid": "{00000000-0000-0000-ba54-000000000002}",
    "commandline": "%PROGRAMFILES%/git/usr/bin/bash.exe -i -l",
    "icon": "%PROGRAMFILES%/Git/mingw64/share/git/git-for-windows.ico",
    "name" : "Bash",
    "startingDirectory" : "%USERPROFILE%"
}
```
