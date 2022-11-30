# 0x00. Shell, basics
## Introduction
This project is part of the many ALX SE projects. It is mennt to test one's understanding of the following Shell basics
## Learning Objectives
At the end of this project, one is expected to be explain to anyone, **without the use of Google these objectives**
### General
* What does RTFM mean?
* What is a Shebang
### What is the Shell
* What is the shell
* What is the difference between a terminal and a shell
* What is the shell prompt
* How to use the history (the basics)
### Navigation
* What do the commands or built-ins **cd**, **pwd**, **ls** do
* How to navigate the filesystem
* What are the **.** and **..** directories
* What is the working directory, how to print it and how to change it
* What is the root directory
* What is the home directory, and how to go there
* What is the difference between the root directory and the home directory of the user root
* What are the characteristics of hidden files and how to list them
* What does the command **cd -** do
### Looking Around
* What do the commands **ls**, **less**, **file** do
* How do you use options and arguments with commands
* Understand the ls long format and how to display it
* [A Guided Tour](http://linuxcommand.org/lc3_lts0040.php)
* What does the **ln** command do
* What do you find in the most common/important directories
* What is a symbolic link
* What is a hard link
* What is the difference between a hard link and a symbolic link
### Manipulating Files
* What do the commands **cp**, **mv**, **rm**, **mkdir** do
* What are wildcards and how do they work
* How to use wildcards
### Working with Commands
* What do **type**, **which**, **help**, **man** commands do
* What are the different kinds of commands
* What is an alias
* When do you use the command help instead of man
### Reading Man Pages
* How to read a man page
* What are man pages sections
* What are the section numbers for User commands, System calls and Library functions
### Keyboard Shortcuts for Bash
* Common shortcuts for Bash
### LTS
* What does **LTS** mean?

## Tasks
### 0. Where am I?
* Write a script that prints the absolute path name of the current working directory

Example:
```
$ ./0-current_working_directory
/root/alx-system_engineering-devops/0x00-shell_basics
$
```

### Repo:
* GitHub repository: **alx-system_engineering-devops**
* Directory: **0x00-shell_basics**
* File: **0-current_working_directory**

### 1. What's in there?
* Display the contents list of your current directory

Example
```
$ ./1-listit
Applications    Documents    Dropbox Movies Pictures
Desktop Downloads    Library Music Public
$
```

### Repo:
tHub repository: **alx-system_engineering-devops**
* Directory: **0x00-shell_basics**
* File: **1-listit**

### 2. There is no place like home
* Write a script that changes the working directory to the user's home directory.
   * Note: Shell variables are not allowed

Example
```
julien@ubuntu:/tmp$ pwd
/tmp
julien@ubuntu:/tmp$ echo $HOME
/home/julien
julien@ubuntu:/tmp$ source ./2-bring_me_home
julien@ubuntu:~$ pwd
/home/julien
julien@ubuntu:~$
```

### Repo:
* GitHub repository: **alx-system_engineering-devops**
* Directory: **0x00-shell_basics**
* File: **2-bring_me_home**

### 3. The long format
* Write a script that displays current directory contents in a long format

Example:
```
$ ./3-listfiles
total 32
-rwxr-xr-x@ 1 sylvain staff 18 Jan 25 00:19 0-current_working_directory
-rwxr-xr-x@ 1 sylvain staff 19 Jan 25 00:23 1-listit
-rwxr-xr-x@ 1 sylvain staff 18 Jan 25 00:29 2-bring_me_home
-rwxr-xr-x@ 1 sylvain staff 18 Jan 25 00:39 3-listfiles
$
```

### Repo:
* GitHub repository: **alx-system_engineering-devops**
* Directory: **0x00-shell_basics**
* File: **3-listfiles**

### 4. Hidden files
* Write a script that displays current directory contents, including hidden files (Starting with **.**). Using the **long format**

Example:
```
$ ./4-listmorefiles
total 32
drwxr-xr-x@ 6 sylvain staff 204 Jan 25 00:29 .
drwxr-xr-x@ 43 sylvain staff 1462 Jan 25 00:19 ..
-rwxr-xr-x@ 1 sylvain staff 18 Jan 25 00:19 0-current_working_directory
-rwxr-xr-x@ 1 sylvain staff 19 Jan 25 00:23 1-listit
-rwxr-xr-x@ 1 sylvain staff 18 Jan 25 00:29 2-bring_me_home
-rwxr-xr-x@ 1 sylvain staff 18 Jan 25 00:39 3-listfiles
-rwxr-xr-x@ 1 sylvain staff 18 Jan 25 00:41 4-listmorefiles
$
```

### Repo:
* GitHub repository: **alx-system_engineering-devops**
* Directory: **0x00-shell_basics**
* File: **4-listmorefiles**

### 5. I love numbers
* Write a script that displays current directory content in
   * Long format
   * with user and group IDs displayed numerically
   * And hidden files (Starting with **.**)

Example:
```
$ ./5-listfilesdigitonly
total 32
drwxr-xr-x@ 6 501 20 204 Jan 25 00:29 .
drwxr-xr-x@ 43 501 20 1462 Jan 25 00:19 ..
-rwxr-xr-x@ 1 501 20 18 Jan 25 00:19 0-current_working_directory
-rwxr-xr-x@ 1 501 20 18 Jan 25 00:23 1-listfiles
-rwxr-xr-x@ 1 501 20 19 Jan 25 00:29 2-bring_me_home
-rwxr-xr-x@ 1 501 20 20 Jan 25 00:39 3-listfiles
-rwxr-xr-x@ 1 501 20 18 Jan 25 00:41 4-listmorefiles
-rwxr-xr-x@ 1 501 20 18 Jan 25 00:43 5-listfilesdigitonly
$
```

### Repo:
* GitHub repository: **alx-system_engineering-devops**
* Directory: **0x00-shell_basics**
* File: **5-listfilesdigitonly**

### 6. Welcome
* Create a script that creates a directory named **my_first_directory** in the **/tmp** directory.

Example:
```
$ ./6-firstdirectory
$ file /tmp/my_first_directory/
/tmp/my_first_directory/: directory
$
```

### Repo:
* GitHub repository: **alx-system_engineering-devops**
* Directory: **0x00-shell_basics**
* File: **6-firstdirectory**
