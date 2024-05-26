### Unix and Shell Scripting QnA

#### Linux System Organization

**Q1:** What is the root directory in Linux?  
<details>
<summary>Answer</summary>
Root user has write privilege under this directory. Every single file and directory starts from the root directory.
</details>

**Q2:** What does the /bin directory contain?  
<details>
<summary>Answer</summary>
Contains binary executables. Common Linux commands used in single-user modes are located here, such as ps, ls, ping, grep, cp.
</details>

**Q3:** What is stored in the /sbin directory?  
<details>
<summary>Answer</summary>
Contains binary executables used by system administrators for system maintenance, such as iptables, reboot, fdisk, ifconfig, swapon.
</details>

**Q4:** What type of files are found in the /etc directory?  
<details>
<summary>Answer</summary>
Contains configuration files required by all programs, including startup and shutdown scripts, such as /etc/resolv.conf, /etc/logrotate.conf.
</details>

**Q5:** What is the purpose of the /dev directory?  
<details>
<summary>Answer</summary>
Contains device files, including terminal devices, USB, or any device attached to the system, such as /dev/tty1, /dev/usbmon0.
</details>

**Q6:** What information is stored in the /proc directory?  
<details>
<summary>Answer</summary>
Pseudo filesystem containing information about running processes, such as /proc/{pid}.
</details>

**Q7:** What type of files are located in the /var directory?  
<details>
<summary>Answer</summary>
Contains files that are expected to grow, such as system log files (/var/log), packages and database files (/var/lib), emails (/var/mail), print queues (/var/spool), lock files (/var/lock), temp files needed across reboots (/var/tmp).
</details>

**Q8:** What is the function of the /tmp directory?  
<details>
<summary>Answer</summary>
Contains temporary files created by the system and users. Files are deleted when the system is rebooted.
</details>

**Q9:** What is stored in the /usr directory?  
<details>
<summary>Answer</summary>
Contains binaries, libraries, documentation, and source code for second-level programs, such as /usr/bin, /usr/sbin, /usr/lib, /usr/local.
</details>

**Q10:** What is the purpose of the /home directory?  
<details>
<summary>Answer</summary>
Home directories for all users to store their personal files, such as /home/john, /home/nikita.
</details>

**Q11:** What does the /boot directory contain?  
<details>
<summary>Answer</summary>
Contains boot loader related files, such as kernel initrd, vmlinux, grub files.
</details>

**Q12:** What is stored in the /lib directory?  
<details>
<summary>Answer</summary>
Contains library files that support the binaries located under /bin and /sbin.
</details>

**Q13:** What is the /opt directory used for?  
<details>
<summary>Answer</summary>
Contains add-on applications from individual vendors.
</details>

**Q14:** What is the /mnt directory used for?  
<details>
<summary>Answer</summary>
Temporary mount directory where sysadmins can mount filesystems.
</details>

**Q15:** What is the /media directory used for?  
<details>
<summary>Answer</summary>
Temporary mount directory for removable devices, such as /media/cdrom for CD-ROM.
</details>

**Q16:** What is stored in the /srv directory?  
<details>
<summary>Answer</summary>
Contains server-specific services related data, such as /srv/cvs for CVS data.
</details>

#### File System

**Q17:** What is a file system?  
<details>
<summary>Answer</summary>
A method and data structure that the operating system uses to control how data is stored and retrieved.
</details>

**Q18:** What are the main functions of a file system?  
<details>
<summary>Answer</summary>
1. Data storage
2. Namespace
3. Security model
4. API
5. Implementation
</details>

**Q19:** Name some popular file system formats.  
<details>
<summary>Answer</summary>
- Windows: FAT, NTFS, exFAT
- macOS: HFS, APFS, HFS+
- Linux: EXT2/3/4, XFS, JFS, Btrfs
</details>

#### Linux File System History

**Q20:** What was the main goal of the EXT file system?  
<details>
<summary>Answer</summary>
To overcome the maximum size of writable files, increasing it from 64 MB to 2 GB and extending the maximum length of file names to 255 bytes.
</details>

**Q21:** What is the primary innovation of EXT2?  
<details>
<summary>Answer</summary>
Data is written in blocks of equal length, significantly increasing filesystem performance and the maximum file size to 2 TB.
</details>

**Q22:** How does EXT3 improve upon EXT2?  
<details>
<summary>Answer</summary>
Includes journaling to reduce the risk of data loss while maintaining the same file size and data block length.
</details>

**Q23:** What are the advantages of EXT4 over EXT3?  
<details>
<summary>Answer</summary>
Increased speed and maximum file size to 16 TB.
</details>

#### Mounting

**Q24:** What does "mounting" a filesystem mean in Linux?  
<details>
<summary>Answer</summary>
Making the filesystem accessible to the operating system by logically connecting it to the OS.
</details>

#### Command Basics

**Q25:** What is the purpose of the prompt in Linux?  
<details>
<summary>Answer</summary>
It indicates where the user can input commands.
</details>

**Q26:** How can you get help regarding a command in Linux?  
<details>
<summary>Answer</summary>
Use `command --help`.
</details>

#### Directory Commands

**Q27:** What does the `pwd` command do?  
<details>
<summary>Answer</summary>
Displays the current directory.
</details>

**Q28:** What is the purpose of the `cd` command?  
<details>
<summary>Answer</summary>
Changes the current directory.
</details>

**Q29:** What does the `ls` command do?  
<details>
<summary>Answer</summary>
Lists the contents of a directory.
</details>

**Q30:** What is the difference between `ls -a`, `ls -l`, and `ls -lh`?  
<details>
<summary>Answer</summary>
- `ls -a`: Includes hidden files.
- `ls -l`: Provides a detailed listing.
- `ls -lh`: Shows file sizes in a human-readable format.
</details>

**Q31:** What does the `mkdir` command do?  
<details>
<summary>Answer</summary>
Creates a new directory.
</details>

**Q32:** What is the `rmdir` command used for?  
<details>
<summary>Answer</summary>
Removes an empty directory.
</details>

#### File Commands

**Q33:** What does the `file` command do?  
<details>
<summary>Answer</summary>
Determines the file type regardless of file extension.
</details>

**Q34:** What does the `touch` command do?  
<details>
<summary>Answer</summary>
Creates an empty file.
</details>

**Q35:** What does the `rm` command do?  
<details>
<summary>Answer</summary>
Removes a file.
</details>

**Q36:** What does the `rm -i` command do?  
<details>
<summary>Answer</summary>
Removes a file with confirmation.
</details>

**Q37:** What is the purpose of the `cp` command?  
<details>
<summary>Answer</summary>
Copies files or directories.
</details>

**Q38:** What is the difference between `cp` and `cp -r`?  
<details>
<summary>Answer</summary>
- `cp`: Copies files.
- `cp -r`: Copies directories recursively.
</details>

**Q39:** What does the `mv` command do?  
<details>
<summary>Answer</summary>
Moves or renames files and directories.
</details>

#### File Content Commands

**Q40:** What does the `head` command do?  
<details>
<summary>Answer</summary>
Displays the first ten lines of a file.
</details>

**Q41:** How can you display the first n lines of a file using the `head` command?  
<details>
<summary>Answer</summary>
Use `head -n [number]`.
</details>

**Q42:** What does the `tail` command do?  
<details>
<summary>Answer</summary>
Displays the last ten lines of a file.
</details>

**Q43:** How can you display the last n lines of a file using the `tail` command?  
<details>
<summary>Answer</summary>
Use `tail -n [number]`.
</details>
