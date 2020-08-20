# Simple Shell

## Description

This project consists of creating our own version of a simple shell which is capable of interacting directly with the user through commands, we
create a system that is capable of handling a path that is in charge
of detecting if the arguments entered by the user are found and then
executing them, differentiating what type they are, whether they are
built-in commands or not, to go through the forking process. which
immediately handles calls to the execv system, running according to
the process and finally exiting with exit or ^D.

## How To Install & Compile ##
To have this repository and its content, you must execute the following on
your terminal:
~~~
$ git clone https://github.com/AlisonQuinter17/simple_shell.git
$ cd simple_shell
$ ls
~~~

And execute the following in your terminal:
~~~
$ gcc -Wall -Werror -Wextra -pedantic *.c -o hsh
$ ./hsh
$ |
~~~

## Description Of The Files Contained. ##

| File  name   | Description   |
| ------------- |:-------------:|
| simple_shell.h | In this header file all the necessary libraries and function prototypes are stored, as well as the environ. |
| main_shell.c      | This file contains the main function of this shell, including the function in charge of handling signs. |
| read_tokenize.c    | Contains the function that reads the line of the standard input and the tokenizer function as well, which return their result to the main. |
| compare_execute.c    | In this file there is a function in charge of comparing if the tokens are built-in or belong to the PATH, executing them respectively. |
| cases_functions.c   | This file contains the semicolon function. |
| builtin_functions.c | Contains Built-in functions. |
| auxiliar_functions.c | It contains all the auxiliary functions that I need to carry out various processes. |
| control_errors.c | Contains the function in charge of the error outputs. |
| man_1_simple_shell   | Custom manual page for our basic shell.|
| AUTHORS   | In this file listing all individuals having contributed content to the repository.|

### Note ###
If you want to review the manual of our Simple Shell function you can execute
in your terminal:
~~~
$ man ./man_1_simple_shell
~~~

##### Examples #####
Here are some examples of how our simple shell works:

- $ /bin/ls
  + AUTHORS builtin_functions.c compare_execute.c main_shell.c README.md simple_shell.h  
    auxiliar_functions.c cases_functions.c control_errors.c LICENSE man_1_simple_shell read_tokenize.c
  $

- $ pwd
  + /home/alzheimeer/tmpalison/simple_shell

- $ env
  + LOGNAME=alison  
    LANGUAGE=en_US  
    COMPIZ_CONFIG_PROFILE=ubuntu  
    DESKTOP_SESSION=ubuntu  
    IM_CONFIG_PHASE=1  
    DEFAULTS_PATH=/usr/share/gconf/ubuntu.default.path  
    GDM_LANG=en_US  
    SHELL=/usr/bin/zsh  
    PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/games:/usr/local/games:/home/alzheimeer/.dotnet/tools  
    DISPLAY=:0

- $ cd [DIRECTORY]  
  $ pwd
  + /home/alzheimeer/tmpalison/simple_shell/[DIRECTORY]

- exit
  + ~/tmpalison/simple_shell on  master! ⌚ 22:18:55  
  $

## Environment ##
* Language: C
* OS: Ubuntu 14.04 LTS
* Compiler: gcc 4.8.4
* Style guidelines: [Betty style](https://github.com/holbertonschool/Betty/wiki)
and
[Betty-doc](https://github.com/holbertonschool/Betty/blob/master/betty-doc.pl)

## Authors

- Valeria Trujillo - vtrujillorodriguez70@gmail.com / https://twitter.com/@valtrurodriguez
- Alison Quintero - alisondanellaquintero@hotmail.com / https://twitter.com/AlisonQuinter17
