## Table of Contents
* [Description](#description)
* [File Structure](#file-structure)
* [Requirements](#requirements)
* [Installation](#installation)
* [Usage](#usage)
* [Authors](#authors)


## Description
simple\_shell is a command line interpreter. The shell has a prompt($) and it is displayed again each time a command has been executed.
This is a project made for the ALX software engineering program, project 0x16. C - Simple Shell.

## File Structure
| File Name | Description and contents |
| --- | --- |
| [man\_1\_simple\_shell](man_1_simple_shell) | This is the manpage for the simple\_shell, where we can find examples and the correct syntax of the commands.|
| [shell.h](shell.h) |This is the header file with the struct and prototypes of the functions.|
| [shell.c](shell.c) |main function - Prints the prompt in a loop and calls the functions to accept arguments and executes the command.|
| [AUTHORS](AUTHORS) |List of contributors to this repository.|
| [\_dollar\_special.c](_dollar_special.c) |the function - Returns the address at which EXIT_CODE is stored and Sets the value for EXIT_CODE var.|
| [\_get\_history\_lines\_count.c](_get_history_lines_count.c) |the function - Counts the lines in a previo and Returns the lines count of history file.|
| [\_getenv.c](_getenv.c) |the function - Returns a pointer to a env var value.|
| [\_handle\_var\_replacement.c](_handle_var_replacement.c) |the function - Handles dollar vars '$'.|
| [\_help.c](_help.c) |the function - print a line of fd.|
| [\_history.c](_history.c) |the function - Return the address of history head.|
| [\_own\_memory.c](_own_memory.c) |the function - Reallocates a memory block.|
| [\_puts.c](_puts.c) |the function - Prints a string to stdout.|
| [\_strcpy.c](_strcpy.c) |the function - Copies the string source to destination.|
| [\_strncpy.c](_strncpy.c) |the function - Copies n amount of string.|
| [\_strtok.c](_strtok.c) |the function - Divides a string into tokens.|
| [\_write\_history.c](_write_history.c) |the function - Writes the history to a file in home dir.|
| [alias\_list.c](alias_list.c) |the function - Checks if the alias input is meant to set an alias.|
| [builtin\_utils.c](builtin_utils.c) |the function - Validates a env var name.|
| [builtins.c](builtins.cc) |the functions - Prints the environment variables to stdout, Sets or adds an environment variable and Removes an evironment variable.|
| [f\_command_handlers.c](f_command_handlers.c) |the functions - Buidls an array of strings as arguments, Counts the number of arguments in a command string, Checks if the command to execute could be found in PATH's dirs and Creates a string representing a full path to file.|
| [f\_error.c](f_error.c) |the function - Dispatches an error.|
| [f\_exit.c](f_exit.c) |the function - Checks if the user entered the exit command.|
| [f\_handle\_builtins.c](f_handle_builtins.c) |the function - Executes the builtin funtions in case the command is one.|
| [f\_handle\_comment.c](f_handle_comment.c) |the function - deletes a comment from the buffer.|
| [f\_handle\_enter.c](f_handle_enter.c) |the function - Check if no command was entered.|
| [f\_handle\_shell\_logical\_operators.c](f_handle_shell_logical_operators.c) |the function - Handle semicolon and logical op, Handles || and && logical part execute the commands.|
| [f\_linked\_lists.c](f_linked_lists.c) |the function - Print the lists and add a new node at the end.|
| [f\_memory.c](f_memory.c) |the function - Manages the memory allocation.|
| [f\_special.c](f_special.c) |the function - Builds the "env vars" array using dynamic memory.|
| [f\_strings.c](f_strings.c) |the function - copy a strings with a malloc, Convert a number to string format and returns the length of a string.|
| [f\_strings\_creation.c](f_strings_creation.c) |the function - concatenates string substract a paragraph.|
| [f\_strings2.c](f_strings2.c) |the function -  for string scanning operation.|


## Requirements

simple\_shell is designed to run in the `Ubuntu 20.04 LTS` linux environment and to be compiled using `gcc` with flags`-Wall -Werror -Wextra -pedantic -std=gnu89`

## Installation

   - Clone this repository: `git clone "https://github.com/MikiyasA/simple_shell.git"`
   - Change directories into the repository: `cd simple_shell`
   - Compile: `gcc -Wall -Werror -Wextra -pedantic -std=gnu89 *.c -o hsh`
   - Run the shell in interactive mode: `./hsh`

## Usage

The simple\_shell is designed to execute commands with given arguments in a way discribed below.
The shell tokenizes written commands into words using " " as a delimiter and the first word is considered as the command and all remaining words as arguments. The command will be searched either in the list of shell builtins or in the elements of the PATH environmental variable and if successful, the shell executes the command with given arguments.  (see man page for complete information on usage):


## Authors
Benroy Kirwa | [GitHub] (https://github.com/BenroyKirwa)

Mikiyas Adere | [GitHub] (https://github.com/MikiyasA/)