# 0x02. Shell, I/O Redirections and filters
## Introduction
* This project is part of the ALX SE program projects. It is meant to test one's understanding of the Shell and Shell permissions.
## Learning Objectives
* At the end of this project, you are expected to be able to **explain to anyone**, *without the help of Google*
### Shell, I/O Redirection
* What do the commands **head**, **tail**, **find**, **wc**, **sort**, **uniq**, **grep**, **tr** do
* How to redirect standard output to a file
* How to get standard input from a file instead of the keyboard
* How to set the output from one program to the input of another program
* How to combine commands and filters with redirections
### Special Characters
* What are special characters
* Understand behaviour, how and when to use;
   * white spaces, single quotes, double quotes, backslash, comment, pipe, command seperator, tilde
### Other Man pages
* How to display a line of text
* How to concatenate files and print on the standard output
* How to reverse a string
* How to remove sections from each line of files
* What is the **/etc/passwd** file and what is its format
* What is the **/etc/shadow** file and what is its format
## Tasks

### 0. My name is Betty
Create a script that switches the current user to the user **betty**.
   * You should use exactly 8 characters for your command (+1 character\\
	 for the new line)
   * You can assume that the user **betty** will exist when the script is\\
   run
```
julien@ubuntu:/tmp/h$ tail -1 0-iam_betty | wc -c
9
julien@ubuntu:/tmp/h$
```
#### Repo:
* GitHub repository: **alx-system_engineering-devops**
* Directory: **0x01-shell_permissions**
* File: **0-iam_betty**

### 1. Who am I
Write a script that prints the effective username of the current user.
```
julien@ubuntu:/tmp/h$ ./1-who_am_i
julien
julien@ubuntu:/tmp/h$
```
#### Repo:
* GitHub repository: **alx-system_engineering-devops**
* Directory: **0x01-shell_permissions**
* File: **1-who_am_i**

### 2. Groups
Write a script that prints all the groups that the current user is part of.
```
julien@ubuntu:/tmp/h$ ./2-groups
julien adm cdrom sudo dip plugdev lpadmin sambashare
julien@ubuntu:/tmp/h$
```
Note: depending on the user, the output will be different
#### Repo:
* GitHub repository: **alx-system_engineering-devops**
* Directory: **0x01-shell_permissions**
* File: **2-groups**

### 3. New owner
Write a script that changes the owner of the file **hello** to the user\\
**betty**.
```
julien@ubuntu:/tmp/h$ ls -l
total 4
-rwxrw-r-- 1 julien julien 30 Sep 20 14:23 3-new_owner
-rw-rw-r-- 1 julien julien  0 Sep 20 14:18 hello
julien@ubuntu:/tmp/h$ sudo ./3-new_owner 
julien@ubuntu:/tmp/h$ ls -l
total 4
-rwxrw-r-- 1 julien julien 30 Sep 20 14:23 3-new_owner
-rw-rw-r-- 1 betty  julien  0 Sep 20 14:18 hello
julien@ubuntu:/tmp/h$
```
#### Repo:
* GitHub repository: **alx-system_engineering-devops**
* Directory: **0x01-shell_permissions**
* File: **3-new_owner**

### 4. Empty!
Write a scipt that creates an empty file called **hellO**.
#### Repo:
* GitHub repository: **alx-system_engineering-devops**
* Directory: **0x01-shell_permissions**
* File: **4-empty**

### 5. Execute
Write a script that adds execute permissions to the owner of the file\\
**hello**.
   * The file **hello** will be in the working directory
```
julien@ubuntu:/tmp/h$ ls -l
total 8
-rwxrw-r-- 1 julien julien 28 Sep 20 14:26 5-execute
-rw-rw-r-- 1 julien julien 23 Sep 20 14:25 hello
julien@ubuntu:/tmp/h$ ./hello
bash: ./hello: Permission denied
julien@ubuntu:/tmp/h$ ./5-execute 
julien@ubuntu:/tmp/h$ ls -l
total 8
-rwxrw-r-- 1 julien julien 28 Sep 20 14:26 5-execute
-rwxrw-r-- 1 julien julien 23 Sep 20 14:25 hello
julien@ubuntu:/tmp/h$
```
#### Repo:
* GitHub repository: **alx-system_engineering-devops**
* Directory: **0x01-shell_permissions**
* File: **5-execute**

### 6. Multiple permissions
Write a script that adds execute permissions to the owner and the group\\
owner, and the read permission to other users, to the file **hello**.
   * The file **hello** will be in the working directory
```
julien@ubuntu:/tmp/h$ ls -l
total 8
-rwxrw-r-- 1 julien julien 36 Sep 20 14:31 6-multiple_permissions
-r--r----- 1 julien julien 23 Sep 20 14:25 hello
julien@ubuntu:/tmp/h$ ./6-multiple_permissions 
julien@ubuntu:/tmp/h$ ls -l
total 8
-rwxrw-r-- 1 julien julien 36 Sep 20 14:31 6-multiple_permissions
-r-xr-xr-- 1 julien julien 23 Sep 20 14:25 hello
julien@ubuntu:/tmp/h$
```
#### Repo:
* GitHub repository: **alx-system_engineering-devops**
* Directory: **0x01-shell_permissions**
* File: **6-multiple_permissions**
