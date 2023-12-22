
# Simple Shell project




## Introduction

This shell project is a basic implementation that adheres to the specified requirements, including features such as interactive and non-interactive modes, process creation, file system navigation, and more.
## Description

This is a simple shell implementation for the Unix-like operating system, following the specifications outlined in the project requirements.


##  Compilation
Compile the shell using the following command:

gcc -Wall -Werror -Wextra -pedantic -std=gnu89 *.c -o hsh


## Authorized functions and system calls

all functions from string.h

access (man 2 access)

chdir (man 2 chdir)

close (man 2 close)

closedir (man 3 closedir)

execve (man 2 execve)

exit (man 3 exit)

_exit (man 2 _exit)

fflush (man 3 fflush)

fork (man 2 fork)

free (man 3 free)

getcwd (man 3 getcwd)

getline (man 3 getline)

getpid (man 2 getpid)

isatty (man 3 isatty)

kill (man 2 kill)

malloc (man 3 malloc)

open (man 2 open)

opendir (man 3 opendir)

perror (man 3 perror)

printf (man 3 printf)

fprintf (man 3 fprintf)

vfprintf (man 3 vfprintf)

sprintf (man 3 sprintf)

putchar (man 3 putchar)

read (man 2 read)

readdir (man 3 readdir)

signal (man 2 signal)

stat (__xstat) (man 2 stat)

lstat (__lxstat) (man 2 lstat)

fstat (__fxstat) (man 2 fstat)

strtok (man 3 strtok)

wait (man 2 wait)

waitpid (man 2 waitpid)

wait3 (man 2 wait3)

wait4 (man 2 wait4)

write (man 2 write)
## Requirements
The allowed editors are vi, vim, and emacs.

The files will be compiled on Ubuntu 20.04 LTS using gcc with the following options: -Wall -Werror -Wextra -pedantic -std=gnu89.

Every file in the project should end with a new line.

It is mandatory to have a README.md file at the root of the project folder.

The code should follow the Betty style and will be checked using betty-style.pl and betty-doc.pl.

Each file should contain no more than 5 functions.

The shell should not have any memory leaks


## Outpout

The program should produce identical output to  the sh (/bin/sh) program, including error messages. The only exception is when you display an error, the program name must be equivalent to  argv[0]




## Testing

The shell should work in interactive mode:
    
    $ ./hsh
    ($) /bin/ls
    hsh main.c shell.c
    ($)
    ($) exit
    $

In non interactive mode:

    $ echo "/bin/ls" | ./hsh
    hsh main.c shell.c test_ls_2
    $
    $ cat test_ls_2
    /bin/ls
    /bin/ls
    $
    $ cat test_ls_2 | ./hsh
    hsh main.c shell.c test_ls_2
    hsh main.c shell.c test_ls_2
    $

