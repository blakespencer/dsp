# Learn command line

Please follow and complete the free online [Bash Scripting Tutorial](https://ryanstutorials.net/bash-scripting-tutorial/) or [Codecademy's Learn the Command Line](https://www.codecademy.com/learn/learn-the-command-line). These are helpful tutorials. You should be able to go through these in a couple of hours.

**Note:** Bash is not installed on a PC. Rather, PC users must install Cygwin. Once Cygwin has been installed, the command line interface witll _emulate_ bash. You can find all information regarding Cygwin [here](https://www.cygwin.com/).

---

### Q1. Cheat Sheet of Commands

Here's a list of items with which you should be familiar:

- show current working directory path
- creating a directory
- deleting a directory
- creating a file using `touch` command
- deleting a file
- renaming a file
- listing hidden files
- copying a file from one directory to another

Make a cheat sheet for yourself: a list of at least **ten** commands and what they do. (Use the 8 items above and add a couple of your own.)

- **pdw** prints working directory
- **mkdir directory_name** makes a new directory
- **rm -rf directory_name** removes a directory and recursively removes all sub folders
- **touch file_1** creates a new file
- **mv file_1 path_to_file** moves a file, can also be used to rename a file
- **cp file_name** copies the file
- **ls -a** listed all files including hidden
- **echo string_variable** prints to the terminal

---

### Q2. List Files in Unix

What do the following commands do:

- `ls` lists all visible folders
- `ls -a` lists all existing folders
- `ls -l` lists the long format
- `ls -lh` lists long format as well as file sizes
- `ls -lah` prints all files in long format with sizes
- `ls -t` lists files in order from newest to oldest
- `ls -Glp`lists long format with a / and colour codes

---

### Q3. More List Files in Unix

Explore these other [ls options](http://www.techonthenet.com/unix/basic/ls.php) and pick 5 of your favorites:

- `ls -a`
- `ls -G`
- `ls -h`
- `ls -x`
- `ls -p`

---

### Q4. Xargs

What does `xargs` do? Give an example of how to use it.

> > Apply a given command to a series of things in order.
> > For example: if there is a command that outputs more than one thing, we can use xargs to apply some command to each output
