# Prep: Practice in the Terminal

**Date Due:** March 18, 11:59pm PDT

## [The Command Line](https://ryanstutorials.net/linuxtutorial/commandline.php)

The command line is akin to the old MS-DOS commands I used hundreds of years
ago. Paths are separated by slashes (/) rather than the backslashes used in
Microsoft operating systems. Everything is relative to the "root" path, which
is indicated by a tilde (~). Some common commands:

- cd: Change directory (same as MS)
- mkdir: Make directory (same as MS)
- rmdirL Remove directory

### Important Directories

- /etc: Stores config files
- /var/log: Stores log files for system programs
- /bin: Several commonly-used programs are kept here
- /usr/bin: Another location for commonly-used programs

_Tab completion is your friend!_ Hitting tab will autocomplete paths (or present
a list of possible choices if there is more than one that fits what you've already
typed).
_Up arrows_ will cycle through your history of commands, which is a nice fast way
of repeating commands!

**Note: Spaces in names are perfectly valid, but a terrible idea.**

- Dots at the beginning of a name indicate a hidden file or directory

**Manual Pages**: basically help files that explain commands in detail

Vi text editor is evil. Anyway:

- ZZ (save and exit)
- q! (discard all changes and quit)
- w (save file)
- wq (save file and exit

cat (file) allows you to view the contents of a file

**Ctrl-C will generally get you out of trouble** whenever you're stuck

### Wildcards

\* = zero or more characters
? = a single characgter
[] = a range of characters
