## Overview

The Simple Shell is a Unix-like shell implemented in C. It supports the execution of both built-in and external commands, manages command history, and allows for command pipelining using pipes (|).
Features
- Command Execution: Execute external commands using execvp, as well as built-in commands like cd and history.
- History Management: Maintain a history of up to 100 commands, with options to view and clear history.
- Pipelining: Support for command pipelining, enabling the execution of commands in sequence with data passed between them.
- Robust Memory Management: Ensures proper allocation and deallocation of memory to prevent leaks.

## Built-In Commands:

Change the current directory to < directory >.
~~~
cd <directory>
~~~
Display the list of commands entered during the session.
~~~
history
~~~
Clear the command history.
~~~
history -c
~~~
Exit the shell.
~~~
exit
~~~

## Usage

To compile the Simple Shell, use the following command:
~~~
gcc -o sish sish.c -lpthread
~~~

To start the Simple Shell, simply run the compiled executable:
~~~
./sish
~~~
### Entering Commands:
- Type commands as you would in a standard Unix shell.
- Use pipes (|) to chain commands together.
- Use the history command to view the command history.
- Use the exit command to quit the shell.
