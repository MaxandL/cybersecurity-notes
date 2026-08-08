## Linux Structure

Linux, is a robust operating system, flexibility, and open-source operating system. An operating system (OS) is software that manages all the hardware resources of a computer, facilitating communication between software applications and hardware componentsy. Linux comes in many different distributions often called "distros " which are versions of Linux tailored to various needs and preferences such as Ubuntu, Debian, Fedora, Kali Linux, and Parrot OS. .

## Linux Philosophy

- Everything is a file.
- Small programs that perform one task well which can be combined to work together.
- Combine programs together to solve complex problems
- Gives the user greater control over the operating system.
- Configuration data stored in a text file

## Linux Components

- Bootloader – run the booting process to start the operating system.
- Kernel – manages the resources for system's I/O devices at the hardware level.
- Daemons – Background services that keep the system running correctly.
- OS Shell – is the interface between the OS and the user. This interface allows the user to tell the OS what to do.
- Graphics server – Provides the graphical environment.
- Window Manager – Manages windows and the graphical desktop.
- Utilities – Programs and tools used by the user.

## Linux Architecture

The Linux operating system can be broken down into layers:
- Hardware
- Kernel
- Shell
- System Utility

## Linux File System Hierarchy

- /	    ->  Root directory containing the entire filesystem.
- /bin	->  Essential user commands.
- /boot	->  Bootloader and kernel files.
- /dev	->  Device files.
- /etc	->  System configuration files.
- /home	->  User home directories.
- /lib	->  Shared libraries.
- /media ->	Removable media.
- /mnt	->  Temporary mount points.
- /opt	->  Optional third-party software.
- /root	->  Home directory of the root user.
- /sbin	->  System administration binaries.
- /tmp	->  Temporary files.
- /usr	->  User applications and libraries.
- /var	->  Variable data such as logs and caches.

## Terminal & Shell

- The Linux terminal is the interface that allows the user to communicate with the operating system by entering text commands.
- The shell interprets those commands and sends them to the Linux kernel to execute them.
- Terminal emulators simulate a physical terminal inside a graphical interface (GUI), allowing users to access the shell without using a real console.
- Tools like Tmux extend the terminal's functionality by allowing multiple sessions, panes, and workspaces in a single window.

## Prompt

The Bash prompt is the command line displayed in the terminal that indicates the system is ready to receive commands. It shows useful information such as the current user, the hostname, and the current working directory. The prompt can be customized by modifying the `PS1` variable to display additional information like the date, time, IP address, or full directory path, making it more useful during penetration testing and system administration.

## Default Prompt

```bash
<username>@<hostname><current_directory>$
```

## Prompt Symbols

| Symbol | Description |
|---------|-------------|
| `$` | Regular user prompt |
| `#` | Root (privileged) user prompt |
| `~` | User's home directory |

## PS1 Special Characters

- `\u` → Current username
- `\h` → Hostname
- `\H` → Full hostname
- `\w` → Full current working directory
- `\d` → Current date
- `\t` → Current time (24-hour format)
- `\T` → Current time (12-hour format)
- `\@` → Current time
- `\n` → New line
- `\s` → Shell name
- `\j` → Number of background jobs

## Getting Help

This section explains how to find information about Linux commands by yourself instead of memorizing everything. It introduces the `ls` command as an example and shows how to use tools like `man`, `--help`, `-h`, and `apropos` to understand what commands do, their syntax, and available options. The main idea is to become independent and learn how to search for command documentation whenever needed.

## Useful Commands

- `ls` → List files and directories.
- `man <command>` → Open the complete manual page.
- `<command> --help` → Display a quick help menu with available options.
- `<command> -h` → Show a short help menu (supported by some commands).
- `apropos <keyword>` → Search for commands related to a keyword.

# System Information

This section introduces essential Linux commands used to gather information about the operating system, users, hardware, processes, networking, and system configuration. It also explains how to connect to a remote Linux machine using SSH to practice these commands in a real environment.

The module includes the first practical exercises, where you must use these commands to inspect the system and find specific information on your own. The goal is not only to learn the commands, but also to develop the ability to explore a Linux system independently, a fundamental skill for penetration testing and privilege escalation.

## Commands

- `ssh` → Connect to a remote machine using SSH.
- `whoami` → Display the current username.
- `id` → Show user ID (UID), group ID (GID), and group memberships.
- `hostname` → Display the system hostname.
- `uname` → Display operating system and kernel information.
- `uname -a` → Show all available system information.
- `uname -r` → Display the kernel release version.
- `pwd` → Print the current working directory.
- `ifconfig` → Display or configure network interfaces.
- `ip` → Display or manage IP addresses, routes, and interfaces.
- `netstat` → Display network connections and statistics.
- `ss` → Display socket and network connection information.
- `ps` → Display running processes.
- `who` → Show users currently logged into the system.
- `env` → Display environment variables.
- `lsblk` → List block storage devices.
- `lsusb` → List connected USB devices.
- `lsof` → List open files and the processes using them.
- `lspci` → List PCI devices.

## Navigation

This section explains how to navigate the Linux filesystem using the shell. It introduces the basic commands to identify the current directory, move between directories, and list their contents. It also covers hidden files, absolute paths, relative paths, tab auto-completion, command history, and shortcuts that make working in the terminal faster and more efficient.

## Commands

- `pwd` → Display the current working directory.
- `ls` → List directory contents.
- `ls -l` → Display a detailed list of files and directories.
- `ls -la` → Display all files, including hidden files, with detailed information.
- `cd <directory>` → Change the current directory.
- `cd -` → Return to the previous directory.
- `cd ..` → Move to the parent directory.
- `clear` → Clear the terminal screen.
- `Ctrl + L` → Clear the terminal screen (shortcut).
- `↑` / `↓` → Browse command history.
- `Ctrl + R` → Search through the command history.
- `TAB` → Auto-complete files and directory names.

# Working with Files and Directories

This section explains how to create, organize, move, rename, and copy files and directories in Linux using the command line. It also introduces directory structures, working with file paths, and basic file management commands. Finally, it encourages experimenting with the commands and researching how to delete files and directories.

## Commands

- `touch <file>` → Create an empty file.
- `mkdir <directory>` → Create a new directory.
- `mkdir -p <path>` → Create nested parent directories automatically.
- `tree` → Display the directory structure in a tree format.
- `mv <source> <destination>` → Move or rename files and directories.
- `cp <source> <destination>` → Copy files or directories.

# Editing Files

This section explains how to view and edit files in Linux using the terminal. It introduces the `cat` command to display file contents, the Nano editor for simple text editing, and the Vim editor for more advanced editing. It also explains Vim's different modes and recommends practicing with `vimtutor` to become familiar with its features.

## Commands

- `cat <file>` → Display the contents of a file.
- `nano <file>` → Create or edit a file using the Nano editor.
- `vim <file>` → Open or edit a file using the Vim editor.
- `:q` → Quit Vim.
- `vimtutor` → Launch the interactive Vim tutorial.
  
## Find Files and Directories

This section explains how to search for files, directories, and installed programs in Linux using different commands.

### which

- Finds the executable path of a program.
- Verifies whether a program is installed on the system.
- `which <command>`

### find

- Searches for files and directories in real time.
- Supports multiple filters to perform advanced searches.

**Common Filters**

- `-type f` → Search only for files.
- `-type d` → Search only for directories.
- `-name "*.conf"` → Search by file name or extension.
- `-user root` → Search files owned by a specific user.
- `-size +20k` → Search files larger than 20 KB.
- `-newermt YYYY-MM-DD` → Search files newer than a specific date.
- `-exec <command> {} \;` → Execute a command on each result.
- `2>/dev/null` → Hide permission errors.

**Example:**

```bash
find / -type f -name "*.conf" -user root -size +20k -newermt 2020-03-03 -exec ls -al {} \; 2>/dev/null
```

---

### locate

- Searches for files using a local database.
- Much faster than `find`.
- The database must be updated to keep the results accurate.

**Update the database**

```bash
sudo updatedb
```

**Example:**

```bash
locate "*.conf"
```
## File Descriptors and Redirections

This section explains how Linux handles input and output using **File Descriptors (FDs)** and how data can be redirected between commands, files, and processes.

### What are File Descriptors?

A **File Descriptor (FD)** is a number used by the Linux kernel to identify an open file, terminal, socket, or any other input/output resource.

Every process automatically starts with three standard file descriptors:

- `0` → **STDIN (Standard Input)**  
  Receives the input of a program, usually from the keyboard.

- `1` → **STDOUT (Standard Output)**  
  Displays the normal output of a program, usually on the terminal.

- `2` → **STDERR (Standard Error)**  
  Displays error messages separately from the normal output.

**Example:**

```bash
cat
```

After typing:

```
Hello World
```

`cat` receives the text through **STDIN (0)** and prints it back through **STDOUT (1)**.

---

## Redirections

### Redirect STDOUT (`>`)

Sends the normal output to a file.

```bash
ls > files.txt
```

---

### Append STDOUT (`>>`)

Adds the output to the end of an existing file without overwriting it.

```bash
echo "Hello" >> notes.txt
```

---

### Redirect STDIN (`<`)

Uses a file as the input for a command.

```bash
cat < file.txt
```

---

### Here Document (`<<`)

Creates an input stream until the delimiter is reached.

```bash
cat << EOF > file.txt
Hello World
EOF
```

---

### Redirect STDERR

Store only error messages.

```bash
find / -name shadow 2> errors.txt
```

Discard all errors.

```bash
find / -name shadow 2>/dev/null
```

---

### Redirect STDOUT and STDERR

Redirect normal output and errors into different files.

```bash
find / -name shadow 1> output.txt 2> errors.txt
```

---

## Pipes (`|`)

A pipe sends the **STDOUT** of one command directly to the **STDIN** of another command.

**Example:**

```bash
find /etc -name "*.conf" | grep systemd
```

The output of `find` becomes the input of `grep`.

Pipes can also be chained together.

```bash
find /etc -name "*.conf" 2>/dev/null | grep systemd | wc -l
```

This command:
- Searches for `.conf` files.
- Ignores permission errors.
- Filters results containing `systemd`.
- Counts the total number of matching files.

## Filter Contents

This section explains how to filter and process the contents of files and command output using different Linux utilities.

### Commands Covered

- **more**: Displays the contents of a file one page at a time.
- **less**: Similar to `more`, but allows forward and backward navigation with more features.
- **head**: Displays the first lines of a file (10 by default).
- **tail**: Displays the last lines of a file (10 by default).
- **sort**: Sorts the output alphabetically or numerically.
- **grep**: Searches and filters lines that match a pattern.
- **cut**: Extracts specific fields from each line using a delimiter.
- **tr**: Replaces or transforms characters.
- **column**: Formats the output into a readable table.
- **awk**: Processes and extracts specific fields from the input.
- **sed**: Replaces or modifies text using regular expressions.
- **wc**: Counts lines, words, or characters.

### Examples

The module demonstrates how these commands can be combined to filter and process data.

Example:

```bash
cat /etc/passwd | grep "/bin/bash" | cut -d":" -f1
```

This command:
1. Reads the `/etc/passwd` file.
2. Filters users whose shell is `/bin/bash`.
3. Displays only the usernames.

## Regular Expressions (RegEx)

This section introduces Regular Expressions (RegEx), which are search patterns used to perform more precise text filtering.

RegEx can be used with tools such as:

- `grep`
- `sed`
- `awk`

### Common Operators

- `()` → Groups expressions.
- `[]` → Defines character classes.
- `{}` → Specifies how many times a pattern is repeated.
- `|` → OR operator.
- `.*` → Operates similarly to an AND operator, Matches any number of characters.

### Examples

```bash
grep -E "(my|false)" /etc/passwd
```

Searches for lines containing **my** or **false**.

```bash
grep -E "(my.*false)" /etc/passwd
```

Searches for lines containing both **my** and **false** in that order.

# Permission Management

This section explains how Linux manages permissions for files and directories.

## File Type and Permissions

You can view the permissions of files and directories using:

```bash
ls -l
```

Example:

```text
-rwxr-xr--
```

The **first character** indicates the file type:

| Symbol | Type |
|--------|------|
| `-` | Regular file |
| `d` | Directory |
| `l` | Symbolic link |
| `c` | Character device |
| `b` | Block device |
| `s` | Socket |
| `p` | Named pipe (FIFO) |

The next nine characters represent the permissions.

Example:

```text
-rwxr-xr--
```

- Owner → `rwx`
- Group → `r-x`
- Others → `r--`

---

## File Permissions

Every file and directory has three basic permissions:

- **r (Read):** Allows reading the file or listing the contents of a directory.
- **w (Write):** Allows modifying a file or creating, deleting, and renaming files inside a directory.
- **x (Execute):** Allows executing a file or traversing (entering) a directory.

Permissions are assigned to three categories:

- **Owner (u)**
- **Group (g)**
- **Others (o)**

---

## Changing Permissions

Permissions can be modified using **chmod**.

### Symbolic mode

```bash
chmod u+x file
chmod g-w file
chmod o+r file
chmod a+r file
```

Where:

- `u` = owner
- `g` = group
- `o` = others
- `a` = all users

### Octal mode

| Value | Permission |
|------:|------------|
| 7 | rwx |
| 6 | rw- |
| 5 | r-x |
| 4 | r-- |
| 3 | -wx |
| 2 | -w- |
| 1 | --x |
| 0 | --- |

Example:

```bash
chmod 754 file
```

- Owner → `rwx`
- Group → `r-x`
- Others → `r--`

---

## Changing Owner

The owner and group of a file or directory can be changed using:

```bash
chown user:group file
```

Example:

```bash
chown root:root file
```

---

## SUID and SGID

Linux provides two special permission bits:

- **SUID (Set User ID):** Executes the file with the permissions of the file owner.
- **SGID (Set Group ID):** Executes the file with the permissions of the file's group.

These permissions appear as **s** instead of **x**.

Example:

```text
-rwsr-xr-x
```

---

## Sticky Bit

The Sticky Bit is mainly used on shared directories.

When enabled:

- Only the file owner, the directory owner, or **root** can delete or rename files.

It appears as:

- **t** → Sticky Bit enabled and execute permission exists.
- **T** → Sticky Bit enabled but execute permission is missing.

Example:

```text
drwxrwxrwt
drwxrwxrwT
```

##User Management

User management is an important part of Linux system administration. It allows administrators to create, modify, and delete users and groups, as well as execute commands with different privileges.

Linux uses users and groups to control access to files, directories, and system resources.

## Executing Commands as a User

Some files require higher privileges to access.

For example, `/etc/shadow` contains sensitive information related to user passwords.

If we try to access it as a normal user:

```bash
cat /etc/shadow
```
We may receive: cat: /etc/shadow: Permission denied.To execute a command with elevated privileges, we can use sudo.


### sudo

sudo stands for "superuser do".

It allows a permitted user to execute a command with the privileges of another user, usually root.

Example
```bash
sudo cat /etc/shadow
```

This executes cat /etc/shadow with root privileges.

sudo is commonly used when a normal user needs to perform an administrative task.

### su

The su command allows us to switch to another user.
By default, if no username is specified, it attempts to switch to the root user.

Example
```bash
su
```

We can also specify a particular user:
```bash
su username
```

The command will request the appropriate credentials and then switch to that user's account.

### useradd

The useradd command is used to create a new user account.

Basic syntax:
```bash
useradd <username>
```
Example:
```bash
useradd alex
```

This creates a new user called alex.

### userdel

The userdel command is used to delete a user account.

Example:
```bash
userdel alex
```

This removes the user account.

### usermod

The usermod command is used to modify an existing user account.

It can be used to change different properties of a user.

Example:
```bash
usermod <options> <username>
```
For example, it can be used to modify the groups associated with a user.

### addgroup

The addgroup command is used to create a new group.

Example:
```bash
addgroup developers
```
This creates a group called developers.

### delgroup

The delgroup command is used to remove a group from the system.

Example:
```bash
delgroup developers
```
This removes the developers group.

### passwd

The passwd command is used to change a user's password.

Example:
```bash
passwd alex
```
The system will ask for the new password.

# Package Management

Package management is used to install, update, and remove software on Linux systems.

A **package** is an archive that contains software binaries, configuration files, dependency information, and information needed to keep track of updates and upgrades.

## Package Managers

Linux distributions use different package management systems. Some common package managers are:

| Command | Description |
|---|---|
| `dpkg` | Installs, builds, removes, and manages Debian packages. |
| `apt` | Provides a high-level command-line interface for package management. |
| `aptitude` | An alternative high-level interface to the package manager. |
| `snap` | Installs, configures, refreshes, and removes Snap packages. |
| `gem` | Package manager for Ruby. |
| `pip` | Package installer for Python. |
| `git` | Distributed version control system used to download and manage repositories. |

## Packages and Dependencies

A package can require other packages to work correctly. These additional packages are called **dependencies**.

For example:

```text
Program
├── Dependency A
├── Dependency B
└── Dependency C
```

# Service and Process Management

## Services

Services, also known as **daemons**, are programs that run in the background without direct user interaction. They perform important tasks and provide functionality to the system.

There are two main types:

- **System Services:** Services required by the operating system, usually started during boot.
- **User-Installed Services:** Services installed by users, such as web servers, databases, SSH servers, etc.

Daemons often have a `d` at the end of their name, for example:

- `sshd` → SSH daemon
- `systemd` → System and service manager

The main things we usually want to do with services are:

1. Start or restart a service.
2. Stop a service.
3. Check the status of a service.
4. Enable or disable a service at boot.
5. Find services and processes.

---

## Processes

A **process** is a running program.

Linux assigns every process a **PID (Process ID)**, which is a unique number used to identify the process.

Processes can also have a **PPID (Parent Process ID)**, which identifies the process that started them.

Information about processes can be found in:

```bash
  /proc/
```

### systemctl

systemctl is used to manage services controlled by systemd.

Start a service
```bash
systemctl start ssh
```
Starts the SSH service.

Check the status of a service
```bash
systemctl status ssh
```
Shows whether the service is running, its PID, logs, and other information.

For example:
```text
Active: active (running)
Main PID: 846 (sshd)
```
Enable a service at boot
```bash
systemctl enable ssh
```
Makes the service start automatically when the system boots.

List all services
```bash
systemctl list-units --type=service
```
Shows the services currently loaded by systemd.

### ps

ps is used to view running processes.

For example:
```bash
ps -aux | grep ssh
```
This searches for processes related to SSH.

Example:
```text
root  846  ... /usr/sbin/sshd -D
```
Here, 846 is the PID of the sshd process.

### journalctl

journalctl is used to view system and service logs.

For example:
```bash
journalctl -u ssh.service --no-pager
```
This displays the logs generated by the SSH service.
This is useful when a service does not start correctly or has an error.

### Killing Processes

Processes can have different states:

- Running → The process is currently running.
- Waiting → The process is waiting for an event or system resource.
- Stopped → The process has been stopped.
- Zombie → The process has stopped but still has an entry in the process table.

Linux provides several commands for controlling processes:

- kill
- pkill
- pgrep
- killall

View available signals
```bash
kill -l
```
Some important signals are:

- SIGINT (2) → Interrupts a process, usually with Ctrl + C.
- SIGKILL (9) → Immediately terminates a process.
- SIGTERM (15) → Requests a process to terminate.
- SIGSTOP (19) → Stops/suspends a process.
- SIGTSTP (20) → Suspends a process, usually with Ctrl + Z.

For example:
```bash
kill -9 <PID>
```
This forcefully terminates the process with the specified PID.

### Background Processes

Sometimes we want to run a process in the background so that we can continue using the terminal.

Ctrl + Z suspends the current process.

Example:
```bash
ping -c 10 www.example.com
```
Press:Ctrl + Z
The process becomes stopped.

### jobs

```bash
jobs
```
Shows the processes currently running or stopped in the background.

### bg
```bash
bg
```
Continues a stopped process in the background.

### Using &

We can start a process directly in the background by adding &:

```bash
ping -c 10 www.example.com &
```

The command continues running while we can keep using the terminal.

### Foreground Processes

To bring a background process back to the foreground, we use:
```bash
fg <ID>
```
For example:
```bash
fg 1
```
This brings job 1 back to the foreground.

### Executing Multiple Commands

Linux allows us to execute multiple commands on the same line.

There are three important ways:

Semicolon ;
```bash
command1; command2; command3
```
The commands are executed one after another regardless of whether the previous command succeeded or failed.

Example:
```bash
echo '1'; ls MISSING_FILE; echo '3'
```

Even though ls produces an error, echo '3' is still executed.

### Double AND &&
```bash
command1 && command2 && command3
```
The next command is executed only if the previous command succeeds.

Example:
```bash
echo '1' && ls MISSING_FILE && echo '3'
```
Since ls MISSING_FILE produces an error, echo '3' is not executed.



