# My-Shell

# Introduction

This repository contains my C code for making a Shell from scratch.

# How to Run
compile the myproject.c file in the bash using-  
`gcc -o shell myproject.c` then `./shell`

# Working
Shell is basically a loop: it repeatedly prints a prompt , parses the input, executes the command specified on that line of input, and waits for the command to finish. This is repeated until the user types `"quit"` or ends their input.  

The fork() system call creates a new process. After this point, two processes will be executing within your code. You will be able to differentiate the child from the parent by looking at the return value of fork; the child sees a 0, the parent sees the pid of the child. For this project, we are using `execvp()`.If `execvp()` is successful, it will not return; if it does return, there was an error (e.g., the command does not exist).  

To implement `cd` command `chdir()` in-built C function has been used.

# Feature added by me

Feature of checking the `history`, which I implemented by storing the previously performed commands in an array.It will show upto last 10 commmands given to the shell.

It also contains the original feature of repeating last performed command by giving input- `!!`

# Example
![acm project](https://user-images.githubusercontent.com/67902213/109394608-e49eff00-794d-11eb-9673-000f3d2d259b.png)
![acm project 1](https://user-images.githubusercontent.com/67902213/109394724-727aea00-794e-11eb-86fc-8c7e37a16464.png)
