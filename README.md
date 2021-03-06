 <div align="right">
    <img src="https://img.shields.io/static/v1?label=Language&message=shell&color=%235BB97E&style=flat-square"/>
    <img src="https://img.shields.io/github/license/ericlay/fuzzy-pkg-finder?color=%235BB97E&label=LIC&style=flat-square"/>
</div>
 <div align="center"><h1>📦<br>Fuzzy-pkg-finder</h1></div>

**Simple cli utility using fzf to search and install/list/remove packages.**\
 \
![Screenshot](https://gitlab.com/airclay/fuzzy-pkg-finder/-/raw/master/fpf.png) \
 \
Leverages the power of fzf to search package names and presents complete package information in preview pane. \
On selection will hand off to Pacman or Yay to complete transaction. \
  \
*For use with Pacman or Yay package managers only.*\
 \
Installation: 
```
git clone https://github.com/ericlay/fuzzy-pkg-finder
cd fuzzy-pkg-finder
makepkg -sric
```
 \
Usage: 
```
Syntax: fpf -[a|l|la|R|o|h]
Defaults to Pacman if no options passed

Searching for a package:
ex: fpf [pkg name] for official repo search
ex: fpf -a [pkg name] for aur search

options:
-a     Search/List and install from AUR with Yay
-l     Search/List installed packages from official repo
-la    Search/List installed packages from AUR 
-R     Search/List installed packages for removal
-o     Search/List orphaned packages for removal
-h     Print this help screen.
```
\
Keybinds:
```
When browsing AUR or installed Aur pkgs:
'ctrl + p' Will preview the highlighted pkgbuild file
'ctrl + x' Will return to the highlighted pkg info
```
 \
*Fish shell users:* \
Use alternate `fpff` command instead. (fuzzy-pkg-finder-fish)\
Same script just adapted the bash-isms so the preview window will work.
