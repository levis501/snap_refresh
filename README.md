# snap_refresh
## One-shot update for snaps

### This repository contains the source files for two tools

`snap_refresh` - a command line tool to restart the snap-store and refresh any available snaps

`snap_refresh.desktop` - a desktop entry to launch the above command line tool as an application

### To build the command line tool:

`  gcc -o snap_refresh snap_refresh.c`

`  sudo chown root snap_refresh`

`  sudo chmod u+s snap_refresh`


### Install to /usr/bin (or your preferred location) with:

`  sudo mv snap_refresh /usr/bin`
  

### To use the desktop application, place the `.desktop` file where it will be picked up by your system

`  cp snap_refresh.desktop ~/.local/share/applications`

### If the command line tool is installed in a different location change the relevant line in the snap_refresh.desktop file.
