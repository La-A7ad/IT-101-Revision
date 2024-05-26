Sure, here is the QnA question bank with highlighted questions and answers hidden using spoilers.

### Unix and Shell Scripting QnA

#### Essential Books

**Q1:** **What are the essential books mentioned in the lecture?**  
<details>
<summary>Answer</summary>
- Linux Fundamentals by Paul Cobbaut (2015)
- Bash Reference Manual by Chet Ramey and Brian Fox, Edition 5.2 for Bash Version 5.2 (September 2022)
</details>

#### File Commands

**Q2:** **What does the `rm -rf` command do?**  
<details>
<summary>Answer</summary>
`rm -rf` removes directories and their contents recursively and forcefully.
</details>

**Q3:** **What are the four main functions of the `cat` command?**  
<details>
<summary>Answer</summary>
1. Copy standard input to standard output.
2. Create flat text files.
3. Concatenate files into a bigger file.
4. Copy files.
</details>

**Q4:** **How do you create a new file using the `cat` command?**  
<details>
<summary>Answer</summary>
`cat > [filename]` and end with `Ctrl+D`.
</details>

**Q5:** **What does the `tac` command do?**  
<details>
<summary>Answer</summary>
Displays file content in reverse order.
</details>

#### Echo Command

**Q6:** **What is the purpose of the `echo` command?**  
<details>
<summary>Answer</summary>
Writes the input it receives on the screen.
</details>

#### Shell Expansion

**Q7:** **What is shell expansion?**  
<details>
<summary>Answer</summary>
Shell expansion is the process by which the shell processes and changes commands before execution, cutting the command line into arguments.
</details>

**Q8:** **How does the shell handle white spaces during expansion?**  
<details>
<summary>Answer</summary>
Commands parts are separated by one or more consecutive white spaces or tabs, effectively cutting the command into arguments.
</details>

**Q9:** **How does the `echo` command handle quotes?**  
<details>
<summary>Answer</summary>
The `echo` command treats text between single or double quotes as a single argument.
</details>

**Q10:** **What does the `echo -e` command do?**  
<details>
<summary>Answer</summary>
Processes special characters within the text.
</details>

#### External and Built-in Commands

**Q11:** **What is the difference between external and built-in commands?**  
<details>
<summary>Answer</summary>
External commands are programs with their own binaries located in `/bin` or `/sbin`, while built-in commands are part of the shell program itself.
</details>

**Q12:** **How can you determine if a command is built-in or external?**  
<details>
<summary>Answer</summary>
Use the `type` command, e.g., `type [command]`.
</details>

#### Aliases

**Q13:** **What is an alias in Linux?**  
<details>
<summary>Answer</summary>
An alias is a shortcut for a command or a way to supply default parameters for commands.
</details>

**Q14:** **How do you view all defined aliases?**  
<details>
<summary>Answer</summary>
Use the `alias` command without parameters.
</details>

**Q15:** **How do you remove an alias?**  
<details>
<summary>Answer</summary>
Use the `unalias [name]` command.
</details>

#### Control Operators

**Q16:** **What does the semicolon (;) operator do?**  
<details>
<summary>Answer</summary>
Executes two or more commands sequentially.
</details>

**Q17:** **What is the purpose of the ampersand (&) operator?**  
<details>
<summary>Answer</summary>
Runs a command in the background.
</details>

**Q18:** **What is stored in the `$?` parameter?**  
<details>
<summary>Answer</summary>
The exit code of the previous command.
</details>

**Q19:** **How does the double ampersand (&&) operator function?**  
<details>
<summary>Answer</summary>
It is a logical AND operator; the second command is executed only if the first succeeds.
</details>

**Q20:** **What does the double vertical bar (||) operator represent?**  
<details>
<summary>Answer</summary>
It represents a logical OR; the second command is executed only if the first fails.
</details>

**Q21:** **How can you combine `&&` and `||` in a command?**  
<details>
<summary>Answer</summary>
Using `&&` and `||` together is the same as writing an if-then-else statement on the command line.
</details>

#### Linux User and Group Management

**Q22:** **What are the types of user accounts in Linux?**  
<details>
<summary>Answer</summary>
1. Root account (superuser)
2. System accounts
3. User accounts
</details>

**Q23:** **What is the function of group accounts in Linux?**  
<details>
<summary>Answer</summary>
Group accounts logically group user accounts for managing file permissions and processes.
</details>

**Q24:** **Name the four main user administration files in Linux.**  
<details>
<summary>Answer</summary>
1. /etc/passwd
2. /etc/shadow
3. /etc/group
4. /etc/gshadow
</details>

**Q25:** **How do you create a new group in Linux?**  
<details>
<summary>Answer</summary>
Use the `groupadd [groupname]` command.
</details>

**Q26:** **How do you modify an existing group name?**  
<details>
<summary>Answer</summary>
Use the `groupmod -n newgroupname oldgroupname` command.
</details>

**Q27:** **How do you delete an existing group in Linux?**  
<details>
<summary>Answer</summary>
Use the `groupdel [groupname]` command.
</details>

**Q28:** **How do you create a new user account in Linux?**  
<details>
<summary>Answer</summary>
Use the `sudo useradd -d homedir -g groupname -m -s shell -u userid accountname` command.
</details>

**Q29:** **How do you modify an existing user account?**  
<details>
<summary>Answer</summary>
Use the `sudo usermod -d /home/newdir -m -l oldname newname` command.
</details>

**Q30:** **How do you delete an existing user account in Linux?**  
<details>
<summary>Answer</summary>
Use the `sudo userdel -r [username]` command.
</details>

This comprehensive QnA question bank should help you thoroughly review and prepare for your exam on Unix and Shell Scripting. If you need any more questions or further details on specific topics, let me know!
