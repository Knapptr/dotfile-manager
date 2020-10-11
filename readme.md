# Dotfile Backup

## A VERY simple backup utility

### How it works:
Dotfile Backup reads ~/.dotfilebackup.config and copies file listed to ~/dotfilemgmt/current
The previous (overwritten) configs will be saved in ~/dotfilemgmt/prev

### Config format
dotfilebackup.config MUST be in ~/ and MUST have the correct filename.
each file needs to be on its own line with NO extra white space. Comments will not work as of now.

### Backups
The "last backed up" version of files will be saved in ~/dotfilemgmt/prev. If a file is
removed from the list, the last backed up version will NOT be removed from ./prevdotfiles. This is 'by design'...or something. If used with git the ./prevdotfiles should be added to .gitignore, as git will handle backups anyway...


