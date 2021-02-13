
# Windows Terminal Settings

    This are my settings for the windows terminal.

---
### Search

    Press `Ctrl + Shift + F` to open the search box.

---
### Normal Pane Splits

    Press `ctrl + shift + e` to split the pane in vertical.
    Press `ctrl + shift + d` to split the pane in horizontal.
    Press `ctrl + shift + -` to split the pane in auto.

---
### Split Pane with Profiles

    In my case, I have 6 profiles

**Git Bash**

    Press `ctrl + shift + 1` to split the pane in vertical.
    Press `ctrl + alt + 1` to split the pane in horizontal.

**Debian**

    Press `ctrl + shift + 2` to split the pane in vertical.
    Press `ctrl + alt + 2` to split the pane in horizontal.

**Kali Linux**

    Press `ctrl + shift + 3` to split the pane in vertical.
    Press `ctrl + alt + 3` to split the pane in horizontal.

**Windows PowerShell**

    Press `ctrl + shift + 4` to split the pane in vertical.
    Press `ctrl + alt + 4` to split the pane in horizontal.

**Command Prompt**

    Press `ctrl + shift + 5` to split the pane in vertical.
    Press `ctrl + alt + 5` to split the pane in horizontal.

**Azure Cloud Shell**

    Press `ctrl + shift + 6` to split the pane in vertical.
    Press `ctrl + alt + 6` to split the pane in horizontal.

---
### Switch between Panes

    Press `ctrl + left` to go left.
    Press `ctrl + right` to go right.
    Press `ctrl + top` to go top.
    Press `ctrl + bottom` to go bottom.

---
### Generate a new GUID

    Lets imagine we have a new terminal and we want to create a new profile.
    For this, we need to generate a new GUID.
    First we need to open the **Windows PowerShell** and type the command `[guid]::NewGuid()`
    Now we can use the new generated GUID in our new profile.
````
{
    "guid": "{NEW GUID HERE}",
    "hidden": false,
    "name": "Git Bash",
    "commandline": "C:\\Program Files\\Git\\bin\\bash.exe",
    "icon": "%PROGRAMFILES%\\git\\mingw64\\share\\git\\git-for-windows.ico",
},
````
---
### Starting Directory with WSL

    For us to choose a starting directory when we launch a WSL terminal, we need to add this `"startingDirectory": "//wsl$/[SO DISTRO]/[PATH]"` to our profile.

##### For Debian/Kali
````
"startingDirectory": "//wsl$/Debian/home/[YOUR USERNAME]"
````
