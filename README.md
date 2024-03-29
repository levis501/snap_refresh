# snap_refresh
## One-shot update for snaps

*When firefox tells me there is a snap update, I shutdown firefox at my next convenience, then click this button.  Snaps are refreshed.  Then, I can start firefox again and get back to work.*

### This repository contains the source files for two tools

`snap_refresh` - a command line tool to restart the snap-store and refresh any available snaps

`snap_refresh.desktop` - a desktop entry to launch the above command line tool as an application

### To build the command line tool:

`  gcc -o snap_refresh snap_refresh.c`

`  sudo chown root snap_refresh`

### Install to /usr/bin (or your preferred location) with:

`  sudo mv snap_refresh /usr/bin`
  

### To use the desktop application, place the `.desktop` file where it will be picked up by your system

`  cp snap_refresh.desktop ~/.local/share/applications`

### Notes:
- If the command line tool is installed in a different location change the relevant line in the `snap_refresh.desktop` file.
- If you're only running from the command line, you can skip the chown & chmod steps and just `sudo snap_refresh`
