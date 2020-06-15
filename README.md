 # fuzzy-pkg-finder

**Simple cli command for using fzf to search and install packages.**\
 \
Leverages the power of fzf to search package names and presents complete package information in preview pane. \
On selection will hand off to Pacman or Yay to complete transaction. \
Includes fpf systemd timer to keep files database up to date automagically. 
  \
*For use with Pacman or Yay package managers only.*\
*Entirely inspired by command found at https://wiki.archlinux.org/index.php/Fzf* \
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
Syntax: fpf -[y|h]
Defaults to Pacman if no options passed

options:
-y	Search and install with Yay
-h	Print this help screen
```
