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
* command to become a superuser
* temporarily move to another directory
* return to original directory before pushing to temporary directory
* copy entire directory with its subfolders and files

Make a cheat sheet for yourself: a list of at least **ten** commands and what they do.  (Use the 8 items above and add a couple of your own.)

**Answers:**

* `pwd`
* `mkdir`
* `touch` <name_of_file>
* `rm` <name_of_file>
* `mv` <old_name_of_file> <new_name_of_file>
* `ls -a`
* `cp` <name_of_file/directory path> <optional_new_name/new directory path>
* `sudo`
* `pushd` <directory_path>
* `popd`
* `cp -r` <directory> <new_directory_name>

---

### Q2.  List Files in Unix   

What do the following commands do:  
`ls` - lists files and directories in the current directory.
`ls -a`  - same as above but shows hidden files.
`ls -l`  - long format of list. gives total cumulative file size and read/write permissions
`ls -lh`  - gives size of files/directories
`ls -lah` - same as above but includes hidden files
`ls -t` - lists file in order of last modified
`ls -Glp`  - list files using color in longform and puts a / after those filenames that are directories

---

### Q3.  More List Files in Unix  

Explore these other [ls options](http://www.techonthenet.com/unix/basic/ls.php) and pick 5 of your favorites:

* `ls -R` -- displays all subdirectories! Careful not to do this in the home directory as it will run for a long time.
* `ls -a` -- great to see hidden files, could be the reason you cannot remove a directory with rmdir
* `ls -t` -- great to see which files were modified last.
* `ls -G` -- great for a bit of color in the terminal
* `ls` -- for a quick snapshot of your current wd.

---

### Q4.  Xargs   

What does `xargs` do? Give an example of how to use it.

* xargs executes a command on a bunch of items in order. Suppose someone is fired from a company, you then wish to find all of their files, and then delete them. The xargs command lets you run the find command and then execute the deletes of these found files. This is easier that writing a bash script or doing a loop!

> An example : ```bash
seq 5 | xargs -n 1 echo "The count is: "
```

 

