 # fuzzy-pkg-finder

**Simple cli command for using fzf to search and install packages.**\
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
Syntax: fpf -[a|l|la|R|Ra|h]
Defaults to Pacman if no options passed

options:
a     Search/List and install from AUR with Yay
l     Search/List installed packages from official repo
la    Search/List installed packages from AUR repo
R     Search/List installed packages from official repos for removal
Ra    Search/List installed packages from AUR repo for removal
h     Print this help screen.
```
