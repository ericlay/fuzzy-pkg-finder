 # fuzzy-pkg-finder

**Simple cli command for using fzf to search and install packages.**\
 \
Performs live search by package name and presents package information including file list in preview pane. \
Includes fpf systemd timer to keep files database up to date automagically. 
  \
*For use with Pacman or Yay package managers only.*\
*Entirely inspired by command found at https://wiki.archlinux.org/index.php/Fzf* \
 \
Installation: 
```bash
git clone https://github.com/ericlay/fuzzy-pkg-finder
cd fuzzy-pkg-finder
makepkg
sudo pacman -U fuzzy-pkg-finder-0.1-1-any.pkg.tar.xz 
```
 \
After installation completes:
```bash
sudo systemctl enable fpf.timer fpf.service
sudo systemctl start fpf.service fpf.timer
```
 \
Usage: \
Invoke `pacfzf` or `yayfzf` commands to search the respective repositories. Press 'Enter' key to select desired package. Follow Pacman/Yay instructions to complete install.

