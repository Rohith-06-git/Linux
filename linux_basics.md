# Linux Basics

## What I Learned

Today I learned how to navigate and work with the Linux filesystem using basic terminal commands.

## Key Commands

- `pwd` — shows the current working directory
- `ls` — lists files and directories
- `cd` — changes the current directory
- `mkdir` — creates a directory
- `touch` — creates a file
- `cat` — displays file contents
- `cat -n` — displays file contents with line numbers
- `less` — views large files one screen at a time
- `cp` — copies files
- `mv` — moves or renames files
- `rm` — removes files
- `rmdir` — removes empty directories

## Important Concepts

- `.` represents the current directory.
- `..` represents the parent directory.
- `~` represents the home directory.
- `/` represents the root directory.

## File Permissions

Linux permissions control who can read, write, or execute a file.

### Permission Types

- `r` — read
- `w` — write
- `x` — execute

### Permission Commands

- `ls -l` — view file permissions
- `chmod` — change file permissions

### Examples

```bash
ls -l test.txt

chmod 644 test.txt

chmod 600 test.txt

## Relative Paths

- `./` represents the current directory.
- `../` represents the parent directory.

### Using `./` and `../` with Files

```bash
vim ./file.txt

## User Management

Linux allows multiple users to have separate accounts and permissions.

### User Commands

- `whoami` — shows the current logged-in user
- `adduser` — creates a new user
- `passwd` — sets or changes a user's password
- `su` — switches to another user

### Creating a User

```bash
sudo adduser rohith

## Modifying Users

The `usermod` command is used to modify an existing Linux user account.

### Adding a User to the Sudo Group

A normal user can be given administrative privileges by adding them to the `sudo` group.

```bash
sudo usermod -aG sudo rohith