# Learn command line

Please follow and complete the free online [Bash Scripting Tutorial](https://ryanstutorials.net/bash-scripting-tutorial/) or [Codecademy's Learn the Command Line](https://www.codecademy.com/learn/learn-the-command-line). These are helpful tutorials. You should be able to go through these in a couple of hours.

**Note:** Bash is not installed on a PC. Rather, PC users must install Cygwin. Once Cygwin has been installed, the command line interface witll _emulate_ bash. You can find all information regarding Cygwin [here](https://www.cygwin.com/).

---

### Q1.  Cheat Sheet of Commands  

Here's a list of items with which you should be familiar:  
* show current working directory path
* creating a directory
* deleting a directory
* creating a file using `touch` command
* deleting a file
* renaming a file
* listing hidden files
* copying a file from one directory to another

Make a cheat sheet for yourself: a list of at least **ten** commands and what they do.  (Use the 8 items above and add a couple of your own.)  

> > pwd; mkdir path; rm -r path; touch fname; rm fname; mv old fname new fname; ls -ld .?*; cp fname dir; cd dir; ls
---

### Q2.  List Files in Unix   

What do the following commands do:  
`ls`  
`ls -a`  
`ls -l`  
`ls -lh`  
`ls -lah`  
`ls -t`  
`ls -Glp`  

> >
list all visible contents of current directory
list all contents, incl. hidden, of current directory
list all contents of curr dir in long form
lists size of all visible folders/files
lists size of all visible and hidden folders/files
lists all contents by date of last edit
lists contents and counts of files

---

### Q3.  More List Files in Unix  

Explore these other [ls options](http://www.techonthenet.com/unix/basic/ls.php) and pick 5 of your favorites:

> > ls -u shows files by access time
    ls -F flags file names
    ls -R shows sub-directories
    ls -m shows contents as comma separated
    ls -p shows directories with "/"
---

### Q4.  Xargs   

What does `xargs` do? Give an example of how to use it.

> > xargs executes a specific command once for each specified argument passed
xargs can be used to perform a command on all files or directories that meet a specified condition. For example, find all files that contain a certain string, and remove them

 

