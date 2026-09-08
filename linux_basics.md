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

### Package Management and Services

Linux uses package managers to install and manage software.

### Installing Apache2

Apache2 is a web server that can be installed using `apt`.

```bash
sudo apt update
sudo apt install apache2

### Other Package Management Commands

#### Upgrade

`apt upgrade` upgrades installed packages to newer available versions.

```bash
sudo apt update
sudo apt upgrade

## Nginx

Nginx is a web server commonly used to handle HTTP requests and serve web applications.

It can also work as a reverse proxy between clients and backend applications.

Nginx maintains logs that can be useful for troubleshooting and debugging.

Important log files include:

- `/var/log/nginx/access.log` — records incoming requests.
- `/var/log/nginx/error.log` — records errors and problems.

### Key Learning

- Nginx is commonly used as a web server and reverse proxy.
- Nginx logs can help identify problems and troubleshoot issues.
- `access.log` contains request information.
- `error.log` contains error information.

### Installing Nginx

```bash
sudo apt install nginx

## Groups

Linux groups are used to organize users and manage permissions.

A user can belong to multiple groups. Groups make it easier to give the same permissions to multiple users.

### Creating a Group

```bash
sudo groupadd developers

### Changing Permissions with chmod

Permissions can be changed using symbolic notation with `chmod`.

The basic structure is:

```bash
chmod [who][operation][permission] file

## Numeric Permissions with chmod

Linux permissions can also be represented using numbers.

### Permission Values

- `r` — read — `4`
- `w` — write — `2`
- `x` — execute — `1`
- No permission — `0`

The values are added together to create a permission number.

### Examples

```text
r-- = 4
-w- = 2
--x = 1

rw- = 4 + 2 = 6
r-x = 4 + 1 = 5
rwx = 4 + 2 + 1 = 7

## Processes

A process is a running instance of a program.

Whenever we start a program or execute a command, Linux creates a process to perform that task.

Each process has a unique Process ID (PID).

Linux manages processes by allocating CPU, memory, and other system resources to them.

Processes can run in the foreground or background.

### Key Learning

- A process is a running program.
- Each process has a unique PID.
- Linux manages processes and their resource usage.
- Multiple processes can run at the same time.
- Processes can be monitored and managed using Linux commands.

## Process Monitoring Commands

### `ps`

The `ps` command displays information about currently running processes.

```bash
ps
ps aux
ps aux | grep something
top
htop
sudo apt install htop

we can get process ID by giving "&"
for ex : python3 main.py & 
gives its process ID

## Killing Processes

Linux provides commands to terminate running processes. The main commands used for this are `kill`, `kill -9`, and `pkill`.

Every process has a unique Process ID (PID).

### `kill`

The `kill` command sends a signal to a process using its PID.

```bash
kill PID