 <div align="right">
    <img src="https://img.shields.io/static/v1?label=Language&message=shell&color=%235BB97E&style=flat-square"/>
    <img src="https://img.shields.io/github/license/ericlay/fuzzy-pkg-finder?color=%235BB97E&label=LIC&style=flat-square"/>
</div>
 <div align="center"><h1>📦<br>Fuzzy-pkg-finder</h1></div>

**Simple cli utility using fzf to search and install/list/remove packages.**\
 \
![Screenshot](https://gitlab.com/airclay/fuzzy-pkg-finder/-/raw/master/fpf.png) \
 \
Leverages the power of fzf to search package names and descriptions then presents complete package information in preview pane. \
On selection will hand off to Pacman or Paru/Yay to complete transaction. \
  \
*For use with Pacman/Yay/Paru package managers only.*\
 \
 There are countless fzf package manager wrappers out there, some much more built out that this.
 What separates Fuzzy-pkg-finder?
- It's mine and it works the way I like it to \
- It works as a simple script to wrap pacman/yay/paru, no need to rebuild the wheel \
- Searches both package names and descriptions for keyword \
- Hide preview window to see only packages and descriptions \
- Shows files list and/or missing files for official repo or installed AUR packages \
- Toggle between package info view and PKGBUILD view on AUR package preview \
 \
Installation: \
For Arch and arch-based distros, it is available in the AUR. \
Use: `paru -S fuzzy-pkg-finder` or `yay -S fuzzy-pkg-finder` \
 \
Manual build and install:
```
git clone https://github.com/ericlay/fuzzy-pkg-finder
cd fuzzy-pkg-finder
makepkg -sric
```
 \
Usage: 
```
Syntax: fpf [-a| --aur] [-l| --list-installed] [-la| --list-aur-installed]
              [R| --remove] [-o| --orphans] [-h | --help]
Defaults to Pacman if no options passed

Searching for a package:
ex: fpf [pkg name] for official repo search
ex: fpf -a [pkg name] for aur search

Options:
-a, --aur
    Search/List and install from AUR with Yay

-l, --list-installed
    Search/List installed packages from official repo

-la, --list-aur-installed
    Search/List installed packages from AUR 

-R, -remove
     Search/List installed packages for removal

-o, --orphans
     Search/List orphaned packages for removal

-h, --help
     Print this help screen
```
\
Keybinds:
```
'ctrl + /' Toggle the preview window
'ctrl + h' Show help in the preview window
'ctrl + k' Show the keybinds in teh preview window
'ctrl + n' Move to the next selected item
'ctrl + b' Back to previoius selected item

When browsing AUR or installed Aur pkgs:
'ctrl + p' Preview the highlighted pkgbuild file
'ctrl + x' Return to the highlighted pkg info
```
