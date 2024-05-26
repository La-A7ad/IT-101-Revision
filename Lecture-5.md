File Permissions Introduction
Q1: What does the ls -l command display?

<details>
<summary>Answer</summary>
It displays the permissions, user, and group owner for files and directories.
</details>
Q2: What are the key questions the kernel checks before executing a program?

<details>
<summary>Answer</summary>
1. Is the file accessible to the user or group of the process that wants to run it?
2. Does the file permit execution by that user or group (or anybody)?
</details>
File Permissions
Q3: What are the abbreviations and octal values for read, write, and execute permissions?

<details>
<summary>Answer</summary>
- Read (r) = 4
- Write (w) = 2
- Execute (x) = 1
</details>
Q4: What does the first character in the permissions string indicate?

<details>
<summary>Answer</summary>
It indicates the file type (e.g., `-` for normal file, `d` for directory, `l` for symbolic link).
</details>
Access Rights
Q5: Who can change the permissions of a file?

<details>
<summary>Answer</summary>
The user who owns the file or the superuser `root`.
</details>
Q6: What are the three categories of permissions in Linux?

<details>
<summary>Answer</summary>
User, group, and others (world).
</details>
Changing Permissions
Q7: How do you change file permissions using symbolic mode?

<details>
<summary>Answer</summary>
Use the `chmod` command with symbolic operators. Example: `chmod g+x testfile`.
</details>
Q8: How do you change file permissions using absolute (octal) mode?

<details>
<summary>Answer</summary>
Use the `chmod` command with octal values. Example: `chmod 755 testfile`.
</details>
Q9: What is the syntax for adding, removing, and setting permissions using chmod in symbolic mode?

<details>
<summary>Answer</summary>
`chmod [who][operator][permission] file`
- `+` adds permission
- `-` removes permission
- `=` sets permission
</details>
Q10: How do you combine multiple permission changes in a single chmod command?

<details>
<summary>Answer</summary>
Use commas to separate multiple changes. Example: `chmod u+w,g-x,o-r file`
</details>
Q11: What are the octal values for read, write, and execute permissions?

<details>
<summary>Answer</summary>
- Read (r) = 4
- Write (w) = 2
- Execute (x) = 1
</details>
Changing Group and User Ownership
Q12: How do you change the group owner of a file?

<details>
<summary>Answer</summary>
Use the `chgrp [groupname] [file]` command.
</details>
Q13: How do you change the user owner of a file?

<details>
<summary>Answer</summary>
Use the `chown [username] [file]` command.
</details>
Q14: How do you change both the user and group owner of a file?

<details>
<summary>Answer</summary>
Use the `chown [username]:[groupname] [file]` command.
</details>
