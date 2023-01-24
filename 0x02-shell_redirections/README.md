# 0x02. Shell, I/O Redirections and filters
## Introduction
* This project is part of the ALX SE program projects. It is meant to test one's understanding of the Shell and Shell IO redirections.
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

### 0. Hello World
Write a script that prints "Hello, World", followed by a new line to the standard output.
```
julien@ubuntu:/tmp/h$ ./0-hello_world 
Hello, World
julien@ubuntu:/tmp/h$ ./0-hello_world | cat -e
Hello, World$
julien@ubuntu:/tmp/h$
```
#### Repo:
* GitHub repository: **alx-system_engineering-devops**
* Directory: **0x02-shell_redirections**
* File: **0-hello_world**
