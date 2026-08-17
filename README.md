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

## Day 1

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

## Day 2 — File Permissions

Linux permissions control who can read, write, or execute a file.

### Permission Commands

- `ls -l` — view file permissions
- `chmod` — change file permissions
- `chown` — change file ownership

### Permission Types

- `r` — read
- `w` — write
- `x` — execute

### Example

```bash
ls -l
chmod +x script.sh
chmod 644 file.txt