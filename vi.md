## Vi
*vi works with buffer buffer save in swap file wrom this file you can reestablish unsaved file*

### i
>*insert mode*

### O
>*insert mode from a new string*

### o
>*insert mode from a previous string*

### I
>*insert from a string beginning*

### a
>*insert mode after cursor position*

### A
>*insert mode in a end of string*

### ESC
>*command mode, in some cases need type ESC 2 times*

### :set wrap
>*long strings transfer mode ON*

### :set nowrap
>*long strings transfer mode OFF*

### :w
>*write file*

### ^C
>*force exit from a inputted command in vi, but not forced exit from vi*

### :q
>*exit*

### :x
>*exit*

### :q!
>*exit without saving*

### :wq
>*exit with saving*

### 0
>*move coursor to beggining fo the current string*  

### ^
>*move coursor to first non-space symbol*

### $
>*move coursor to end of string*
 
### {
>*move to beginning of paragraph*

### }
>*move to end of paragrqaph*
>*paragraph in vi - text fragments, separated by empty string*

### g
>*move to end of file*

### gg
>*move to beginning

### w
>*move to beginning of next word*

### b
>*move to beginning of previous word* 

### (
>*move to beginning of previous sentence, according to regular expression*

### )
>*move to beginning of next sentence, according to regular expression*

### 3w
>*move to 3 words forward, multiplier also works for another vi commamds*

### /{key_word}
>*searching in a text elements by  ccording to key_word, you can navigate by using * - next, # - previous* 

### x
>*delete current symbol*

### dd
>*delete whole string*

### :center
>*move current string to center, you can also move whole text (see regular expressions)*

### :left
>*move current string to left border, you can also move whole text (see regular expressions)*

### :right
>*move current string to right border, you can also move whole text (see regular expressions)*

### u
>*undo*

### )
>*cluster identifyer, it means, that you can apply command till end the sentence (dot or empty string), 
you can combine cluster command with another commands, for example: d), c) e.t.c.*

### cw
>*change word*

### y
>*yank (copy) command*

### p
>*paste deleted cluster by using d, c, x,or copied (yank command) usefull for mooving text parts*

### :{begin line number},{end line number}command
>*execute command without substitution the coursor in a need position in text*

### .
>* identifyer of current string*


## VIM

### ^p
>*search previous similar word, see (:help ins-completion)*

### ^n
>*search next similar word, see (:help ins-completion)*

## SETTING AND CONFIGURATIONAL FILES

### :set {option}
>*change option in a command line mode*

### .exrc
>*Vi config*

### .vimrc
>*VIM config*

### :options
>*see settings, ONLY FOR VIM*