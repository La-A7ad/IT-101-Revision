Sure, here is the QnA question bank with highlighted questions and answers hidden using spoilers.

### Unix and Shell Scripting QnA

#### If Statement

**Q1:** **What is an if statement in programming?**  
<details>
<summary>Answer</summary>
In programming, the if statement is a conditional expression.
</details>

**Q2:** **What does the if statement evaluate in Bash?**  
<details>
<summary>Answer</summary>
The command tested in the if statement evaluates based on the exit status.
</details>

**Q3:** **What is the exit status if a command completes successfully?**  
<details>
<summary>Answer</summary>
The exit status is 0.
</details>

**Q4:** **What is the exit status if a command throws an error?**  
<details>
<summary>Answer</summary>
The exit status is any number between 1 and 255.
</details>

**Q5:** **What is the syntax for an if statement in Bash?**  
<details>
<summary>Answer</summary>
The if statement is composed of the `if` keyword, the conditional phrase, and the `then` keyword. The `fi` keyword is used at the end of the statement.
</details>

**Q6:** **What happens if the condition in an if statement evaluates to true?**  
<details>
<summary>Answer</summary>
The commands get executed.
</details>

**Q7:** **What happens if the condition in an if statement returns false?**  
<details>
<summary>Answer</summary>
The commands are ignored.
</details>

**Q8:** **What are the variations of the if statement in Bash?**  
<details>
<summary>Answer</summary>
- `if...else` statement
- `if...elif...else` statement
- Nested if statement
</details>

#### Bash and Linux Commands

**Q9:** **What are some common builtin commands in Bash?**  
<details>
<summary>Answer</summary>
Common commands include `ls`, `echo`, `touch`, `mkdir`, `grep`, `pwd`, `cd`, `rmdir`, `cat`, `head`, `tail`, `chmod`, `cp`, `rm`.
</details>

**Q10:** **How do you execute a shell script in Bash?**  
<details>
<summary>Answer</summary>
Shell scripts are executed using `bash file.sh`.
</details>

#### Positional Command-Line Arguments

**Q11:** **How are command-line arguments read in Bash?**  
<details>
<summary>Answer</summary>
Command-line arguments are read in a positional manner, from position `$1`, `$2`, ..., `$n`.
</details>

**Q12:** **What does `$0` denote in a shell script?**  
<details>
<summary>Answer</summary>
`$0` denotes the name of the script.
</details>

**Q13:** **How are command-line arguments represented in Bash?**  
<details>
<summary>Answer</summary>
The pattern `$` followed by an integer is a reserved combination to represent the command-line arguments.
</details>

#### Logical Operators

**Q14:** **What are logical operators also known as?**  
<details>
<summary>Answer</summary>
Logical operators are also known as boolean operators.
</details>

**Q15:** **What does the logical AND (`&&`) operator do?**  
<details>
<summary>Answer</summary>
The logical AND (`&&`) operator returns true if both operands are true, otherwise it returns false.
</details>

**Q16:** **What does the logical OR (`||`) operator do?**  
<details>
<summary>Answer</summary>
The logical OR (`||`) operator returns true if either of the operands is true or both are true, and returns false if both are false.
</details>

**Q17:** **What does the Not Equal to (`!`) operator do?**  
<details>
<summary>Answer</summary>
The Not Equal to (`!`) operator returns true if the operand is false and returns false if the operand is true.
</details>

#### Bitwise Operators

**Q18:** **What is a bitwise operator?**  
<details>
<summary>Answer</summary>
A bitwise operator is used to perform bitwise operations on bit patterns.
</details>

**Q19:** **What does the bitwise AND (`&`) operator do?**  
<details>
<summary>Answer</summary>
The bitwise AND (`&`) operator performs binary AND operation bit by bit on the operands.
</details>

**Q20:** **What does the bitwise OR (`|`) operator do?**  
<details>
<summary>Answer</summary>
The bitwise OR (`|`) operator performs binary OR operation bit by bit on the operands.
</details>

#### Exit and Exit Status

**Q21:** **What does the exit status of a command indicate?**  
<details>
<summary>Answer</summary>
The exit status indicates whether a command executed successfully or failed. A zero (0) exit status indicates success, and a non-zero (1-255) exit status indicates failure.
</details>

**Q22:** **What exit status does a command return if it is not found?**  
<details>
<summary>Answer</summary>
If a command is not found, the child process created to execute it returns a status of `127`.
</details>

**Q23:** **What exit status does a command return if it is found but not executable?**  
<details>
<summary>Answer</summary>
If a command is found but is not executable, the return status is `126`.
</details>

**Q24:** **How can you get the exit status of the previously executed command in Bash?**  
<details>
<summary>Answer</summary>
You can use the special shell variable `$?` to get the exit status of the previously executed command.
</details>

**Q25:** **How do you print the exit status of the last command in Bash?**  
<details>
<summary>Answer</summary>
Use the `echo` command with `$?`, e.g., `echo $?`.
</details>

#### Regular Expressions

**Q26:** **What is a regular expression?**  
<details>
<summary>Answer</summary>
A regular expression is a pattern which matches some regular (predictable) text.
</details>

**Q27:** **Which Unix utilities commonly use regular expressions?**  
<details>
<summary>Answer</summary>
Regular expressions are used in many Unix utilities like `grep`, `sed`, `vi`, `emacs`, `awk`.
</details>

**Q28:** **How are regular expressions different from file name wildcards?**  
<details>
<summary>Answer</summary>
Regular expressions are interpreted and matched by special utilities like `grep`, whereas file name wildcards are interpreted and matched by shells. They have different wildcarding systems.
</details>

**Q29:** **What does the dot (`.`) character match in a regular expression?**  
<details>
<summary>Answer</summary>
The dot (`.`) matches any single character.
</details>

**Q30:** **What does the asterisk (`*`) character match in a regular expression?**  
<details>
<summary>Answer</summary>
The asterisk (`*`) matches zero or more occurrences of the previous single character pattern.
</details>

**Q31:** **How do you match a set or range of characters in a regular expression?**  
<details>
<summary>Answer</summary>
Use square brackets (`[]`). For example, `[wxyz]` matches any of `wxyz`, and `[u-z]` matches any character in the range `u` to `z`.
</details>

**Q32:** **How do you match the beginning of a line in a regular expression?**  
<details>
<summary>Answer</summary>
Use the caret (`^`). For example, `^TITLE` matches any line containing "TITLE" at the beginning.
</details>

**Q33:** **How do you match the end of a line in a regular expression?**  
<details>
<summary>Answer</summary>
Use the dollar sign (`$`). For example, `FINI$` matches any line ending in the phrase "FINI".
</details>

This comprehensive QnA question bank covers all the relevant content from Lecture 9 on Unix and Shell Scripting, including detailed analysis and examples from the images provided in the lecture slides. If you need any more questions or further details on specific topics, let me know!
