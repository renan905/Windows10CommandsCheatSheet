# Windows 10 Commands Cheat Sheet
A list of helpful Windows 10 Commands


## System File
If some Windows functions aren't working or Windows crashes, use the System File Checker to scan Windows and restore your files.

Terminal: *PowerShell*

$ DISM.exe /Online /Cleanup-image /Restorehealth
$ sfc /scannow

**observation:** It's recommended to restart your system and run the commands again

reference: [https://support.microsoft.com/en-us/help/929833/use-the-system-file-checker-tool-to-repair-missing-or-corrupted-system]

