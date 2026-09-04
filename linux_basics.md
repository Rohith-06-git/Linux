## What I Learned

Today I learned how to navigate and work with the Linux filesystem using basic terminal commands.

### Key Commands

- `pwd` — shows the current working directory
- `ls` — lists files and directories
- `cd` — changes the current directory
- `mkdir` — creates a directory
- `touch` — creates a file
- `cat` — displays file contents
- `cp` — copies files
- `mv` — moves or renames files
- `rm` — removes files
- `rmdir` — removes empty directories

### Important Concepts

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

### Permission Command

- `ls -l` — view file permissions
- `chmod` — change file permissions

### Examples

```bash
ls -l test.txt
chmod 644 test.txt
chmod 600 test.txt

## Nested Directories

The `mkdir -p` command can create directories and subdirectories at once.

### Example

```bash
mkdir -p my/folder/one