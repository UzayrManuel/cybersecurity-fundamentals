# 🐧 Linux Fundamentals

This file covers essential Linux commands often used in cybersecurity, ethical hacking, and system administration. Understanding these commands is key when navigating a Linux system, running tools, or analyzing outputs during CTFs and penetration testing.

---

## 📘 Common Linux Commands

| Command | Full Name             | Purpose / Use |
|---------|------------------------|----------------|
| `echo`  | Echo                   | Outputs text or variables to the terminal |
| `whoami`| Who Am I               | Displays the current user |
| `ls`    | List                   | Lists files and directories |
| `cd`    | Change Directory       | Navigates between directories |
| `cat`   | Concatenate            | Displays the contents of a file |
| `pwd`   | Print Working Directory| Shows the current directory path |
| `find`  | Find                   | Searches for files and directories |
| `grep`  | Global Regular Expression Print | Searches for patterns within files |
| `&`     | Background Execution   | Runs a process in the background |
| `&&`    | AND Operator           | Chains commands, runs second only if first succeeds |
| `>`     | Output Redirection     | Overwrites a file with command output |
| `>>`    | Append Redirection     | Appends command output to a file |

---

## 🧪 Command Examples

```bash
# echo
echo "Hello, Hacker"
# Output: Hello, Hacker

# whoami
whoami
# Output: uzayr (or your current user)

# ls
ls
# Output: Lists files in the current directory

# cd
cd /etc
# Changes to the /etc directory

# cat
cat file.txt
# Prints the content of file.txt

# pwd
pwd
# Output: /home/uzayr/Documents

# find
find /home -name "*.txt"
# Finds all .txt files under /home

# grep
grep "password" secrets.txt
# Finds the word "password" in secrets.txt

# &
ping 8.8.8.8 &
# Runs ping in the background

# &&
mkdir test && cd test
# Makes a directory and enters it only if creation succeeds

# >
echo "This is a test" > notes.txt
# Overwrites notes.txt with the string

# >>
echo "Another line" >> notes.txt
# Appends the string to notes.txt
