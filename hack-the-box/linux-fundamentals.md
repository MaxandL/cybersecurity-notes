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

## Task Scheduling

Task scheduling in Linux allows users and administrators to **automatically execute tasks at specific times or at regular intervals** without having to start them manually.

Tasks can include:

- Running scripts
- Software updates
- Database maintenance
- Backups
- System maintenance

Task scheduling is also important in cybersecurity because scheduled tasks can be used legitimately for administration, but they can also be abused to maintain **persistence** by automatically executing malicious scripts at specific times or intervals.

### Systemd

`systemd` can be used to schedule processes and scripts to run at specific times or intervals.

To schedule a task with `systemd`, we need:

1. Create a **timer** → Defines when the task should run.
2. Create a **service** → Defines what command or script should be executed.
3. Activate the **timer** → Starts and enables the scheduled task.

### Timer

A timer can specify when and how often the service should run.

Example:

```ini
[Unit]
Description=My Timer

[Timer]
OnBootSec=3min
OnUnitActiveSec=1hour

[Install]
WantedBy=timers.target
```

OnBootSec=3min means the task will run 3 minutes after the system boots.
OnUnitActiveSec=1hour means the task will run every hour after the unit was activated.

### Service

The service defines the command or script that will be executed.

```ini
[Unit]
Description=My Service

[Service]
ExecStart=/full/path/to/my/script.sh

[Install]
WantedBy=multi-user.target
```
ExecStart specifies the full path to the script or command that should be executed.

After creating or modifying a systemd service or timer, we need to reload systemd:
```bash
sudo systemctl daemon-reload
```
Then we can start and enable the timer:
```bash
sudo systemctl start mytimer.timer
sudo systemctl enable mytimer.timer
```
- start → Starts the timer immediately.
- enable → Makes the timer start automatically when the system boots.

### Cron

Cron is another tool used in Linux to schedule and automate tasks.

Cron uses a file called crontab to define when a command or script should be executed.

A Cron schedule has five time fields:

Field	        Values	 Description
- Minutes	    0-59	   Minute when the task should run
- Hours	      0-23	   Hour when the task should run
- Day of month	1-31   	 Day of the month
- Month	      1-12	   Month when the task should run
- Day of week	0-7	     Day of the week

Example:
```bash
0 */6 * * * /path/to/update_software.sh
```txt
This executes update_software.sh every 6 hours.
```
Another example:
```txt
0 0 1 * * /path/to/scripts/run_scripts.sh
```
This executes the script at midnight on the first day of every month.

- Systemd → Uses timers and services.
- Cron → Uses a crontab file.

# Network Services

Network services are programs that provide specific functionality over a network. Some of the important services covered are SSH, NFS, Web Servers, and VPNs.

## SSH

**SSH (Secure Shell)** allows us to connect remotely to another computer and interact with it through a terminal.

The connection is encrypted, which protects the communication between the two machines.

SSH can be used to:

- Connect to a remote Linux system.
- Execute commands on the remote system.
- Manage a remote computer.
- Transfer files securely.

---

## NFS

**NFS (Network File System)** allows files and directories to be shared over a network.

With NFS, a directory located on one system can be accessed from another system through the network.

This allows users and systems to work with network files as if they were part of the local filesystem.

---

## Web Servers

A **web server** is a service that provides web pages, files, and other resources to clients over a network.

One example is **Apache**.

Apache can be used to host websites and serve their files to users who connect to the server through HTTP or HTTPS.

---

## VPN

A **VPN (Virtual Private Network)** creates a private connection between a device and another network through a network tunnel.

VPNs can use encryption to protect the data transmitted through the connection.

They can allow a user to remotely access resources that are available inside another network.

---

## Summary

| Service | Purpose |
|---|---|
| **SSH** | Connect to and manage a remote computer securely |
| **NFS** | Share files and directories over a network |
| **Web Server** | Host and serve websites and files |
| **VPN** | Create a private connection to another network |


## Web Services

### Apache
- Apache is one of the most widely used web servers.
- It handles communication between web browsers and web servers.
- Apache is modular, meaning it can be extended with different modules for specific tasks.
Some important modules:
 - mod_ssl → encrypts communication using SSL/TLS.
 - mod_proxy → works with proxy servers and redirects requests.
 - mod_headers → allows modification of HTTP headers.
 - mod_rewrite → allows URLs and requests to be rewritten.
- Apache can serve static content and generate dynamic web pages using languages such as PHP, Perl, Ruby, Python, JavaScript, and others.

By default, Apache listens on HTTP port 80.

The default Apache page can be accessed through:
```bash
http://localhost
```
If port 80 is already being used, Apache can be configured to use another port, such as 8080, by modifying:
```bash
/etc/apache2/ports.conf
```
Then the server can be accessed with:
```bash
http://localhost:8080
```
## cURL

cURL is a command-line tool used to communicate with web servers and transfer data through protocols such as:

- HTTP
- HTTPS
- FTP
- SFTP
- FTPS
- SCP

It can be used to retrieve web pages and inspect server responses directly from the terminal.
```bash
curl http://localhost
```
## Wget

wget is another command-line tool used to download files from HTTP and FTP servers.
```bash
wget http://localhost
```
Unlike curl, wget normally saves the downloaded content to a local file, such as:
```txt
index.html
```
## Python 3 Web Server

Python 3 can be used to quickly create a simple web server from any directory:
```bash
python3 -m http.server
```
By default, it listens on port 8000:
```bash
http://0.0.0.0:8000/
```
This is useful for quickly serving files or testing web communication.

## Backup and Restore


Linux provides several tools that can be used to create backups and restore data. These tools help protect files and directories from data loss, corruption, or system failures.

The main tools covered in this section are:

- **Rsync**
- **Duplicity**
- **Deja Dup**

### Rsync

**Rsync** is an open-source tool used to create fast and secure backups locally or on a remote system.

One of its main advantages is that it only transfers the parts of files that have changed, making it efficient when working with large amounts of data.

It can be used to:

- Backup directories.
- Synchronize files between systems.
- Transfer backups to remote servers.
- Restore files and directories.

### Duplicity

Duplicity is a backup tool that builds on Rsync and adds encryption capabilities.

It can be used to create encrypted backups and store them on:

Remote servers.
FTP servers.
Cloud services such as Amazon S3.

This provides an additional layer of security because sensitive backup data can be encrypted.

### Deja Dup

Deja Dup is a more user-friendly backup tool that provides a graphical interface.

It makes it easier to create and restore backups without having to use the command line.

Deja Dup also supports encrypted backups and uses Rsync behind the scenes.

### Auto-Synchronization

Rsync can be combined with Cron to automatically synchronize files at regular intervals.

For example, we can create a script called:

```bash
RSYNC_Backup.sh
```
The script can contain:

```bash
#!/bin/bash

rsync -avz -e ssh /path/to/mydirectory user@backup_server:/path/to/backup/directory
```

We need to make the script executable:
```bash
chmod +x RSYNC_Backup.sh
```
Then we can edit the user's crontab:
```bash
crontab -e
```
For example:
```bash
0 * * * * /path/to/RSYNC_Backup.sh
```
This runs the backup script every hour at minute 0.

# File System Management

---

Linux file system management involves organizing, storing, and managing data on disks and other storage devices.

Linux supports different file systems, such as:

- `ext2`
- `ext3`
- `ext4`
- `XFS`
- `Btrfs`
- `NTFS`

## File Types

Linux mainly uses three types of files:

### Regular Files

Regular files are the most common type of files. They can contain text, binary data, images, audio, or executable programs.

### Directories

Directories are special files that contain other files and directories. They are used to organize the file system.

### Symbolic Links

Symbolic links (`symlinks`) act as references or shortcuts to other files or directories. They allow us to access files located in another part of the file system without duplicating them.

---

### Inodes

An **inode** is a data structure that stores metadata about a file or directory.

It contains information such as:

- Permissions
- Owner
- File size
- Timestamps
- Pointers to the blocks where the file's data is stored

The inode does **not** store the actual file contents or the file name.

The `inode table` contains all the inodes used by the file system.

---

### Disks and Partitions

Linux allows us to manage physical storage devices such as:

- Hard drives
- SSDs
- USB drives

A disk can be divided into different **partitions**. Each partition can have its own file system, such as `ext4`, `NTFS`, or `FAT32`.

### Fdisk

`fdisk` can be used to manage disk partitions and display information about disks and their partitions.

```bash
sudo fdisk -l
```
### Mounting

A partition or storage device needs to be assigned to a directory before its contents can be accessed through the Linux file system.

This process is called mounting.

The directory where the device is mounted is called the mount point.

View Mounted File Systems

```bash
mount
```
Mount a USB Drive

For example, to mount /dev/sdb1 to /mnt/usb:

```bash
sudo mount /dev/sdb1 /mnt/usb
```
Then we can access it:
```bash
cd /mnt/usb
ls -l
```
Unmount a File System

To unmount a file system:
```bash
sudo umount /mnt/usb
```
A file system cannot be unmounted while it is being used by an active process.

### Lsof

lsof can be used to find open files and processes that are using a file system.
```bash
lsof | grep cry0l1t3
```
## SWAP

Swap is disk space that Linux can use when the available physical RAM is completely used.

When the system runs out of physical memory, the kernel can move inactive memory pages from RAM to the Swap space. This process is called swapping.

Swap can be created during the operating system installation or added later.

### Mkswap

mkswap prepares a device or file to be used as Swap space.

### Swapon

swapon activates the Swap space so that the system can use it.

# Containerization

---

Containerization is a technology used to package and run applications in isolated environments called **containers**.

Containers are different from virtual machines because they **do not require a complete operating system for each instance**. Instead, containers share the **kernel of the host system**, making them lighter and more efficient than virtual machines.

A container includes everything an application needs to run, such as:

- Application code
- Libraries
- Dependencies
- Configuration files
- Required tools

This makes applications more portable and consistent between different environments.

### Docker

**Docker** is an open-source platform used to create, deploy, and manage containers.

Docker uses **images** as templates for creating containers. An image contains the files, libraries, dependencies, and configurations required by an application.

A `Dockerfile` contains the instructions used to build a Docker image.

Some important Docker commands are:

```bash
docker ps
```
Lists running containers.
```bash
docker start <container>
```
Starts a stopped container.
```bash
docker stop <container>
```
Stops a running container.
```bash
docker restart <container>
```
Restarts a container.
```bash
docker rm <container>
```
Removes a container.
```bash
docker rmi <image>
```
Removes a Docker image.
```bash
docker logs <container>
```
Displays the logs of a container.
```bash
Docker Build
docker build -t FS_docker .
```
Builds a Docker image from a Dockerfile and gives it the tag FS_docker.

Docker Run
```bash
docker run -p 8022:22 -p 8080:80 -d FS_docker
```
Creates and starts a container from the FS_docker image.

The -p option maps ports from the host to the container, while -d runs the container in the background.

Docker containers are stateless by design, meaning that changes made inside a container can be lost when the container is removed. To preserve data, Docker volumes can be used.

### Linux Containers (LXC)

LXC (Linux Containers) is another Linux containerization technology.

LXC allows multiple isolated Linux environments to run on the same host. Like Docker, LXC containers share the host's Linux kernel instead of running a complete operating system kernel for every container.

LXC uses Linux features such as:

- cgroups → Control and limit resources such as CPU and memory.
- namespaces → Isolate processes, networks, and file systems between containers.
Install LXC
```bash
sudo apt install lxc -y
```
Create an LXC Container
```bash
sudo lxc-create -n linuxcontainer -t ubuntu
```
Creates a new Ubuntu container named linuxcontainer.

LXC Management Commands
```bash
lxc-ls
```
Lists existing containers.
```bash
lxc-stop -n <container>
```
Stops a container.
```bash
lxc-start -n <container>
```
Starts a stopped container.
```bash
lxc-restart -n <container>
```
Restarts a container.
```bash
lxc-attach -n <container>
```
Connects to a container.

