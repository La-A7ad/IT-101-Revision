I understand the issue with the code formatting in the answer section. To ensure the code is properly formatted in markdown, you should use triple backticks to enclose the code block and specify the language. Here is the corrected version with proper formatting:

### Unix and Shell Scripting QnA

**Q1:** **Print Elements of an Array**
- Write a Bash script that declares an indexed array with at least five elements and prints each element on a new line.
<details>
<summary>Answer</summary>

```bash
#!/bin/bash
declare -a my_array=("one" "two" "three" "four" "five")
for element in "${my_array[@]}"; do
  echo $element
done
```
</details>

**Q2:** **Check File Existence and Permissions**
- Write a Bash script that takes a file name as an argument, checks if the file exists, and if it is readable, writable, and executable. Print appropriate messages.
<details>
<summary>Answer</summary>

```bash
#!/bin/bash
file=$1
if [ -e "$file" ]; then
  echo "File exists."
  [ -r "$file" ] && echo "File is readable."
  [ -w "$file" ] && echo "File is writable."
  [ -x "$file" ] && echo "File is executable."
else
  echo "File does not exist."
fi
```
</details>

**Q3:** **Calculate Factorial Using While Loop**
- Write a Bash script to calculate the factorial of a number provided as an argument using a while loop.
<details>
<summary>Answer</summary>

```bash
#!/bin/bash
number=$1
factorial=1
while [ $number -gt 1 ]; do
  factorial=$((factorial * number))
  number=$((number - 1))
done
echo "Factorial: $factorial"
```
</details>

**Q4:** **Function to Add Two Numbers**
- Write a Bash script that defines a function to add two numbers passed as arguments and prints the result.
<details>
<summary>Answer</summary>

```bash
#!/bin/bash
add() {
  result=$(( $1 + $2 ))
  echo "Sum: $result"
}
add 3 5
```
</details>

**Q5:** **Merge Two Arrays**
- Write a Bash script that declares two indexed arrays, merges them into a third array, and prints the elements of the merged array.
<details>
<summary>Answer</summary>

```bash
#!/bin/bash
array1=("one" "two" "three")
array2=("four" "five" "six")
merged_array=("${array1[@]}" "${array2[@]}")
for element in "${merged_array[@]}"; do
  echo $element
done
```
</details>

**Q6:** **Check User Input Validity Using If Statements**
- Write a Bash script that prompts the user to enter a number between 1 and 10. Use an if statement to check the input and print whether it is valid or not.
<details>
<summary>Answer</summary>

```bash
#!/bin/bash
read -p "Enter a number between 1 and 10: " num
if [ $num -ge 1 ] && [ $num -le 10 ]; then
  echo "Valid number."
else
  echo "Invalid number."
fi
```
</details>

**Q7:** **Print Even Numbers in a Range Using For Loop**
- Write a Bash script that takes two arguments representing a range and prints all even numbers within that range using a for loop.
<details>
<summary>Answer</summary>

```bash
#!/bin/bash
start=$1
end=$2
for ((i=start; i<=end; i++)); do
  if ((i % 2 == 0)); then
    echo $i
  fi
done
```
</details>

**Q8:** **Count Words in a File**
- Write a Bash script that reads a file line by line and counts the total number of words in the file.
<details>
<summary>Answer</summary>

```bash
#!/bin/bash
file=$1
word_count=0
while read -r line; do
  word_count=$((word_count + $(echo $line | wc -w)))
done < $file
echo "Total words: $word_count"
```
</details>

**Q9:** **Demonstrate Case Statement**
- Write a Bash script that asks the user to enter a day of the week and prints a specific message for each day using a case statement.
<details>
<summary>Answer</summary>

```bash
#!/bin/bash
read -p "Enter a day of the week: " day
case $day in
  Monday) echo "Start of the work week." ;;
  Friday) echo "End of the work week." ;;
  Saturday|Sunday) echo "Weekend!" ;;
  *) echo "Midweek day." ;;
esac
```
</details>

**Q10:** **Check for Palindrome String**
- Write a Bash script that checks if a given string is a palindrome.
<details>
<summary>Answer</summary>

```bash
#!/bin/bash
read -p "Enter a string: " str
if [ "$str" == "$(echo $str | rev)" ]; then
  echo "Palindrome."
else
  echo "Not a palindrome."
fi
```
</details>

**Q11:** **Associative Array for Storing Student Grades**
- Write a Bash script that uses an associative array to store student names as keys and their grades as values, then prints each student and their grade.
<details>
<summary>Answer</summary>

```bash
#!/bin/bash
declare -A student_grades
student_grades["Alice"]="A"
student_grades["Bob"]="B"
student_grades["Charlie"]="C"
for student in "${!student_grades[@]}"; do
  echo "$student: ${student_grades[$student]}"
done
```
</details>

**Q12:** **Append Timestamp to Log File**
- Write a Bash script that appends the current date and time to a log file every time it is run.
<details>
<summary>Answer</summary>

```bash
#!/bin/bash
log_file="log.txt"
echo "$(date)" >> $log_file
```
</details>

**Q13:** **Sum of Numbers Using Until Loop**
- Write a Bash script that calculates the sum of numbers from 1 to a given number using an until loop.
<details>
<summary>Answer</summary>

```bash
#!/bin/bash
number=$1
sum=0
counter=1
until [ $counter -gt $number ]; do
  sum=$((sum + counter))
  counter=$((counter + 1))
done
echo "Sum: $sum"
```
</details>

**Q14:** **Find and Replace Text in a File Using Sed**
- Write a Bash script that takes a filename, a search string, and a replacement string as arguments and replaces all occurrences of the search string with the replacement string in the file using `sed`.
<details>
<summary>Answer</summary>

```bash
#!/bin/bash
file=$1
search=$2
replace=$3
sed -i "s/$search/$replace/g" $file
```
</details>

**Q15:** **Check If a Number is Prime**
- Write a Bash script that checks if a given number is a prime number.
<details>
<summary>Answer</summary>

```bash
#!/bin/bash
number=$1
is_prime=1
for ((i=2; i<=number/2; i++)); do
  if ((number % i == 0)); then
    is_prime=0
    break
  fi
done
if ((is_prime)); then
  echo "$number is a prime number."
else
  echo "$number is not a prime number."
fi
```
</details>

**Q16:** **Calculate Fibonacci Sequence**
- Write a Bash script that calculates the first N Fibonacci numbers where N is provided as an argument.
<details>
<summary>Answer</summary>

```bash
#!/bin/bash
N=$1
a=0
b=1
echo "Fibonacci sequence up to $N terms:"
for ((i=0; i<N; i++)); do
  echo $a
  fn=$((a + b))
  a=$b
  b=$fn
done
```
</details>

**Q17:** **Script to Backup Files**
- Write a Bash script that takes a directory as an argument and creates a compressed backup of that directory.
<details>
<summary>Answer</summary>

```bash
#!/bin/bash
dir=$1
tar -czf backup_$(date +%F).tar.gz $dir
```
</details>

**Q18:** **Script to Monitor Disk Usage**
- Write a Bash script that checks the disk usage of a given directory and sends an email alert if the usage exceeds a specified threshold.
<details>
<summary>Answer</summary>

```bash
#!/bin/bash
dir=$1
threshold=$2
usage=$(du -s $dir | awk '{print $1}')
if [ $usage -gt $threshold ]; then
  echo "Disk usage of $dir exceeds $threshold" | mail -s "Disk Usage Alert" user@example.com
fi
```
</details>

**Q19:** **Generate System Report**
- Write a Bash script that generates a system report containing information about CPU, memory, disk usage, and network interfaces.
<details>
<summary>Answer</summary>

```bash
#!/bin/bash
echo "

CPU Info:"
lscpu
echo
echo "Memory Info:"
free -h
echo
echo "Disk Usage:"
df -h
echo
echo "Network Interfaces:"
ip a
```
</details>

**Q20:** **Script to Rotate Logs**
- Write a Bash script that rotates logs for a given application. Keep the last 7 days of logs and delete older logs.
<details>
<summary>Answer</summary>

```bash
#!/bin/bash
log_dir=$1
find $log_dir -type f -name "*.log" -mtime +7 -exec rm {} \;
```
</details>

**Q21:** **Check System Uptime**
- Write a Bash script that checks the system uptime and sends an alert if the system has been up for more than a specified number of days.
<details>
<summary>Answer</summary>

```bash
#!/bin/bash
threshold_days=$1
uptime_days=$(awk '{print int($1/86400)}' /proc/uptime)
if [ $uptime_days -gt $threshold_days ]; then
  echo "System has been up for more than $threshold_days days" | mail -s "Uptime Alert" user@example.com
fi
```
</details>

**Q22:** **Monitor User Logins**
- Write a Bash script that monitors user logins and sends an email alert when a specific user logs in.
<details>
<summary>Answer</summary>

```bash
#!/bin/bash
user=$1
if who | grep -q $user; then
  echo "$user has logged in" | mail -s "Login Alert" user@example.com
fi
```
</details>

**Q23:** **Create a Menu-Driven Program**
- Write a Bash script that presents a menu to the user with options to display date, list files, show free memory, and exit. Implement the menu using a while loop and case statement.
<details>
<summary>Answer</summary>

```bash
#!/bin/bash
while true; do
  echo "1. Display Date"
  echo "2. List Files"
  echo "3. Show Free Memory"
  echo "4. Exit"
  read -p "Choose an option: " option
  case $option in
    1) date ;;
    2) ls ;;
    3) free -h ;;
    4) break ;;
    *) echo "Invalid option" ;;
  esac
done
```
</details>

**Q24:** **Script to Compress Old Files**
- Write a Bash script that compresses files older than 30 days in a given directory into a tar.gz archive.
<details>
<summary>Answer</summary>

```bash
#!/bin/bash
dir=$1
find $dir -type f -mtime +30 -print0 | tar -czvf archive_$(date +%F).tar.gz --null -T -
```
</details>

**Q25:** **Generate a Report of Large Files**
- Write a Bash script that generates a report of files larger than a specified size in a given directory.
<details>
<summary>Answer</summary>

```bash
#!/bin/bash
dir=$1
size=$2
find $dir -type f -size +${size}c -exec ls -lh {} \; | awk '{ print $9 ": " $5 }'
```
</details>

This comprehensive QnA question bank prompts users to apply everything they have learned in the course, covering arrays, loops, functions, conditionals, file operations, regular expressions, and more. If you need any more questions or further details, let me know!
