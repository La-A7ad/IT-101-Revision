Q1: How are variables assigned in Bash?

<details>
<summary>Answer</summary>
Variables in Bash are assigned using the syntax `variable_name=value`. Unlike many other programming languages, Bash does not segregate its variables by "type."
</details>
Q2: How do you avoid using spaces in variable assignment in Bash?

<details>
<summary>Answer</summary>
When assigning variables in Bash, ensure there are no spaces around the equals sign. For example, `variable_name=value`.
</details>
Q3: How do you perform arithmetic operations and assign values using the let command in Bash?

<details>
<summary>Answer</summary>
Use the `let` command, for example: `let "x = 10 + 3"`.
</details>
Reserved Words
Q4: What are reserved words in Bash?

<details>
<summary>Answer</summary>
Reserved words are words that have special meaning to the shell. They are used to begin and end the shell’s compound commands.
</details>
Q5: Give examples of reserved words in Bash.

<details>
<summary>Answer</summary>
Examples include `if`, `else`, `while`, `for`, `do`, `done`, `function`.
</details>
Typing Variables
Q6: How can you assign textual values to Bash variables?

<details>
<summary>Answer</summary>
Bash variables can be assigned textual values using the syntax `variable_name="value"`.
</details>
Q7: What is the syntax for the declare statement in Bash?

<details>
<summary>Answer</summary>
The syntax for the `declare` statement is `declare OPTION(s) VARIABLE=value`.
</details>
Q8: What does the -a option in the declare statement do?

<details>
<summary>Answer</summary>
The `-a` option treats the variables as arrays.
</details>
Q9: What does the -f option in the declare statement do?

<details>
<summary>Answer</summary>
The `-f` option uses function names only.
</details>
Q10: What does the -i option in the declare statement do?

<details>
<summary>Answer</summary>
The `-i` option treats the variables as integers.
</details>
Q11: What does the -r option in the declare statement do?

<details>
<summary>Answer</summary>
The `-r` option makes the variables read-only.
</details>
Q12: What does the -x option in the declare statement do?

<details>
<summary>Answer</summary>
The `-x` option marks the variables for export via the environment.
</details>
Integer Variables and Arithmetic
Q13: What does the + operator do in Bash arithmetic?

<details>
<summary>Answer</summary>
The `+` operator performs addition.
</details>
Q14: What does the - operator do in Bash arithmetic?

<details>
<summary>Answer</summary>
The `-` operator performs subtraction.
</details>
Q15: What does the * operator do in Bash arithmetic?

<details>
<summary>Answer</summary>
The `*` operator performs multiplication.
</details>
Q16: What does the / operator do in Bash arithmetic?

<details>
<summary>Answer</summary>
The `/` operator performs division.
</details>
Q17: What does the ** operator do in Bash arithmetic?

<details>
<summary>Answer</summary>
The `**` operator performs exponentiation.
</details>
Q18: What does the % operator do in Bash arithmetic?

<details>
<summary>Answer</summary>
The `%` operator calculates the remainder of a division (modulo).
</details>
Q19: How do you increment a variable by a constant in Bash?

<details>
<summary>Answer</summary>
Use the `+=` operator. Example: `let "x += 3"`
</details>
Q20: How do you decrement a variable by a constant in Bash?

<details>
<summary>Answer</summary>
Use the `-=` operator. Example: `let "x -= 3"`
</details>
Q21: How do you multiply a variable by a constant in Bash?

<details>
<summary>Answer</summary>
Use the `*=` operator. Example: `let "x *= 3"`
</details>
Q22: How do you divide a variable by a constant in Bash and get the quotient?

<details>
<summary>Answer</summary>
Use the `/=` operator. Example: `let "x /= 3"`
</details>
Q23: How do you divide a variable by a constant in Bash and get the remainder?

<details>
<summary>Answer</summary>
Use the `%=` operator. Example: `let "x %= 3"`
</details>
Comparison Operators
Q24: What does the -eq operator do in Bash?

<details>
<summary>Answer</summary>
The `-eq` operator checks if two integers are equal.
</details>
Q25: What does the -ne operator do in Bash?

<details>
<summary>Answer</summary>
The `-ne` operator checks if two integers are not equal.
</details>
Q26: What does the -gt operator do in Bash?

<details>
<summary>Answer</summary>
The `-gt` operator checks if one integer is greater than another.
</details>
Q27: What does the -lt operator do in Bash?

<details>
<summary>Answer</summary>
The `-lt` operator checks if one integer is less than another.
</details>
Q28: What does the -ge operator do in Bash?

<details>
<summary>Answer</summary>
The `-ge` operator checks if one integer is greater than or equal to another.
</details>
Q29: What does the -le operator do in Bash?

<details>
<summary>Answer</summary>
The `-le` operator checks if one integer is less than or equal to another.
</details>
Ways to Compute Arithmetic Operations
Q30: How do you perform arithmetic operations using double parenthesis in Bash?

<details>
<summary>Answer</summary>
Use the syntax `result=$(( arithmetic_expression ))`. For example, `result=$(( 10 + 3 ))`.
</details>
Q31: How do you use the let command to perform arithmetic operations in Bash?

<details>
<summary>Answer</summary>
Use the `let` command with the arithmetic expression, for example: `let "result = 10 + 3"`.
</details>
Q32: How do you use the expr command with backticks to perform arithmetic operations in Bash?

<details>
<summary>Answer</summary>
Use the `expr` command with backticks, for example: ``result=`expr 10 + 3` ``.
</details>
String Operators
Q33: What is a string in Bash?

<details>
<summary>Answer</summary>
A string is a data type used to represent text rather than numbers. Strings are enclosed in quotation marks.
</details>
Q34: What does the = operator do in Bash string comparison?

<details>
<summary>Answer</summary>
The `=` operator checks whether two strings are equal.
</details>
Q35: What does the != operator do in Bash string comparison?

<details>
<summary>Answer</summary>
The `!=` operator checks whether two strings are not equal.
</details>
Q36: What does the < operator do in Bash string comparison?

<details>
<summary>Answer</summary>
The `<` operator checks whether one string is less than another.
</details>
Q37: What does the > operator do in Bash string comparison?

<details>
<summary>Answer</summary>
The `>` operator checks whether one string is greater than another.
</details>
Q38: What does the -n operator do in Bash string comparison?

<details>
<summary>Answer</summary>
The `-n` operator checks if the string length is greater than zero.
</details>
Q39: What does the -z operator do in Bash string comparison?

<details>
<summary>Answer</summary>
The `-z` operator checks if the string length is equal to zero.
</details>
Q40: How do you find the length of a string in Bash?

<details>
<summary>Answer</summary>
Use the syntax `${#string}` to find the length of a string.
</details>
Q41: How do you split a string by space in Bash?

<details>
<summary>Answer</summary>
Use `IFS=' ' read -r -a array <<< "$string"` to split a string by space.
</details>
Q42: How do you extract a substring in Bash?

<details>
<summary>Answer</summary>
Use the syntax `${string:position:length}` to extract a substring.
</details>
Q43: How do you concatenate strings in Bash?

<details>
<summary>Answer</summary>
Use the syntax `concatenated_string="${string1}${string2}"` to concatenate strings.
</details>
