hese Linux commands empower users to efficiently navigate, manage, and manipulate files and directories. Understanding their functionality and various options is key to becoming proficient in working with the Linux command line.

# File Manipulation

## 1. sudo (Superuser Do) command
**sudo** stands for "Superuser Do," granting elevated privileges to execute commands. It's crucial for tasks requiring administrative access, such as system updates or installing software packages.
```Bash
Example: sudo apt upgrade
```
Here, sudo is used to upgrade the package list (apt upgrade) with elevated privileges, ensuring that the system's package information is current.
![sudo command screenshot](<images/linux_project_sudo apt Upgrade command.png>)


## 2. pwd (Print Working Directory) command
**pwd** prints the full path of the current working directory. It's fundamental for navigating the file system and understanding your current location.
```Bash
Example: pwd [option]
```
When you run pwd, it outputs the complete path from the root directory to your current working directory, helping you orient yourself within the file system.
![pwd command screenshot](<images/linux_project_pwd command.png>)


## 3. cd (Change Directory) command
**cd** is used to change the current working directory. It's essential for navigating through different folders.
```Bash
Example: cd [directory]
```
In this example, cd is employed to move into the "Documents" directory. You can use relative or absolute paths with cd to switch directories.

## 4. ls (List) command
**ls** lists the contents of a directory. It can be customized with various options to display additional information.
```Bash
Example: ls -l
```
The -l option provides a detailed listing, including file permissions, ownership, size, and modification date. This extra information aids in understanding the characteristics of listed files.
![ls command screenshot](images/linux_project_ls_command.png)


## 5. cat (Concatenate) command
**cat** is versatile; it concatenates and displays the content of files. It's commonly used to read the contents of text files.
```Bash
Example: cat filename.txt
```
In this example, cat outputs the entire content of the specified file, "filename.txt," to the terminal.


## 6. cp (Copy) command
**cp** copies files or directories. It's valuable for creating duplicates or backups.
```Bash
Example: cp sourcefile destination
```
Here, cp duplicates "sourcefile" to the specified "destination" path. It's crucial to ensure data redundancy or create replicas of files.

![cp command screenshot](images/linux_project_cp.png)


## 7. 'mv' (Move) command
**mv** moves files or directories, and it can also be used to rename them. It's a versatile command for organizing and managing files.
```Bash
Example: mv sourcefile destination
```
In this case, mv is used to move "sourcefile" to the specified "destination" path. It effectively relocates files within the file system.

![mv command screenshot](<images/linux_project_mv command.png>)

## 8. 'mkdir' (Make Directory) command
**mkdir** creates a new directory. It's essential for organizing files and projects.
```Bash
Example: mkdir new_directory
```
Running mkdir with a directory name as an argument creates a new directory with that name. This is useful for structuring your file system.
![mkdir command screenshot](<images/linux_project_mkdir command.png>)

## 9. rmdir (Remove Directory) command

**rmdir** removes empty directories. It's a straightforward way to delete directories without content.
```Bash
Example: rmdir empty_directory
```
Elaboration: If "empty_directory" is indeed empty, running rmdir removes it. For non-empty directories, rm -r is typically used.

## 10. rm (Remove) command

**rm** removes files or directories. Use with caution, as deleted data is usually not recoverable.
```Bash
Example: rm file.txt
```
Here, rm permanently deletes "file.txt." The -r option is often added for deleting directories and their contents recursively.

## 11. touch command
**touch** creates an empty file or updates access/modification times on existing files.
```Bash
Example: touch newfile.txt
```
Running touch with a filename as an argument creates an empty file or updates the timestamp of an existing file to the current time.

## 12. locate command
locate quickly searches for files based on a pre-built database. It's a fast but less comprehensive alternative to find.
```Bash
Example: locate filename
```
locate swiftly returns results based on the indexed database, making it efficient for finding files. Regularly updating the database is essential (updatedb).
![locate command screenshot](images/Linux_project_locate_command.png)

## 13. 'find' command
**find*** searches for files and directories within a directory hierarchy based on various criteria.
```Bash
Example: find /home/user -name "*.txt"
```
This example searches for all files with a ".txt" extension within the "/home/user" directory and its subdirectories. find provides extensive search options.
![find command screenshot](<images/linux_project_find command.png>)

## 14. 'grep' (Global Regular Expression Print) command
**grep** searches for patterns in files. It supports regular expressions and is useful for text extraction and filtering.
```Bash
Example: grep "pattern" file.txt
```
grep scans "file.txt" for occurrences of the specified "pattern" and prints lines containing matches. Regular expressions can enhance the search.
![grep command screenshot](<images/linux_project_grep command.png>)

## 15. df (Disk Free) command
**df** displays information about disk space usage, showing the available and used space on mounted filesystems.
```Bash
Example: df -h
```
The -h option makes the sizes human-readable (in KB, MB, GB). df provides a quick overview of available disk space.
![df command screenshot](images/linux_project_df_command.png)

## 16. du (Disk Usage) command

**du** shows the disk usage of files and directories. It's helpful for identifying space-consuming items.
```Bash
Example: du -h
```
The -h option makes the sizes human-readable. du can be used to analyze the disk space usage of specific directories.
![du command screenshot](images/linux_project_du_command.png)

## 17. 'head' command
**head** displays the first few lines of a file. It's useful for quickly inspecting the beginning of a file.
```Bash
Example: head -n 10 file.txt
```
The -n option specifies the number of lines to display. In this example, the first 10 lines of "file.txt" are shown.
![head command screenshot](images/linux_project_head_command.png)


## 18. 'tail' command
tail displays the last few lines of a file. It's handy for monitoring log files or checking the end of a file.
```Bash
Example: tail -n 5 file.txt
```
Similar to head, the -n option specifies the number of lines to display. Here, the last 5 lines of "file.txt" are shown.

![tail command screenshot](images/linux_project_tail_command.png)

## 19. diff (Difference)
**diff** compares the content of two files line by line, highlighting the differences.

```Bash
Example: diff file1.txt file2.txt
```
diff is commonly used for code changes, document revisions, or identifying alterations between two versions of a file. It outputs the lines that differ between the specified files.
![diff command screenshot](images/linux_project_diff_command.png)

## 20. tar command
tar is a versatile command for creating, modifying, and extracting tar archives, which are often used for bundling files and directories together.
```Bash
Example: tar -cvf archive.tar.gz /path/to/directory
```
In this example, tar is used to create a compressed tarball (archive.tar.gz) of the specified directory.

The following options can be used to archieve other useful outcomes.
-c: Create a new archive.
-v: Verbosely list the files processed.
-f: Use archive file specified.

# File Permisson and Ownership

## 21. chmod (Change Mode) command
**chmod** is a command used to modify the permissions of a file or directory in Linux. Permissions include read, write, and execute privileges for the owner, group, and others.
```Bash
Example: chmod 755 filename
```
In this example, chmod 755 assigns read (4) + write (2) + execute (1) permissions to the file owner, and read (4) + execute (1) permissions to the group and others.

## 22. chown (Change Owner) command

The **chown** command allows the change of file ownership in Linux. It can be used to change both the user and group ownership of a file or directory.
```Bash
Example: chown user:group filename
```
The command alters the owner to "user" and the group to "group" for the specified file, providing control over file access.
jobs

## 23. jobs command
The **jobs** command displays a list of background jobs running in the current shell session. These are processes that were started asynchronously.
```Bash
Example: jobs
```
It provides job IDs and their status, aiding in managing background tasks. Use with bg and fg to bring jobs to the foreground or send them to the background.

## 24. Kill command
kill is a versatile command for managing processes. It sends signals to processes, allowing termination, pausing, or reloading.
```Bash
Example: kill -9 PID
```
The -9 option sends the SIGKILL signal, forcibly terminating the process with the specified Process ID (PID). Different signals can be used to achieve various effects.


## 25. ping command

The ping command is a network diagnostic tool that sends ICMP echo requests to a specified host, testing network connectivity and latency.
```Bash
Example: ping google.com
```
![screen shot of ping command](images/linux_project_ping_command.png)
It measures the round-trip time for packets to travel to the target host and back. Continuous pinging helps identify network issues and packet loss.

## 26. wget command
**wget** is a command-line utility for downloading files from the internet. It supports various protocols, including HTTP, HTTPS, and FTP.
```Bash
Example: wget https://wordpress.org/latest.zip
```
![screenshot of wget command](images/linux_project_wget_command.png)
wget is scriptable and can be used for batch downloads. It supports resuming interrupted downloads, making it a reliable tool for fetching files from the web.

## 27. uname command
The **uname** command provides detailed system information, revealing the kernel version, network node hostname, kernel release, architecture, and more.

```Bash
Example: uname -a
```
![screen shot of uname command](images/linux_project_uname_command.png)
The -a option displays all available information. uname is valuable for identifying the system's characteristics and architecture.

## 28. 'top' command
The **top** command is a dynamic, real-time system monitoring tool that displays system resource usage, running processes, and overall system health.
```Bash
Example: top
```
![Top command screenshot](images/linux_project_top_command.png)
It provides a live, updating view of system activity, including CPU and memory usage, process details, and system uptime. Interactive features allow users to manage processes on-the-fly.

## 29. history command
The **history** command maintains a record of previously executed commands in the current shell session, promoting efficient command recall.
```Bash
Example: history
```
![history command screen shot](images/linux_project_history_command.png)
It assigns a unique number to each command, and users can rerun specific commands by referencing their respective numbers. This aids in command history management and repetition.
## 30. man (Manual) command
The **man** provides access to the manual pages, offering comprehensive documentation for various commands, utilities, and system calls.
```Bash
Example: man ls
```
Manual pages offer in-depth explanations of command options, usage syntax, and related details. A valuable resource for users seeking detailed information on command functionalities.
## 31. echo command

The **echo** command prints text or variable values to the terminal, making it a fundamental tool for script output and debugging.
```Bash
Example: echo "Hello, World!"
```
It is commonly used in shell scripts for displaying messages, setting environment variables, and producing script outputs. Supports the concatenation of text and variables.

## 32. zip command
The **zip** command compresses files into a zip archive, simplifying file storage, transfer, and backup.
```Bash
Example: zip -r archive.zip directory/
```
The -r option recursively includes all files and subdirectories within the specified directory in the zip archive. zip provides compression and archiving capabilities.

## 33. hostname command
The **hostname** command displays or sets the system's hostname, a critical identifier for networking purposes.
```Bash
Example: hostname
```
![hostname command screenshot](images/linux_project_hostname_command.png)
It is essential for network identification, and changing the hostname often requires superuser privileges. The hostname is a key component in network configurations.

## 34. useradd command

The **useradd** command is used to create a new user account on a Linux system. It involves setting up user-specific information and creating a home directory.
```Bash
Example: sudo useradd -m west
```

In this example, the -m option creates a home directory for the new user. Additional options can be used to set the user's shell, assign groups, and more.

## 35. apt-get command
The **apt-get** is a package management command used in Debian-based systems to install, upgrade, or remove software packages.
```Bash
Example: sudo apt-get install package-name
```

It fetches packages from repositories and resolves dependencies, simplifying software management. Modern systems often use apt as a more user-friendly front end to apt-get.

## 36. vi command
The **vi** command is a versatile text editor with multiple modes for inserting, deleting, and manipulating text. It is a standard editor in many Unix-like systems.
```Bash
Example: vi filename
```
vi has modes such as command mode, insert mode, and visual mode. It provides powerful features for efficient text editing but has a steeper learning curve compared to some other text editors.

## 37. alias, unalias command

The **alias** command allows users to create custom command shortcuts or aliases. It simplifies complex commands or provides alternative names.
```Bash
Example: alias ll='ls -l'
```
alias Elaboration: In this example, ll becomes an alias for ls -l, making it easier to remember and type.

**unalias** is used to remove previously defined aliases.

```Bash
Example: unalias ll
```
This removes the ll alias, reverting it to its default behavior.

## 38. su command

The **su** (Switch User) is used to switch to another user account or become the superuser. It prompts for the user's password.

```Bash
Example: su - username
```
The - option loads the environment variables of the specified user, providing a fresh environment.

## 39. htop command
The **htop** is an interactive process viewer that provides a detailed and visually appealing representation of system resources and processes.

```Bash
Example: htop
```
![htop command screen shot](images/linux_project_htop_command.png)

htop displays processes in a hierarchical tree structure and allows users to interactively manage processes, making it a more user-friendly alternative to top.
## 40. ps command

The **ps** (Process Status) displays information about currently running processes.
```Bash
Example: ps aux
```
The aux options provide a detailed listing of all processes, including those owned by other users. ps is a versatile command with various options for customizing output.
