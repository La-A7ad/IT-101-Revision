Sure, here is the corrected version of the QnA with proper formatting for the code blocks.

### Unix and Shell Scripting QnA

**Q1:** **When is a case statement used in Bash?**  
<details>
<summary>Answer</summary>
A case statement is used when a decision has to be made against multiple choices, replacing multiple if-statements in a script.
</details>

**Q2:** **What are the benefits of using a case statement over multiple if-statements?**  
<details>
<summary>Answer</summary>
A case statement improves the readability of code and is easier to maintain.
</details>

**Q3:** **How does a case statement in Bash differ from a case statement in C language?**  
<details>
<summary>Answer</summary>
In Bash, the case statement stops searching as soon as a match occurs and does not require a break statement.
</details>

**Q4:** **What keywords are used to start and end a case statement in Bash?**  
<details>
<summary>Answer</summary>
The `case` keyword starts the statement, and the `esac` keyword ends it.
</details>

**Q5:** **What operator is used to end the pattern cases list in a case statement?**  
<details>
<summary>Answer</summary>
The closing parenthesis `)` is used to end the pattern cases list.
</details>

**Q6:** **What must follow the body of a pattern case in a case statement?**  
<details>
<summary>Answer</summary>
The body must be followed by `;;`.
</details>

**Q7:** **How is the default case defined in a Bash case statement?**  
<details>
<summary>Answer</summary>
The default case is defined using the wildcard asterisk symbol `*`.
</details>

**Q8:** **What is the return status if no pattern is matched in a case statement?**  
<details>
<summary>Answer</summary>
The return status is zero.
</details>

**Q9:** **What is the return status if a pattern is matched and executed in a case statement?**  
<details>
<summary>Answer</summary>
The return status is the exit status of the executed body of the matched pattern case.
</details>

**Q10:** **How can multiple patterns be specified in a case statement?**  
<details>
<summary>Answer</summary>
Multiple patterns can be used, separated by the `|` operator.
</details>

#### Repetitive Tasks (Loops)

**Q11:** **What does a for loop do in Bash?**  
<details>
<summary>Answer</summary>
A for loop allows for the specification of a list of values and executes a list of commands for each value in the list.
</details>

**Q12:** **What is the syntax of a for loop in Bash?**  
<details>
<summary>Answer</summary>

```bash
for { variable name } in { list }
do
  commands
done
```

</details>

**Q13:** **What does a while loop do in Bash?**  
<details>
<summary>Answer</summary>
A while loop iterates over a block of code until the condition specified is evaluated to false.
</details>

**Q14:** **When is a while loop used in Bash?**  
<details>
<summary>Answer</summary>
A while loop is used when the number of iterations is unknown.
</details>

**Q15:** **What is the syntax of a while loop in Bash?**  
<details>
<summary>Answer</summary>

```bash
while [ condition ]
do
  commands
done
```

</details>

**Q16:** **What is the purpose of the until loop in Bash?**  
<details>
<summary>Answer</summary>
An until loop executes until the test command succeeds. As long as this command fails, the loop continues.
</details>

**Q17:** **What is the syntax of an until loop in Bash?**  
<details>
<summary>Answer</summary>

```bash
until [TEST-COMMAND];
do
  COMMANDS
done
```

</details>

#### Functions

**Q18:** **What is a function in Bash scripting?**  
<details>
<summary>Answer</summary>
A function is a method used in shell scripts to group reusable code blocks.
</details>

**Q19:** **What are the benefits of using functions in Bash scripting?**  
<details>
<summary>Answer</summary>
1. Functions are read directly into the shell's memory and stored for later use, making execution faster.  
2. Functions help organize long shell scripts into modular and reusable code blocks.
</details>

**Q20:** **What is the syntax for defining a function in Bash?**  
<details>
<summary>Answer</summary>

```bash
function <function name> () {
  commands
}
```

</details>

**Q21:** **How can a function be defined in a single line in Bash?**  
<details>
<summary>Answer</summary>

```bash
function <function name> () { commands; }
```

</details>

**Q22:** **What must be included at the end of commands when defining a function in a single line?**  
<details>
<summary>Answer</summary>
Commands must end with a semicolon `;`.
</details>

**Q23:** **When does a function execute in Bash?**  
<details>
<summary>Answer</summary>
A function executes when it is invoked after being declared.
</details>

#### Function Variables

**Q24:** **What is the default scope of variables in Bash?**  
<details>
<summary>Answer</summary>
Variables in Bash are global by default and accessible from anywhere, including function bodies.
</details>

**Q25:** **How do you declare a local variable in a Bash function?**  
<details>
<summary>Answer</summary>
Use the `local` keyword to declare a local variable.
</details>

**Q26:** **What happens when a local variable has the same name as a global variable in Bash?**  
<details>
<summary>Answer</summary>
A local variable shadows a global variable when the two carry the same name.
</details>

#### Function Arguments

**Q27:** **How do you pass arguments to a function in Bash?**  
<details>
<summary>Answer</summary>
Add the parameters after the function call separated by spaces.
</details>

**Q28:** **How do you access function arguments within a function in Bash?**  
<details>
<summary>Answer</summary>
Use positional command-line arguments (`$1`, `$2`, etc.) to access them within the function.
</details>

This should now have proper formatting and display the code correctly. Let me know if you need any further adjustments!
