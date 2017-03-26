#Users and groups
>Each user have UID (user identifier), for simple users takes from pool: 500...1000 >(basically).

>*UID 0 – root users (administrator).*
>*UID logged in system logs, for determination which user is did what.*


###Text interface, 1..6 virtual consoles minimum, (can configure greater).

###Ctrl+Alt+{F1...F6}


>*ttyN N FN  number of virtual console, getty utility convert terminal (black screen) to usefull terminal*

**Ctrl+Alt+F8**

###Graphics consoles

* **Ctrl+Alt+F7**
* **Ctrl+Alt+F8**        
* **Ctrl+Alt+F9**

###Ctrl+Alt+F12 
>*Console that show all logs of system*

###passwd 
>*change password utilite*

###autologin
>*autologin utilite, all users will be logged how one user, recommended only, when host work without internet connection and all fuiles and folders must have public access*

###who       
>*all users logged*

###whoami 
>*output user login*

###who am i 
>*output user login*

###who -m 
>*output user login*

###last    
>*all users, including logged off in last time*

###su 
>*shell of users can launch shell command from a  specific user name*

###sudo 
>*can run a only defined commands from a specific user name*

###logout
>*logout from consoles*

###shutdown
>*shutdown the machine*

###Ctrl+D   
>*equivalent to logout, that talks to bash, that in input stream is nothing will be prompted*

###man [object]  
>*manual of all, structured like pages manual*

###info [object]  
>*hypertext-based manual, but for not all Linux objects wrote info*

###whatis [object]   
_searching in NAME columns in manuals [object]_

###apropos [object] 
>*searching everywhere in manuals [object]*
>*[object] command, system calls e.t.c.*

###whatis intro 
>*manuals sections (basically 9).*


###echo Hello, world!      
>*output in console text Hello, world!*

###echo “Hello, world! “  
>*output in console text Hello, world!*

###date     
>*date*

###cal      
>*calendar*

	cat
	Any test
	Any test    
	Ctrl+D
>*repeat all, that input in console*

###keys

####who -m      
>*one letter key*

####who --me

####who --help   
>*multi letter key*
	
####-o 
>*often output to standard output*

###type  [command]  
>*type of command*

###type  - a [command]  
>*type of command in all variants*

###type -t [command] 
>*type type of command*

###Ctrl+C  
>*equivalent, bat say to bash cancel activity of bash*

###ls -i   
>*show index deskriptor*

##HARDLINK

###ln [target_file] [file-hardnlink] 
>*file-hardlink*

##SYMBOLIC LINK

###ln -s [target_file] [file-symlink]
>*file file-symlink* 

###realpath [file-symlink]      
>*real path of file-symlink*


##MULTITHREADING

###ps -f
>*full information about processes, launched*

###ps -h 
>*show process list hierarhically*



	cat > [filename]   
	//some text to file
	^D
>*write to file*


###sh loop&   
>*launch process in background mode*

###top        
>*system resources utility*

###fg         
>*move last background process to foreground mode*

###Ctrl+Z         
>*stop propcess without deleting from PID table*

###bg         
>*move last stopped process to background*


##SIGNALS

*    9   (KILL)
*  19   (SТОР)
*  18   (CONТ)
*    2   (INT)


###sh   
>*new shell process*


###date > tmpfile  
>*transfer from standard console output to file tmpfile, excluding error standard output*

###chmod +/-{r,w,X} file 
>*change access mode for file read, write, execute*

###рwd           
>*print working directory*


##UTILITES
 
###find    
>*search for files in a directory hierarchy*

###wc      
>*word count*

###head    
>*search from a beginning of file*

###tail    
>*search from a end of file*

###cut
> *search something in a each line*

###tr      
>*transliteration tool: change letter A to another symbol, or delete some letters*

###sed     
>*stream editor for filtering and transforming text*

###sort    
>*sorting a text*

###xargs   
>*biuld and execute command lines from standard input*

###\enter  
>*continue to editing a command in a new command line*

##FILES

###chown 
>*change file owner and group*

###hexdump             
>*show non-text files in ASCI HEX format*

>**-C [file]**      
>*show in right part symbols from left part, non printed symbols will be replaced to dots*

###file | less  
>*scrolling*

###strings              
>*show in non-text file parts that can be text*

##SHARED CATALOGUES

	drwxr-xr-t  6 [group] [owner]      [size] [date] [time] [name]
>*t in the end means that catalogue - shared it means, that only owner of catalogue can*
>*change the all files in catalogue, another users can manage only files, that consist to them*
>*if need read-only shared catalogue, in the end will be T*

##Descriptors and streams
>*Deskriptors are named like 0,1,2,3,4,5...e.t.c. It used for access to files, streams e.t.c. in Linux.*

>*In Linux already open 3 descriptors:*

* **0**	(stdin) - standard input stream.
* **1**	(stdout) - standard output stream.
* **2** (stderr) - standard error stream.

###command > [file]  
>*move data from stdout (printout of command to file)*

###command < [file]  
>*give a text data to a program, that launched by command from file string by string*

###command 2> [file] 
>*move data from stderr (standard error stream) to file*

###/dev/null   
>*file-gap, you can move all streams to this file, data wrom which you don`t need, data will be deleted*