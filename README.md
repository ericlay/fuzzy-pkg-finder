 # Fuzzy-pkg-finder

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

options:
a     Search/List and install from AUR with Yay
l     Search/List installed packages from official repo
la    Search/List installed packages from AUR 
R     Search/List installed packages from official repos for removal
o     Search/List orphaned packages for removal
h     Print this help screen.
```
