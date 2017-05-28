# General   
This is where I'll upload any of my Arch User Repository PKGBUILD's before they actually get uploaded to the AUR.  
After the upload the the AUR I will most likely remove it from this git, as I don't want to maintain two separate git's.  

Each PKGBUILD has a README that I will put the current working/tested status in, so please check it before submitting an issue.

## Usage  
**Pre-requisites to use**  
*   You need an Arch-based Linux distribution. If you are unsure of what you have, run `uname -r` in your terminal to check. It should return something similar to `X.X.X-ARCH` if you are using an Arch-based Linux distribution.

*   You need the `git` package before-hand. You can check if you have it by running `pacman -Q git` from the terminal.
    *   If that command returns `error: package 'git' was not found` then run `sudo pacman -S git`  

### How To Use
**Note:** replace `nameOfProject` with whatever PKGBUILD folder you want.   
*   Example: `cd aur-packages/tribler/`  -- **File paths are case-sensitive.**  

Open your terminal, and run the following commands...
```
cd ~/Downloads
git clone https://github.com/sum01/aur-packages.git
cd aur-packages/NameOfProjectHere/
makepkg -csi PKGBUILD
```
