//First and foremost THANK YOU DEREK52!!

//I am new to github repos so if this in any way affects the branch I forked from please let me know!

//I'm gratefully forking this repo and using it as a template to save me countless hours spent distro-hopping and making it a less mandala like experience. 

# configure-linux-scripts

These are a few scripts designed to automate the process of installing your desired software, and making a few customization tweaks.

Using these scripts is pretty simple. Simply download or clone this repo, and cd into it.

From there run the linux-setup script and type in your operating system. That would look like this
```
./linux-setup.sh debian
```
It will then prompt you for a password, and you should be good to go from there.

This script calls a couple other scripts. One is `configure-linux.sh`, which has sudo rights, and installs a ton of software. There are multiple `configure-linux` scripts. `linux-setup.sh` will call the configure-linux script, from inside the folder, of the system you are using. 

For example:
```
./linux-setup.sh Fedora
```
will call `fedora/configure-linux.sh`

You can simply delete the folders for any OS you aren't using.

`linux-setup.sh` also calls `customize-home.sh` which does some non sudo stuff, like change wallpaper and adds a few directories to the home folder.

This is still a work in progress. I intend to add scripts for other systems, and some more config files and some utility scripts I've written for various things.
