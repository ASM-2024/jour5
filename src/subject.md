---
title: "-1sh"
author: paul.lege
logo: https://avatars.githubusercontent.com/u/96961500?s=200&v=4
---
# Introduction
In this mini-project you will have to implement a small command executer, a few standard commands and an interactive prompt to use these commands.

# -1SH

You will write a program named -1SH, wich will read a line from a standard input (stdin), split it on the spaces, then execute the corresponding command.

## Standard commands

You will have to implement some commands for your -1SH. If an error occurs while a command is executed, you must display the relevant error message (err.h/errno.h) on the stderr.
For every command you must to refer to its man page.

### Cat

Cat print on the standard output the content of each file passed as an argument, without any separator.
You must handle -e parameter.
If there is an error, stop the processing of the arguments.

### Echo

Echo print on the standard output given argumen as is, followed by a newline character

### Head

head prints on the standard output the first 10 lines of the given files. In the case where is more than one file to read, head will display the name of the read file before its content. If there is an error, stop the processing of the arguments.

### Quit

The quit command will stop the execution of you -1SH correctly. Don't forget free everything. The return code has to be the same than the one of the last executed command. If no one was executed return 0.

### &&

And operator must be handle. You must execute the left command before the right. If the left command fail, you don't have to run the right.

### ||

Or operator must be handle. As the and operator you must execute the left command before the right. If the left succed, you don't have to run the right.

### ()

The priority of parentheses operators must be handled

# Working in group
For this project you must work in group of 2-4 persons, you should create a git repos on the cri gitlab.

# Tips

For this project you check the shunting yard algorithm and the reverse polish notation. They will help you to handle && and || operator.
