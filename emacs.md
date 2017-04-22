## EMACS

### LAUNCH

### emacs
>*launch emacs, if graphical view abaliable, emacs will be launched in graphical mode*

### emacs -nw
>*launch emacs in terminal*

### c-h h
>*say "hello" in different languages*

### C-x C-c
>*exit*

## SHORTCUT COMMANDS

### C-h ?
.*help commands*

### C-h t
>*Tutorials for beginners*

### C-h i
>*full info-styled help*

## NAME COMMANDS

### M-x
>*call a command without keyboyard shortcut*

### M-x help-for-help
>*help for help*

## WORKING WITH FILES

>*scratch - special buffer, that use for temporary bookmarks, it will be clean after emacs closing*

### Dired mode
>*You can also work with catalogues, like with strings in file, for activating dired mode, you need open a catalogue, like open file*

### C-x C-f
>*open file*

### C-x C-s
>*Save file*

## WORKING WITH TEXT

### C-a
>*move to string beginning*

### C-e
>*move to string end*

### M-<
>*move to beginning of buffer (working text space)

### M->
>*move to end of buffer (working text space)

### M-a
>*move to beginning of sentence*

### M-e
>*move to end of sentence*

### M-f
>*move forward to next word*

### M-b
>*move backward to previous word*

### M-{
>*move to beginning of paragraph*

### M-}
>*move to end of paragraph*

### M-Del
>*delete last word*

### C-x Del
>*delete last sentence*

### M-d
>*delete forward word*

### M-k
>*delete forward sentence*

### C-y
>*insert, last deleted text*

### M-y
>*use previous deleted texts, like in stack*

### C-t
>*swap two digits around the coursor*

### M-t
>*swap two words around the coursor, without punctuation*

### C-x C-t
>*swap two strings around the coursor*

## ORPHOGRAPHY

### M-x ispell-buffer
>*orphography check program*

### M-x flyspell-mode
>*marking online wrong-wroted words*

### M-x $
>*check word, close to coursor*

### M-x Tab
>*end word, according to vocabulary*

### M-x replace-string [what replace] Enter [what will be inserted]
>*replace string in all buffer*

### M-x replace-regexp [what replace] Enter [waht will be inserted]
>*replace string according to regular expression*

### M-%
>*replace strings side by side*

### C-M-%
>*replace strings side by side*

### C-_
>*undo*

## TEXT CLUSTERS

>*Text cluster located inside area, that creates in space with mark and coursor*

### C-Space
>*set/unset mark*

### C-w
>*delete cluster*

### M-w
>*copy cluster*

### C-y
>*insert cluster*

### M-@
>*set mark in the end of next word*

### M-h
>*mark current paragrpah*

### C-x h
>*mark whole buffer*

### C-u C-@
>*previous position of mark*

### C-x r Space x
>*write coursor position to regixter X*

### C-x r j x
>*move coursor to position, that wrote in register X*

### C-x r s x
>*copy text cluster to register X*

### C-x r i x
>*paste text cluster from register X*

## CONFIGURATIONAL FILES

>*.emacsrc*


## SEARCHING

>*In emacs presents several type of searching (register independent):

* Searching string.

* Regular expression-based searching.


### C-s
>*Stackable searching*

### C-r
>*Stackable searching in order to beginning of buffer*

### C-M-s
>*Stackable regular expression-based searching*
