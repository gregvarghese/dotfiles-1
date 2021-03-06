## dotfiles ##

This repo serves as a master collection of all my dotfiles. Each grouping has its own folder here. The install script will install all of the appropriate files for the platform to their respective place.

### Dependencies ###

The dotfiles installation requires the GNU program `stow`. To install this, do your brand of:

	brew install stow
	-or-
	sudo apt-get install stow


### Install ###

From cloned git repo folder:

    $ make

The Makefile will attempt to determine your platform automatically and install the right files. You can override this by specifying the platform specifically in the make command (e.g., `make OSX`). Or you can install specific packages with make as well (e.g., `make tmux`).

### OSX Setup ###

Optionally my full OSX setup script can be run directly from this repository. It should, with a little luck, configure the system, install all sorts of programs, pull down these dotfiles, and run all the necessary installers.

	curl https://raw.githubusercontent.com/jamestomasino/dotfiles/master/osxsetup.sh | bash

### Credits ####

Most stuff is original, but a lot of the aliases and functions are ripped off from around the web. If you notice your idea in my repo somewhere and want credit, send me a note. Once I'm done rolling my eyes, I'll post a link or something.

Special thanks to [Stephen Tudor](https://github.com/smt/), my partner in dotfile exploration.
