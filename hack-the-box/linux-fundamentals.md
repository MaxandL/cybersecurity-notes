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
