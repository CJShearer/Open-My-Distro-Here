# Open-My-Distro-Here
Microsoft recently added a shift+right-click context menu option for opening the default shell in the working directory. Unfortunately, there's no provided method to change this to a custom WSL distribution (I am aware of wslconfig; it does not have the desired effect). With the right program and arguments placed in the registry, the correct distro can be launched in the working directory.

# Installation:
1. Change ownership of HKEY_CLASSES_ROOT\Directory\Background\shell\WSL with [these instructions](https://www.tenforums.com/tutorials/3587-change-owner-file-folder-drive-registry-key-windows-10-a.html#option4).
 Be sure to select:
 - "Replace owner of subcontainers and objects"
 - "Replace all child object permission entries with inheritable permission entries from this object"

2. (Optional) In the registry file, change "ubuntu1804.exe" to your distribution's executable.
3. Import/Run the regedit file.

# Usage:
 Shift+right-click in a directory and select the "Open Linux Shell Here" option. Your distro should launch in the working directory.

# Additional info:
Check [the wiki](https://github.com/CJShearer/Open-My-Distro-Here/wiki) for a project "post-mortem".
