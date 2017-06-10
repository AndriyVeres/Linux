# Users and groups
>Each user have UID (user identifier), for simple users takes from pool: 500...1000 >(basically).

>*UID 0 – root users (administrator).*
>*UID logged in system logs, for determination which user is did what.*


### Text interface, 1..6 virtual consoles minimum, (can configure greater).

### Ctrl+Alt+{F1...F6}


>*ttyN N FN  number of virtual console, getty utility convert terminal (black screen) to usefull terminal*

**Ctrl+Alt+F8**

### Graphics consoles

* **Ctrl+Alt+F7**
* **Ctrl+Alt+F8**        
* **Ctrl+Alt+F9**

### Ctrl+Alt+F12 
>*Console that show all logs of system*

### passwd 
>*change password utilite*

### autologin
>*autologin utilite, all users will be logged how one user, recommended only, when host work without internet connection and all fuiles and folders must have public access*

### who       
>*all users logged*

### whoami 
>*output user login*

### who am i 
>*output user login*

### who -m 
>*output user login*

### last    
>*all users, including logged off in last time*

### su 
>*shell of users can launch shell command from a  specific user name*

### sudo 
>*can run a only defined commands from a specific user name*

### logout
>*logout from consoles*

### shutdown
>*shutdown the machine*

### Ctrl+D   
>*equivalent to logout, that talks to bash, that in input stream is nothing will be prompted*

### man [object]  
>*manual of all, structured like pages manual*

### info [object]  
>*hypertext-based manual, but for not all Linux objects wrote info*

### whatis [object]   
_searching in NAME columns in manuals [object]_

### apropos [object] 
>*searching everywhere in manuals [object]*
>*[object] command, system calls e.t.c.*

### whatis intro 
>*manuals sections (basically 9).*


### echo Hello, world!      
>*output in console text Hello, world!*

### echo “Hello, world! “  
>*output in console text Hello, world!*

### date     
>*date*

### cal      
>*calendar*

	cat
	Any test
	Any test    
	Ctrl+D
>*repeat all, that input in console*

### keys

#### who -m      
>*one letter key*

#### who --me

#### who --help   
>*multi letter key*
	
#### -o 
>*often output to standard output*

### type  [command]  
>*type of command*

### type  - a [command]  
>*type of command in all variants*

### type -t [command] 
>*type type of command*

### Ctrl+C  
>*equivalent, bat say to bash cancel activity of bash*

### ls -i   
>*show index deskriptor*

## HARDLINK

### ln [target_file] [file-hardnlink] 
>*file-hardlink*

## SYMBOLIC LINK

### ln -s [target_file] [file-symlink]
>*file file-symlink* 

### realpath [file-symlink]      
>*real path of file-symlink*


## MULTITHREADING

### ps -f
>*full information about processes, launched*

### ps -h 
>*show process list hierarhically*

### ps -ef
>*
	cat > [filename]   
	//some text to file
	^D
>*write to file*


### sh loop&   
>*launch process in background mode*

### top        
>*system resources utility*

### vmstat
>*virtual memory statistics*

### fg         
>*move last background process to foreground mode*

### Ctrl+Z         
>*stop propcess without deleting from PID table*

### bg         
>*move last stopped process to background*

### /var/run
>*file, where located PIDs of processes*


## SIGNALS

*    9   (KILL)
*  19   (SТОР)
*  18   (CONТ)
*    2   (INT)


### sh   
>*new shell process*


### date > tmpfile  
>*transfer from standard console output to file tmpfile, excluding error standard output*

### chmod +/-{r,w,X} file 
>*change access mode for file read, write, execute*

### рwd           
>*print working directory*


## UTILITES
 
### find    
>*search for files in a directory hierarchy*

### cmp
>*compare two files byte by byte*

### wc      
>*word count*

### head    
>*search from a beginning of file*

### tail    
>*search from a end of file*

### cut
> *search something in a each line*

### tr      
>*transliteration tool: change letter A to another symbol, or delete some letters*

### sed     
>*stream editor for filtering and transforming text*

### sort    
>*sorting a text*

### xargs   
>*biuld and execute command lines from standard input*

### \enter  
>*continue to editing a command in a new command line*

### chroot
>*utilite for testing services, that can run command in some catalogue, like utilite will be think like non-root catalogue - root catalogue*

### visudo
>*change sudoers file*

### useradd
>*add user*

### usermod
>*modify user account*

### userdel
>*delete user*

### groupadd
>*add group*

### groupmod
>*change group*

### gruopdel
>*delete group*

### patch
>*apply a diff file to an original*

## FILES

### chown 
>*change file owner and group*

### stmpclean
>*utilite for cleaning /tmp*

### locate
>*find files by name*

### hexdump             
>*show non-text files in ASCI HEX format*

>**-C [file]**      
>*show in right part symbols from left part, non printed symbols will be replaced to dots*

### file | less  
>*scrolling*

### strings              
>*show in non-text file parts that can be text*

## SHARED CATALOGUES

	drwxr-xr-t  6 [group] [owner]      [size] [date] [time] [name]
>*t in the end means that catalogue - shared it means, that only owner of catalogue can*
>*change the all files in catalogue, another users can manage only files, that consist to them*
>*if need read-only shared catalogue, in the end will be T*

## DEDCRIPTORS AND STREAMS
>*Deskriptors are named like 0,1,2,3,4,5...e.t.c. It used for access to files, streams e.t.c. in Linux.*

>*In Linux already open 3 descriptors:*

* **0**	(stdin) - standard input stream.
* **1**	(stdout) - standard output stream.
* **2** (stderr) - standard error stream.

### command > [file]  
>*move data from stdout (printout of command to file)*

### command < [file]  
>*give a text data to a program, that launched by command from file string by string*

### command 2> [file] 
>*move data from stderr (standard error stream) to file*

### /dev/null   
>*file-gap, you can move all streams to this file, data wrom which you don`t need, data will be deleted*

### bind -l
>*list of all bash functions of readline library, readline  conigurational file inputrc, that*
>*file consist of the next commands: "manage keyboyard sequence": function*

### bind -p
>*list of all sequences, that linked to readline functions*

### tput
>*utilite that works with TERM variable, and terminfo database can manage keyboyard sequence for all*
>*terminfo*


## CAPABILITIES OF TERMINAL AND CONTROL CHARACTERS

### ^W
>*Delete word*

### ^U
>*Delete string*

### ^R
>*Search in history of entered commands, need to type search key after ^R*
>*The next suitable variant of command, according to search key can show also by using ^R*
>*history of entered command stored in .bash_history file*

### stty -a
>*Change and print terminal line settings*

### ^S
>*Stop showing info on terminal*

### ^Q
>*Continue showing info on terminal*

### ^V
>*Don`t use the next control character as control character*

### ^J
>*Symbol of ending a string equivalent to enter*

### ^J stty sane ^J
>*Help reset terminal to some default values*

### reset
>*Reset terminal according to system configuration, that stored in /etc/inittab*

### ^P
>*Go to previous entered command, equivalent to key up arrow*

### ^N
>*Go to next entered command, equivalent to key down arrow*

### sleep
>*delay in terminal*


## ALIASES

### alias
>*show already defined aliases for user*

### unalias shortkey
>*remove shortkey from aliases*

 

## WORKING WITH CATALOGUES
 

### pushd [catalogue]

>*push into stack new catalogue*

### pupd [catalogue]
>*remove from stack last added new catalogue, adn go to this catalogue*

### dirs
>*show catalogues stack*

### type tab on keyboyard
>*Completion*

### basename [catalogue]
>*show in terminal catalogue name*

### ^G
>*beeper*

## TEMPLATES

>**

### Variables
>*A=dit*
>*B=dash*
>*C="$A $B*
>*will be output ditdash*

### ?
>*Use for returning an exit status.*
>*You can show the prorgam returning status by using echo $?*

### test
>*check file types and compare values*

## GRUB

Grand Unified Bootloader, have:

* Boot sector on disk with map of placement.

* Stage 1.5 - special intermediate bootloader (drivers of one special filesystem).

* Second bootloader.

### /boot/grub/
>*GRUB catalogue

### /etc/default/grub
>*grub configurational file*

## KERNEL

Kernel and start virtual disk archived by using gzip utilite, kernel can own unpack

### /dev/kmem
>*kernel memory, where directly save information about all processes, that kernel manage*

### dmesg
>*kernel launching log*

### lsmod
>*list of loaded kernel modules*

### insmod
>*load kernel module in to kernel*

### rmmod
>*unload kernel module from kernel*

### mkinitrd
>*assembly start virtual disk*

### /boot
>*catalogue, that have all need images, kernel also, for boot*

### init
>*father of all processes (excluding kernel processes), by default located in **/sbin/init** *
>*/etc/init/ folder have configurational skripts, what do, when init lauch (in ubuntu miss inittab)*


## START SKRIPTS

>in older Linux version organization of launching start scenario was in a dedicated file, but this solution was not so good, in case of logic of launching (you need for example launch one deamon after another), also, when user install new module he need every time add start skripts of module to file, so it was not usable, in help, developers of Linux brings **.d-scheme,** it means, that in catalogue **/etc/ with new [module],** with configuration file **/etc/[module].conf** will be added new catalogue **/etc/[module].d**, for providing boot order, for skripts, inside rc.d catalogue, files inside named with using two digits, and order will provide by numbers of this digits (from lower to higher), also this files - symlink to skripts (that actually launch modules), that stored in **/etc/init.d/** catalogue. K-letter in beggining means kill process, S - start, when you change runlevels, for example from wih networking to without networking, network processes will be ended, and after ending will be started another, specific to next run level modules, if not need to change status of module, when You change run levels, skript willn`t execute.

### /etc/rc.d/init.d
>*folder with start skripts*
### or
### etc/init.d
>*for compatibility with UNIX in some distributives*

### [skript] start
>*launch skript*

### [skript] stop
>*stop skript*

>*[scenario] full path to skript in /etc/rc.d/*

### service [module] start
>*launch kernel module (the same like in previous case) by utilite service*

### service [module] stop
>*stop kernel module (the same like in previous case) by utilite service*

## START SKRIPTS.RUN LEVELS

Run level - type of launching the system, profile of system launch
In Linux present several types of run levels (depends on distributive):

* Level 0: System stop.

* Level 1: Mono-user mode, one terminal, without deamons.

* level 2: Multi-user mode, without networking.

* Level 3: Multi-user mode, with networking.

* Level 4: User-defined.

* Level 5: Graphical multi-suer mode.

* Level 6: Restart.

* Level 7: User-defined.

* Level 8: User-defined.

* Level 9: User-defined.

### init [level]
>*change run level*

### runlevel
>*current run level, locate in __/sbin/runlevel__ *
>*default runlevel presents in __/etc/inittab file__

>*In Ubuntu presents systemd manager, thats why in Ubuntu miss inittab, where You can change default run level, for Ubuntu need to use __update-rc.d__ utilite or __sysv-rc-conf__   or __rcconf__* 

## DEVICES

> In linux presents two types of devices naming:
* Static - file holes many in /dev, stable using.
* Dynamic - file holes not many in /dev, user-friendly for human, but need to check inconsistencies, use virtual file system.

>File-hole - named pipe, vs file-pipe, has a name.
>All file-holes saved in */dev/* catalogue.

### /dev/null
>*real black hole, in this lace all wrote will be not saved*

### /dev/urandom or /dev/random 
>*random digits generator*

### /dev/zero
>*source of zeros*

File-holes doesn`t have an size, they have vs size two id:
*  1 digit (major device number) - driver type*
*  2 digit (minor device number) - access type (for disc-types - section).*

There are several types of file-holes:
* minor device number b - block type, access by block transmittion, block devices can suppert direct access, like write block number 5 e.t.c.
* minor device number c - character type, acess by byte transmittion
* fifo-channel - (named pipe), any program can write to fifo and another program in the same moment can read wrom fifo.
* socket - open for two users: server,that open socket first, any time listen for any messages, process massages, if they come, and responce to them; client, connect to socket, listn socket, send messages, process responces. 

### mkfifo
>*make fifo*

### lspci
>*list of all PCI-compatible devices*

### fdisk
>*program for working with disk partitions*

## WORKING WITH DISK

### mount
>*mount device or disk partition for colaboration if file system*
### umount
>*unmount device or disk partition*

### fsck
>*utilite for checking and repairing Linux file system*

### sync
>*synchronize cached data to persistent storage, if you need immidiately writing process without buffer (will decrese device lifecycle)*

### etc/fstab
>*configurational file, when saved settings for devices mounting after system startup*

### updfstab
>*utilite, that change /etc/fstab file*


## VIRTUAL FILESYSTEM

### ROOMFS or TMPFS
>*start virtual drive*

###PROCFS
>*processes, see /proc/*

### devpts
>*use for terminals emulators*

### NFS
>*network file system*

### LUFS
>*linux userland file system - use for organizing file system, that use information from linux processes, FTP, SSH clients,access to NTFS with vine e.t.c.*

## CONFIGURATIONAL FILES AND SYSTEM PROFILES

In Linux for solving different problems and tasks use several types of system solutions.
* Solution - special distributive, or software, that can solve dedicated problem, if user requirements not sppecific, in most cases solution will be usefull: see films, process sheets, work with e-mail.
* Realization + system profile - constructor, that use software and deamons (realization) with deskription of them interaction (system profile), user can combine different modules, that solve problem by splitting it to subproblems (mini tasks, that element of realization can solve: text sorting, http server, e-mail server e.t.c), and deskribe interaction logic by using profile. For managing profile use CONFIGURATIONAL FILES.

A lot of configurational files can also be customized by using /home directory of each user, in this directory customization configurational files use hidden formats: .[file]

Can organized through the folowing way:

* .d-scheme, i.e. different files for different profiles (like startup profiles).
* layered files - core config - have settings for standard configuration, second, third files use core file by default, and can combine changed settings from core file in the third files, modified, so You can change default settings.
* sectionizing of config - in configurational files split settings to groups, according to parts of profile.

>Often configurational files  commented  in the  own  file, a principle called SELF-DESCRIPTIVE CONFIGURATIONAL FILE.

### Configurational files for some utilites and deamons:

### .vim
>*group of files /usr/share/vim*

### man dircolors
>*ls colors configuration*

<<<<<<< HEAD
### wvdial
>*config ~/.wvdialrc - utilite for dial up*

### man
>*/etc/manpath.config*

### updfstab
>*configurational file /etc/updfstab.conf*

### /usr/share/doc/{service}/examples
>*often examples of configs are putted here*

### users
>*/etc/passwd  and /etc/group*


## SYSTEM LOGS

Managed by syslogd deamon, which have /etc/syslog.d configurational file.
If a program need save in system some event it can do it by two ways:
* Write in opened by syslogd file event info. Usefull in cases when mennasges - not text, or it will be a lot, so syslogd will be overloaded - specific cases.
* Use system call syslog(), which re-address message to syslogd. Most of the cases.

In a previous version of Debian and Ubuntu cofigurational file of syslogd was located in **/etc/syslog.conf**  now it migrated to **/etc/rsyslog.d/50-default.conf**.

All messages clasified horizontally (facility) (from which service) and vertically (priority).

### man logger
>*Facility and priority types description*

In configurational files presents two fields: 
* Facility.Priority
* Logging file


In configurational file can be presents * symbol - that means any, or none, that means no one.

System logs stored in /var/log/messages and another archives, that in order to filling delete, from messages.1 to messages.n, i.e. scrolling method, when oldest logs gradually moves from messages.1 to messages.n and delete.

### logrotate
>*utilite that rotates, comress and mails system logs*
>*have a /etc/logrotate.d catalogue and /etc/logrotate.conf configurational file*

## SCHEDULED ACTIONS

Managed by cron utilite, that have */etc/crontab* cobfigurational file.
Fields are named:
* Minute
* Hour
* Day of month
* month of year
* day of week
* user
* commands

>Symbol * means that field not active.

In commands usually presents commands for execution files from .d-scheme, whene located sorted in alphabetic (numbers have higher priority, than letters).

Also, because computer can be swithed off in time, when cron need to do some tasks, there is presents additional deamon: anacron (asynchronous cron), that do unfulfilled tasks, in possible time, without high load to system, configurational file */etc/anacrontab*.

User can add his own scenario with the same syntax, but user field must be empty.

### crontab -e
>*editing the crontab*

## PACKAGE MANAGEMENT

In Linux install, update, remove programs, services and utilites can be do with package help.
Package - tool for manipulating of program/utilite/service source code, binary, libraries, configurational and another files, for easy do install, update, remove.
All files need to be installed package to archive.
Archive - tree of files, which can be managed like a one file.

### tar
>*utilite for archiving and unzipping arcchives, becomes eralier than Linuix, from UNIX, presents in any UNIX-compatible OS, mean "tape archiver".

Package have an archive and some another components, so .tar format not usefull for package place, so it was dedicated some specific formats (in this files archives included):
* .rpm - managed by rpm utilite: Red Hat packet manager.
* .deb - managed by dpkg utilite: debian binary package format.

Because a lot of packages has a relatives to another packages, installation of one program maybe will take a long time, bacause a user need to install another packages with primary, because primary use them like resources, and another of another packages, because them use them like resources e.t.c. For helping user in installation process was developed package managers, most popular - APT: Advanced Package Tool.

### apt-cache seacrh
>*search a package*

### apt-get install
>*install package*

### apt-get remove
>*remove package*

>User can use VIRTUAL PACKAGE for installing to new OS software list, versus installing one by one components of list.

### /etc/apt/sources.list
>*list of repositories, that use apt, after changing lists need update apt cache by typing  apt-get update*

### apt-get update
>*update cache after updating repositories list*

### apt-get source
>*copy only package from repository*

### apt-cdrom add
>*add repository from cdrom, when user need install software from cdrom*

### apt-get dist-upgrade
>*upgrade whole distributive with packages*

## TCP/IP NETWORKING

Linux allows see ip-networks transmission on differents OSI-levels.

### ip
>*show, manipulate, configure routing, devices, policy routing and tunnels*

### ip link
>*network device configuration on interface level*

### ip link show
>*show list of network interfaces*

### ip address show
>*show list of ip-adresses*

### ip neighbour show
>*show ARP-table (Address Resolution Protocol), MAC-adresses i one subnetwork*

### ping
>*send ICMP packets*

### ifconfig
>*iterface configuration old utilite, ip more powered*

### ip route show
>*show routing table*
>*default means defailt route - exit to external network with mask 0, if default route not configured, you can`t send packets to external network*

### arp
>*show arp table old utilite, ip use the same functionality*

### iptables
>*packet filtering and NAT*

### traceroute
>*define the trace route to address*

### tcpdump
>*dump traffic on a network*

### tcpdump -pi {interface}
>*dump traffic on interface*

### /etc/services
>*list of all application protocoles, and ports, that they use*

### netstat -antu
>*print information about network connections*

### telnet {address} {port}
>*usefull to check if server provide service on port, but not for remote connection to server*

### netcat
>*ntework cat utilite*

### inetd
>*internet server*

### /etc/hosts
### /etc/hosts.conf
### /etc/resolvconf
>*list of domain names of hosts*

### host
### dig
>*DNS loockup utility*


>Loopback address use for transfering packets from computer hisself.

>MTU - maximum tranfer unit, maximum allowed unit for transmission over interface.

>FF:...:FF - hardware broadcast MAC-address, use, when  MAC-adress of subscriber unknown. 





## GRAPHICAL INTERFACE X11

Address of server for addressing from X-clients (visual programs) stored in variable DISPLAY

### startx
>*start X11 session*

### X
>*start X-server*

### /etc/X11
>*graphical subsystem profile*


### editres
>*see tree of X-objects, that application use*

### xrdb
>*X server resource database utility*