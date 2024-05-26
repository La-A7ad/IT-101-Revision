Sure, here is the corrected version of the QnA with proper formatting for the code blocks and additional questions to make the concepts more concrete.

### Unix and Shell Scripting QnA

#### Linux User and Group Management

**Q1:** **How do you create a new user account in Linux?**  
<details>
<summary>Answer</summary>

```bash
sudo useradd -d homedir -g groupname -m -s shell -u userid accountname
```
</details>

**Q2:** **How do you modify an existing user account in Linux?**  
<details>
<summary>Answer</summary>

```bash
sudo usermod -d /home/newdir -m -l oldname newname
```
</details>

**Q3:** **How do you delete a user account in Linux?**  
<details>
<summary>Answer</summary>

```bash
sudo userdel -r username
```
</details>

#### File Globbing

**Q4:** **What is file globbing?**  
<details>
<summary>Answer</summary>
File globbing, also known as Path Name Expansion, is the operation that recognizes wildcard patterns and expands them into path names.
</details>

**Q5:** **What does the asterisk (*) wildcard do in file globbing?**  
<details>
<summary>Answer</summary>
It matches any combination of characters, including none.
</details>

**Q6:** **What does the question mark (?) wildcard do in file globbing?**  
<details>
<summary>Answer</summary>
It matches exactly one character.
</details>

**Q7:** **How do square brackets ([]) work in file globbing?**  
<details>
<summary>Answer</summary>
Square brackets match a range of characters. For example, `[A-Z]` matches uppercase alphabets, `[a-z]` matches lowercase alphabets, `[0-9]` matches digits.
</details>

#### Pipe and Filters

**Q8:** **What is a pipe in Linux?**  
<details>
<summary>Answer</summary>
A pipe allows the output of one command to serve as input to the next command. It is represented by the `|` symbol.
</details>

**Q9:** **What are filters in Linux?**  
<details>
<summary>Answer</summary>
Filters are small programs that perform specific tasks efficiently, often used with pipes to process data streams.
</details>

**Q10:** **What is the `tee` filter used for?**  
<details>
<summary>Answer</summary>
The `tee` filter puts stdin on stdout and also writes it to a file.
</details>

**Q11:** **What does the `grep` command do?**  
<details>
<summary>Answer</summary>
`grep` is used to filter lines of text containing a specific string.
</details>

**Q12:** **What does the `grep -i` option do?**  
<details>
<summary>Answer</summary>
It performs a case-insensitive search.
</details>

**Q13:** **What does the `grep -v` option do?**  
<details>
<summary>Answer</summary>
It outputs lines that do not match the specified string.
</details>

**Q14:** **How can you combine `-i` and `-v` options in `grep`?**  
<details>
<summary>Answer</summary>
Use `grep -vi [pattern] [file]` to filter all lines that do not contain a case-insensitive match of the pattern.
</details>

**Q15:** **What is the `cut` command used for?**  
<details>
<summary>Answer</summary>
The `cut` command is used to select columns from files based on a delimiter or a count of bytes.
</details>

**Q16:** **How do you use the `cut` command to select fields based on a delimiter?**  
<details>
<summary>Answer</summary>

```bash
cut -d ':' -f1,3 file.txt
```
</details>

**Q17:** **What does `cut -c 5- file.txt` do?**  
<details>
<summary>Answer</summary>
It extracts everything from character 5 until the end of the line from each line of `file.txt`.
</details>

**Q18:** **What does the `wc` command do?**  
<details>
<summary>Answer</summary>
It counts words, lines, and characters in a file.
</details>

**Q19:** **What is the default behavior of the `sort` command?**  
<details>
<summary>Answer</summary>
The default behavior is to sort lines of text alphabetically.
</details>

**Q20:** **What does the `uniq` command do?**  
<details>
<summary>Answer</summary>
It removes duplicate lines from a sorted list.
</details>

**Q21:** **Why must data be sorted before using `uniq`?**  
<details>
<summary>Answer</summary>
`uniq` only removes consecutive duplicate lines, so the data must be sorted first to group duplicates together.
</details>

**Q22:** **What is `sed` used for in Linux?**  
<details>
<summary>Answer</summary>
`sed` is a stream editor used to search through, replace, add, and delete lines in a text file without opening it in a text editor.
</details>

**Q23:** **How do you use `sed` to replace text in a file?**  
<details>
<summary>Answer</summary>

```bash
sed 's/old-string/new-string/' filename.txt
```
</details>

**Q24:** **What does the `awk` command do?**  
<details>
<summary>Answer</summary>
`awk` is a powerful programming language used for text processing and pattern matching.
</details>

**Q25:** **How do you use `awk` to print the second column of a file?**  
<details>
<summary>Answer</summary>

```bash
awk '{print $2}' file.txt
```
</details>

**Q26:** **What does the `tr` command do?**  
<details>
<summary>Answer</summary>
The `tr` command translates or deletes characters from stdin and writes the result to stdout.
</details>

**Q27:** **How do you use `tr` to convert all lowercase letters to uppercase?**  
<details>
<summary>Answer</summary>

```bash
echo "text" | tr '[:lower:]' '[:upper:]'
```
</details>

**Q28:** **What does the `find` command do?**  
<details>
<summary>Answer</summary>
The `find` command searches for files and directories in a directory hierarchy based on a given expression.
</details>

**Q29:** **How do you use the `find` command to search for files named `example.txt`?**  
<details>
<summary>Answer</summary>

```bash
find /path -name example.txt
```
</details>

**Q30:** **What does the `xargs` command do?**  
<details>
<summary>Answer</summary>
The `xargs` command builds and executes command lines from stdin, allowing the output of one command to be used as arguments for another command.
</details>

**Q31:** **How do you use `find` and `xargs` to delete all `.txt` files in a directory?**  
<details>
<summary>Answer</summary>

```bash
find /path -name "*.txt" | xargs rm
```
</details>

This expanded QnA question bank covers more details about user and group management, file globbing, pipes and filters, and various commands used in Unix and Linux, providing a thorough understanding of the concepts. If you need any more questions or further details, let me know!
