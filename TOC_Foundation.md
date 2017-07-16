Table of Contents

I. introduction to Linux
  1. Linux history
  - 1969
  - 1980s
  - 1990s
  - 2015
2. distributions
Red Hat
Ubuntu
Debian
Other
Which to choose ?
3. licensing
about software licenses
public domain software and freeware
Free Software or Open Source Software
GNU General Public License
using GPLv3 software
BSD license
other licenses
combination of software licenses
II. installing Linux
4. installing Debian 8
Debian
Downloading
virtualbox networking
setting the hostname
adding a static ip address
Debian package management
5. installing CentOS 7
download a CentOS 7 image
Virtualbox
CentOS 7 installing
CentOS 7 first logon
setting the hostname
Virtualbox network interface
configuring the network
adding one static ip address
package management
logon from Linux and MacOSX
logon from MS Windows
6. getting Linux at home
download a Linux CD image
download Virtualbox
create a virtual machine
attach the CD image
install Linux
III. first steps on the command line
7. man pages
man $command
man $configfile
man $daemon
man -k (apropos)
whatis
whereis
man sections
man $section $file
man man
mandb
8. working with directories
pwd
cd
cd ~
cd ..
cd -
absolute and relative paths
path completion
ls
ls -a
ls -l
ls -lh
mkdir
mkdir -p
rmdir
rmdir -p
practice: working with directories
solution: working with directories
9. working with files
all files are case sensitive
everything is a file
file
touch
create an empty file
touch -t
rm
remove forever
rm -i
rm -rf
cp
copy one file
copy to another directory
cp -r
copy multiple files to directory
cp -i
mv
rename files with mv
rename directories with mv
mv -i
rename
about rename
rename on Debian/Ubuntu
rename on CentOS/RHEL/Fedora
practice: working with files
solution: working with files
10. working with file contents
head
tail
cat
concatenate
create files
custom end marker
copy files
tac
more and less
strings
practice: file contents
solution: file contents
11. the Linux file tree
filesystem hierarchy standard
man hier
the root directory /
binary directories
/bin
other /bin directories
/sbin
/lib
/opt
configuration directories
/boot
/etc
data directories
/home
/root
/srv
/media
/mnt
/tmp
in memory directories
/dev
/proc conversation with the kernel
/sys Linux 2.6 hot plugging
/usr Unix System Resources
/usr/bin
/usr/include
/usr/lib
/usr/local
/usr/share
/usr/src
/var variable data
/var/log
/var/log/messages
/var/cache
/var/spool
/var/lib
/var/...
practice: file system tree
solution: file system tree
IV. shell expansion
12. commands and arguments
arguments
white space removal
single quotes
double quotes
echo and quotes
commands
external or builtin commands ?
type
running external commands
which
aliases
create an alias
abbreviate commands
default options
viewing aliases
unalias
displaying shell expansion
practice: commands and arguments
solution: commands and arguments
13. control operators
; semicolon
& ampersand
$? dollar question mark
&& double ampersand
|| double vertical bar
combining && and ||
# pound sign
\ escaping special characters
end of line backslash
practice: control operators
solution: control operators
14. shell variables
$ dollar sign
case sensitive
creating variables
quotes
set
unset
$PS1
$PATH
env
export
delineate variables
unbound variables
practice: shell variables
solution: shell variables
15. shell embedding and options
shell embedding
backticks
backticks or single quotes
shell options
practice: shell embedding
solution: shell embedding
16. shell history
repeating the last command
repeating other commands
history
!n
Ctrl-r
$HISTSIZE
$HISTFILE
$HISTFILESIZE
prevent recording a command
(optional)regular expressions
(optional) Korn shell history
practice: shell history
solution: shell history
17. file globbing
* asterisk
* ? question mark
* [] square brackets
* a-z and 0-9 ranges
* $LANG and square brackets
* preventing file globbing
* practice: shell globbing
* solution: shell globbing
* V. pipes and commands
* 18. I/O redirection
* stdin, stdout, and stderr
* output redirection
output file is erased
noclobber
overruling noclobber
>> append
>> error redirection
>> 2> stderr
>> 2>&1
>> output redirection and pipes
>> joining stdout and stderr
>> input redirection
>> < stdin
>> << here document
>> <<< here string
>> confusing redirection
>> quick file clear
>> practice: input/output redirection
>> solution: input/output redirection
>> 19. filters
>> cat
>> tee
>> grep
>> cut
>> tr
>> wc
>> sort
>> uniq
>> comm
>> od
>> sed
>> pipe examples
>> who | wc
>> who | cut | sort
>> grep | cut
>> practice: filters
>> solution: filters
>> 20. basic Unix tools
>> find
>> locate
>> date
>> cal
>> sleep
>> time
>> gzip - gunzip
>> zcat - zmore
>> bzip2 - bunzip2
>> bzcat - bzmore
>> practice: basic Unix tools
>> solution: basic Unix tools
>> 21. regular expressions
>> regex versions
>> grep
>> print lines matching a pattern
>> concatenating characters
>> one or the other
>> one or more
>> match the end of a string
>> match the start of a string
>> separating words
>> grep features
>> preventing shell expansion of a regex
>> rename
>> the rename command
>> perl
>> well known syntax
>> a global replace
>> case insensitive replace
>> renaming extensions
>> sed
>> stream editor
>> interactive editor
>> simple back referencing
>> back referencing
>> a dot for any character
>> multiple back referencing
>> white space
>> optional occurrence
>> exactly n times
>> between n and m times
>> bash history
>> VI. vi
>> 22. Introduction to vi
>> command mode and insert mode
>> start typing (a A i I o O)
>> replace and delete a character (r x X)
>> undo and repeat (u .)
>> cut, copy and paste a line (dd yy p P)
>> cut, copy and paste lines (3dd 2yy)
>> start and end of a line (0 or ^ and $)
>> join two lines (J) and more
>> words (w b)
>> save (or not) and exit (:w :q :q! )
>> Searching (/ ?)
>> replace all ( :1,$ s/foo/bar/g )
>> reading files (:r :r !cmd)
>> text buffers
>> multiple files
>> abbreviations
>> key mappings
>> setting options
>> practice: vi(m)
>> solution: vi(m)
>> VII. scripting
>> 23. scripting introduction
>> prerequisites
>> hello world
>> she-bang
>> comment
>> variables
>> sourcing a script
>> troubleshooting a script
>> prevent setuid root spoofing
>> practice: introduction to scripting
>> solution: introduction to scripting
>> 24. scripting loops
>> test [ ]
>> if then else
>> if then elif
>> for loop
>> while loop
>> until loop
>> practice: scripting tests and loops
>> solution: scripting tests and loops
>> 25. scripting parameters
>> script parameters
>> shift through parameters
>> runtime input
>> sourcing a config file
>> get script options with getopts
>> get shell options with shopt
>> practice: parameters and options
>> solution: parameters and options
>> 26. more scripting
>> eval
>> (( ))
>> let
>> case
>> shell functions
>> practice : more scripting
>> solution : more scripting
>> VIII. local user management
>> 27. introduction to users
>> whoami
>> who
>> who am i
>> w
>> id
>> su to another user
>> su to root
>> su as root
>> su - $username
>> su -
>> run a program as another user
>> visudo
>> sudo su -
>> sudo logging
>> practice: introduction to users
>> solution: introduction to users
>> 28. user management
>> user management
>> /etc/passwd
>> root
>> useradd
>> /etc/default/useradd
>> userdel
>> usermod
>> creating home directories
>> /etc/skel/
>> deleting home directories
>> login shell
>> chsh
>> practice: user management
>> solution: user management
>> 29. user passwords
>> passwd
>> shadow file
>> encryption with passwd
>> encryption with openssl
>> encryption with crypt
>> /etc/login.defs
>> chage
>> disabling a password
>> editing local files
>> practice: user passwords
>> solution: user passwords
>> 30. user profiles
>> system profile
>> ~/.bash_profile
>> ~/.bash_login
>> ~/.profile
>> ~/.bashrc
>> ~/.bash_logout
>> Debian overview
>> RHEL5 overview
>> practice: user profiles
>> solution: user profiles
>> 31. groups
>> groupadd
>> group file
>> groups
>> usermod
>> groupmod
>> groupdel
>> gpasswd
>> newgrp
>> vigr
>> practice: groups
>> solution: groups
>> IX. file security
>> 32. standard file permissions
>> file ownership
>> user owner and group owner
>> listing user accounts
>> chgrp
>> chown
>> list of special files
>> permissions
>> rwx
>> three sets of rwx
>> permission examples
>> setting permissions (chmod)
>> setting octal permissions
>> umask
>> mkdir -m
>> cp -p
>> practice: standard file permissions
>> solution: standard file permissions
>> 33. advanced file permissions
>> sticky bit on directory
>> setgid bit on directory
>> setgid and setuid on regular files
>> setuid on sudo
>> practice: sticky, setuid and setgid bits
>> solution: sticky, setuid and setgid bits
>> 34. access control lists
>> acl in /etc/fstab
>> getfacl
>> setfacl
>> remove an acl entry
>> remove the complete acl
>> the acl mask
>> eiciel
>> 35. file links
>> inodes
>> inode contents
>> inode table
>> inode number
>> inode and file contents
>> about directories
>> a directory is a table
>> . and ..
>> hard links
>> creating hard links
>> finding hard links
>> symbolic links
>> removing links
>> practice : links
>> solution : links
>> X. Appendices
>> A. keyboard settings
>> about keyboard layout
>> X Keyboard Layout
>> shell keyboard layout
>> B. hardware
>> buses
>> about buses
>> /proc/bus
>> /usr/sbin/lsusb
>> /var/lib/usbutils/usb.ids
>> /usr/sbin/lspci
>> interrupts
>> about interrupts
>> /proc/interrupts
>> dmesg
>> io ports
>> about io ports
>> /proc/ioports
>> dma
>> about dma
>> /proc/dma
>> C. License
