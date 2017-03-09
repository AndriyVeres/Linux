#Users and groups
Each user have UID (user identifier), for simple users takes from pool: 500...1000 (basically).

 _UID 0 – root users (administrator)._
_ UID logged in system logs, for determination which user is did what._


##Text interface, 1..6 virtual consoles minimum, can configure greater.

**Ctrl+Alt+F1**
**Ctrl+Alt+… **        
**Ctrl+Alt+F6**

_ttyN N FN  number of virtual console, getty utility convert terminal (black screen) to usefull terminal_

**Ctrl+Alt+F8**


##Graaphics consoles
**Ctrl+Alt+F7**
**Ctrl+Alt+F8 **        
**Ctrl+Alt+F9**

###Ctrl+Alt+F12 ?  
_Console that show all logs of system?_



###passwd 
_change password utilite_

**autologin**
 _autologin utilite, all users will be logged how one user, recommended only, when host work without internet connection and all fuiles and folders must have public access _

###who       
_all users logged_
###whoami 
_output user login_
###who am i 
_output user login_
###who -m 
_output user login_
###last    
_all users, including logged off in last time_

###logout
_logout from consoles_
###shutdown
_shutdown the machine_

###Ctrl+D   
_equivalent to logout, that talks to bash, that in input stream is nothing will be prompted_


	###man [object]  
_manual of all, structured like pages manual_
	###info [object]  
_hypertext-based manual, but for not all Linux objects, is wrote info_

###whatis [object]   
_searching in NAME columns in manuals [object]_
###apropos [object] 
_searching everywhere in manuals [object]_

###whatis intro 
_manuals sections (basically 9)._

_[object] command, system calls e.t.c._

###echo Hello, world!      
_output in console text Hello, world!_
###echo “Hello, world! “  
_output in console text Hello, world!_
###date     
_date_
###cal      
_calendar_


###repeat all, that input in console
###cat
###Any test
###Any test    
###Ctrl+D

###keys
	who -m      //one letter key
	who --me   //multi letter key
	who –help

###-o 
_often output to standard output_

###type  [command]  
_type of command_
###type  - a [command]  
_type of command in all variants_
###type -t [command] 
 _type type of command_
###Ctrl+C  
_equivalent, bat say to bash cancel activity of bash_

###ls -i   
_show index deskriptor_

##HARDLINK

_ln file file-hardlink_

###SYMBOLIC LINK

###ln -s 
_file file-symlink_
###realpath file-symlink      
_real path of file-symlink_


##MULTITHREADING

###ps -f
_full information about processes, launched_
###ps -h 
_show process list hierarhically_



	cat > [filename]   
	//some text to file
	^D
*write to file*


	sh loop&   launch process in background mode
	top        // system resources utility
	fg         //move last background process to foreground mode
	^Z         //stop propcess without deleting from PID table
	bg         //move last stopped process to background


##SIGNALS

*  **9 **   (KILL)
*  **19**  (SТОР)
*  **18**  (CONТ
*  **2**    (INT)


	sh   //new shell process


	date > tmpfile  
**transfer from standard console output to file tmpfile, excluding error standard output**

	chmod +/-{r,w,X} file 

**change access mode for file read, write, execute**

	рwd            //print working directory



