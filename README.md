# Linux-Shell-Scripting

## Project Review

Linux shell scripting is a powerful tool that automates repetitive tasks, enhances system administration, and improves workflow efficiency. 
A shell script is a text file containing a series of commands that the shell executes sequentially. These scripts can automate tasks such as file manipulation, system monitoring, and software deployment, improving efficiency and reliability.

## What is Shell Scripting

Shell scripting is the process of writing and executing of series of instructions in a sheel to automate a task. Shell script is basically a scrip or program written in a shell language such as bash, sh, zsh or powershell.

## Shell Environments

The following are the everal shell environments are available in Linux, each with unique features:

Bash: This is the most commonly used shell, known for its scripting capabilities and backward compatibility with the Bourne shell.

Zsh: It is an extended version of Bash with improved customization and interactive features.

Ksh: This offers advanced scripting functionalities and performance improvements over Bash.

Fish: This focuses on usability with features like syntax highlighting and auto-suggestions.

## Example

A basic shell script to create multiple folders and muliple linux users at once

![alt text](/sh11.JPG)

## Shebang Line (#!/bin/bash)

This is usually at the beginning of every shell script which helps to specify the interpreter to execute the script. It is a special notation used in Unix-like operating system like Linux, to specify the interpreter that should execute the script. In this case, #!/bin/bash specificially indicates that the Bash shell should be used to interpret and execute the script.

Bash is one of the shell tool used to interpret script. If we wanted to use another shell tool like sh, shebang would be updated to #!/bin/sh.

/bin/bash: This is the absolute path to the Bash shell execuable. It tells the system to use he Bash interpreter locaed in the /bin/bash to execute the script.


## Project Taske 

### Step 1: Create a folder on an ubuntu and name it shell-scripting

'mkdir shell-scripting'

![alt text](/sh1.JPG)

### Step 2: Using vim editor, create a file called 'my_first_shell_script.sh'

'vim my_first_shell_script.sh'

![alt text](/sh11.JPG)

![alt text](/sh2.JPG)

### Step 3: Type the shell script given and save it

i = to activate the insert mode.

:wq = to save and exit vim.

![alt text](/sh2.JPG)

### Step 4: Open the shell-scripting directory to confirm the file created

'cd shell-scripting'

'ls -latr'

![alt text](/sh3.JPG)

## Permissions

The above image indicates the various permissions which are assigned to the file that is "-rw-r--r--". This means

- The owner of the file has read (r) and write (w) permissions.
- Members of the file group has read (r) permission.
- Other groups have read (r) permission.

However, none of the categories have the execute (x) permission o the file.

Normally to execute this file, you run the below script command 

'./my_first_shell_script.sh'

This will print permission denied because it doesn't have permission to execute (x).

The "./" prefix in the file indicates the command to locate the current directory.

- The dot (.) indicates the current directory.
- The slash (/) is a directory separator.

### Step 5: Add the execute permission for the 'owner' to be able to execute the shell script and run it.

'chmod +x my_first_shell_script.sh'

'./my_first_shell_script.sh'

![alt text](/sh4.JPG)

![alt text](/sh5.JPG)

![alt text](/sh6.JPG)

![alt text](/sh7.JPG)

### Step 6: Evaluate and ensure that 3 folders are created.

'ls'

![alt text](/sh8.JPG)

### Step 6: Evaluate and ensure that 3 users are created on linux server.

'id user1'

'id user2'

'id user3'

![alt text](/sh9.JPG)


## Variable Declaration and Initialization

In programming generally, not just shell scripting, variables are essential for creating dynamic and flexible programs.

In Linux shell scripting, variables store data and are declared without a datatype. Initialization assigns a value using = without spaces (e.g., var="Hello"). Use $var to reference it. Variables can be local or environmental (export VAR=value). Quoting prevents unintended expansion, ensuring proper handling of strings and special characters.

For example assign "John" as value to a variable "name".

'name="John"'

![alt text](/sh12.JPG)

## Retrieving value from a variable

After assigning a value to a variable, as shown in the example above where "John" was assigned to the variable "name", you can utilize his variable in various ways in he scrip or program. To retrieve the value from the variable, it is done by echoing on the console using the "echo command" in shell scripting.

For example to retrieve "John" from the name variable by typing the command below and executing it.

'echo $name'

![alt text](/sh10.JPG)

## Task

### Assign a value to a variable and print it

'name = "John"

'echo $name'

'echo My name is $name'

![alt text](/sh10.JPG)

