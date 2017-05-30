# Learn command line

Please follow and complete the free online [Command Line Crash Course
tutorial](https://web.archive.org/web/20160708171659/http://cli.learncodethehardway.org/book/) or [Codecademy's Learn the Command Line](https://www.codecademy.com/learn/learn-the-command-line). These are helpful tutorials. Each "chapter" focuses on a command. Type the commands you see in the _Do This_ section, and read the _You Learned This_ section. Move on to the next chapter. You should be able to go through these in a couple of hours.

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

Command | Action
------------ | -------------
`pwd` | show current working directory path
`mkdir [dir]` | creating a directory
`rm -r [dir]` | deleting a directory
`touch [file]` | creating a file using `touch` command
`rm -i [file]` | deleting a file
`mv [file] [newfilename]` | renaming a file
`ls -a` | listing hidden files
`cp [file] [dir]` | copying a file from one directory to another
`open [file]` | opening a file
`sudo [command]` | running a command with the security privileges of the superuser (Super User DO)

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

Command | Action
------------ | -------------
`ls` | short listing
`ls -a` | listing including hidden files
`ls -l` | long listing
`ls -lh` | long listing with human-readable file sizes
`ls -lah` | long listing with human-readable file sizes including hidden files
`ls -t` | listing sorted by time modified (most recently modified first) before sorting the operands by lexicographical order.
`ls -Glp` | long listing with colorized output where directories end with '/'

---

### Q3.  More List Files in Unix  

Explore these other [ls options](http://www.techonthenet.com/unix/basic/ls.php) and pick 5 of your favorites:

1. `ls -m`
2. `ls -d`
3. `ls -u`
4. `ls -g`
5. `ls -c`

---

### Q4.  Xargs   

What does `xargs` do? Give an example of how to use it.

`xargs` runs commands on the output from other command line programs. You can force `xargs` to use at most `max-args` arguments per command line. For example, the following will use the first two arguments per command:
```console
$ echo 1 2 3 4 | xargs -n 2
```

 

