Sure, here is the QnA question bank with highlighted questions and answers hidden using spoilers.

### Unix and Shell Scripting QnA

#### What is GitHub?

**Q1:** **What is GitHub?**  
<details>
<summary>Answer</summary>
GitHub is an online platform that allows you to synchronize your local Git repository onto the web. It is an online hosting service for Git repositories.
</details>

**Q2:** **What are the benefits of hosting a project on GitHub?**  
<details>
<summary>Answer</summary>
Hosting a project on GitHub enables working on a project remotely from different places, accessing and downloading the project from any computer, and collaborating with other developers from any location.
</details>

#### Git and GitHub

**Q3:** **What are the steps to install Git?**  
<details>
<summary>Answer</summary>
Use the command `sudo apt-get install git` to install Git.
</details>

**Q4:** **How do you configure Git with your name and email?**  
<details>
<summary>Answer</summary>
Use the commands:
- `git config --global user.name "Your Name"`
- `git config --global user.email "your.email@example.com"`
</details>

**Q5:** **What command initializes a Git repository?**  
<details>
<summary>Answer</summary>
`git init`
</details>

**Q6:** **How do you stage files for commit in Git?**  
<details>
<summary>Answer</summary>
Use the command `git add [filename]` to stage files.
</details>

**Q7:** **How do you commit changes in Git?**  
<details>
<summary>Answer</summary>
Use the command `git commit -m "Commit message"`
</details>

**Q8:** **What is the purpose of the `git push` command?**  
<details>
<summary>Answer</summary>
`git push` uploads local files to the remote repository on GitHub.
</details>

**Q9:** **What is the purpose of the `git pull` command?**  
<details>
<summary>Answer</summary>
`git pull` downloads files from the remote repository on GitHub to the local workspace.
</details>

#### BASH Shell

**Q10:** **What is a shell in Unix?**  
<details>
<summary>Answer</summary>
A shell is a macro processor that executes commands and serves as both a command interpreter and a programming language.
</details>

**Q11:** **What does BASH stand for?**  
<details>
<summary>Answer</summary>
BASH stands for Bourne-Again SHell.
</details>

**Q12:** **How can shells be used?**  
<details>
<summary>Answer</summary>
Shells can be used interactively, accepting input typed from the keyboard, or non-interactively, executing commands read from a file.
</details>

#### Bash Script File

**Q13:** **What is the first line of a Bash script?**  
<details>
<summary>Answer</summary>
`#!/bin/bash`
</details>

**Q14:** **How do you indicate a comment in a Bash script?**  
<details>
<summary>Answer</summary>
Lines that start with `#` are comments.
</details>

**Q15:** **How do you run a Bash script?**  
<details>
<summary>Answer</summary>
To run a script, use `./scriptname` or `bash scriptname.sh`.
</details>

#### `echo` Command

**Q16:** **What is the `echo` command used for in Bash?**  
<details>
<summary>Answer</summary>
The `echo` command is used to print text to the screen.
</details>

#### Get User Input

**Q17:** **How do you get user input in a Bash script?**  
<details>
<summary>Answer</summary>
Use the `read` command to get user input.
</details>

#### Use of Comments

**Q18:** **How do you add a single-line comment in a Bash script?**  
<details>
<summary>Answer</summary>
Use the `#` symbol to add a single-line comment.
</details>

#### Multi-Line Comment

**Q19:** **How do you add a multi-line comment in a Bash script?**  
<details>
<summary>Answer</summary>
Use `:` and `‘’` symbols to add multi-line comments.
</details>

#### Bash Shell Variable

**Q20:** **How do you create a variable in Bash?**  
<details>
<summary>Answer</summary>
Assign a value to the variable using `variable_name=value`.
</details>

**Q21:** **How do you access the value of a variable in Bash?**  
<details>
<summary>Answer</summary>
Use `$variable_name` to access the value of a variable.
</details>

#### Bash Shell Readonly Variables

**Q22:** **How do you declare a readonly variable in Bash?**  
<details>
<summary>Answer</summary>
Use the `readonly` keyword to declare a readonly variable.
</details>

#### Bash Variable Scope – Local and Global

**Q23:** **What is a global variable in Bash?**  
<details>
<summary>Answer</summary>
Global variables, also called environment variables, are available to all shells.
</details>

**Q24:** **How do you declare a global variable in Bash?**  
<details>
<summary>Answer</summary>
Use the `export` command to declare a global variable, e.g., `export VAR=value`.
</details>

**Q25:** **What is a local variable in Bash?**  
<details>
<summary>Answer</summary>
Local variables are visible only within the block of code where they are declared.
</details>

**Q26:** **How do you declare a local variable in Bash?**  
<details>
<summary>Answer</summary>
Use the `local` keyword within a function to declare a local variable.
</details>

#### Midterm Questions Examples

**Q27:** **True or False: The shell is an interface that interprets the command line input and calls the necessary programs to do the work.**  
<details>
<summary>Answer</summary>
True
</details>

**Q28:** **True or False: Linux can use FAT, NTFS as a file system.**  
<details>
<summary>Answer</summary>
False
</details>

**Q29:** **True or False: Namespace in an operating system is a naming and organizational methodology that provides rules for naming and structuring data.**  
<details>
<summary>Answer</summary>
True
</details>

**Q30:** **True or False: Linux is a case insensitive environment.**  
<details>
<summary>Answer</summary>
False
</details>

**Q31:** **Write the Linux command to delete a directory named 'stuff'.**  
<details>
<summary>Answer</summary>
`rm -rf stuff`
</details>

**Q32:** **Write the Linux command to change the user permission of 'dmesg.txt' to allow the user owner to execute the file (symbol or number).**  
<details>
<summary>Answer</summary>
`chmod u+x dmesg.txt`
</details>

**Q33:** **Write the Linux command to copy files that start with 's' to a destination directory "Work".**  
<details>
<summary>Answer</summary>
`cp s* Work/`
</details>

**Q34:** **What is the result of the command `tail -2 Numbers.txt` given the file 'Numbers.txt' with content: One, Two, Three, Four?**  
<details>
<summary>Answer</summary>
Displays the last 2 lines of the file: Three, Four
</details>

**Q35:** **What is the result of the command `tac Numbers.txt` given the file 'Numbers.txt' with content: One, Two, Three, Four?**  
<details>
<summary>Answer</summary>
Displays the file content in reverse order: Four, Three, Two, One
</details>

This comprehensive QnA question bank covers all the relevant content from Lecture 7 on Unix and Shell Scripting, including detailed analysis and examples from the images provided in the lecture slides. If you need any more questions or further details on specific topics, let me know!
