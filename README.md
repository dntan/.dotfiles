# Rationale:
I need a way of saving my configurations and capture my learning progress in one place. As I learn how to configure and curate my own system, I want to be able to share my preferences across any operating system that I use linux, macOS and windows. This is ever evolving repo, depending on how much I wish to keep it up to date.

## Requirements:
1. Install git on the OS. e.g. `sudo pacman -S git` on arch based systems
2. Create a folder called DATA in the home dir then `git clone https://github.com/dntan/.dotfiles`
3. Ensure `.sh` files are executable from this cloned repo.

## Getting started:

### 1. twm_on_arch:
Install a tiling window manager if on a arco/arch based system.
a. Run `chadwm.sh`

### 2. emacs_on_arch:
Review and run the `dannys_emacs` install script. this should:
1. Install emacs if it doesn't exist already
2. Copy over the repo emacs.d folder to `~/.config/` including my configured `config.org` and `init.el`.
3. Configure caplocks to ctrl with `.Xmodmap`
4. Check if on DE or TWM. Configure Emacs Daemon and Emacsclient accordingly. This will edit either autostartup or run.sh AND (sxhkdrc OR xfce4 ... something) 
5. logout.
