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

## FILES

### chown 
>*change file owner and group*

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


##VIRTUAL FILESYSTEM

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

### .vimrc
>*vim configurational file*

### man dircolors
>*ls colors configuration*
