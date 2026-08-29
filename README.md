# Starting Linux

My Linux learning journey for Data Engineering.

## Topics

- Linux basics
- File system
- Permissions
- Processes
- Networking
- Shell scripting

## Learning Approach

Learn → Practice → Document → Commit

---

## Day 0 — Linux Fundamentals

- Linux is built around the Linux kernel.
- Ubuntu is a Linux distribution.
- Bash is a shell.
- The terminal is an interface used to interact with the shell.
- The shell interprets commands and interacts with the operating system.

---

## Day 1 — Linux Basics

Started learning Linux basics and terminal commands.

### Navigation Commands

- `pwd` — print current working directory
- `ls` — list files and directories
- `cd` — change directory

### File and Directory Commands

- `mkdir` — create a directory
- `touch` — create a file
- `rm` — remove a file
- `rmdir` — remove an empty directory

### File Operations

- `cp` — copy a file
- `mv` — move or rename a file
- `cat` — display file contents
- `echo` — print text

### Redirection

- `>` — write or overwrite file contents
- `>>` — append content to a file

### File Viewing

- `head` — display the beginning of a file
- `tail` — display the end of a file

### Useful Concepts

- `.` — current directory
- `..` — parent directory
- `~` — home directory
- `/` — root directory

### Command Structure

Most Linux commands follow this pattern:

`command [options] [arguments]`

Example:

`ls -l /home`

- `ls` — command
- `-l` — option
- `/home` — argument

## Practice

```bash
pwd
ls
cd ..

mkdir test
touch file.txt
rm file.txt
rmdir test

touch file1.txt
echo "Hello Linux" > file1.txt
cat file1.txt

cp file1.txt file2.txt
mv file2.txt renamed.txt

echo "Second line" >> renamed.txt

head renamed.txt
tail renamed.txt

rm file1.txt renamed.txt

### Getting Help

Linux provides built-in help for commands.

- `man` — opens the manual page for a command
- `command --help` — shows basic usage and options

Examples:

```bash

man ls
ls --help

```
### Command History
- `history` — shows previously executed commands
- `clear` — clears the terminal screen
- `Ctrl + L` — clears the terminal screen

Examples:
```bash
history
clear