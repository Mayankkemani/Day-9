# Day 09 - Bash Conditions & Loops 🚀

## Overview

Today I learned Bash conditional statements and loops. I practiced taking user input, comparing values, checking file existence, and using for loops with ranges and step values.

---

# Bash Conditional Statements

## if-else Syntax

```bash
#!/bin/bash

num=10

if [ $num -gt 5 ]
then
    echo "Greater"
else
    echo "Smaller"
fi
```

---

## Comparison Operators

```text
-eq  Equal To
-ne  Not Equal To
-gt  Greater Than
-lt  Less Than
-ge  Greater Than or Equal To
-le  Less Than or Equal To
```

---

## User Input with if-else

```bash
#!/bin/bash

echo "Enter your age:"
read age

if [ $age -ge 18 ]
then
    echo "Adult"
else
    echo "Minor"
fi
```

Example Output:

```text
Enter your age:
20

Adult
```

---

# Even and Odd Number Check

```bash
#!/bin/bash

echo "Enter a number:"
read num

if [ $((num % 2)) -eq 0 ]
then
    echo "Even Number"
else
    echo "Odd Number"
fi
```

---

# File Existence Check

```bash
#!/bin/bash

if [ -f kk.txt ]
then
    echo "File Exists"
else
    echo "File Not Found"
fi
```

---

# Bash For Loops

## Basic For Loop

```bash
#!/bin/bash

for i in 1 2 3 4 5
do
    echo $i
done
```

Output:

```text
1
2
3
4
5
```

---

## Loop with Names

```bash
#!/bin/bash

for user in Rahul Amit Rohit
do
    echo "Welcome $user"
done
```

---

## Range Loop

```bash
#!/bin/bash

for i in {1..10}
do
    echo $i
done
```

Output:

```text
1
2
3
4
5
6
7
8
9
10
```

---

## Step Values

Odd Numbers:

```bash
for i in {1..10..2}
do
    echo $i
done
```

Output:

```text
1
3
5
7
9
```

Even Numbers:

```bash
for i in {2..10..2}
do
    echo $i
done
```

Output:

```text
2
4
6
8
10
```

---

# Simple Backup Script

```bash
#!/bin/bash

echo "Enter file name:"
read file

if [ -f $file ]
then
    cp $file $file.bak
    echo "Backup Created"
else
    echo "File Not Found"
fi
```

---

# Commands Practiced

```bash
read
if
else
fi
for
cp
echo
```

---

# Skills Learned Today

✅ Bash Conditions

✅ Comparison Operators

✅ User Input Handling

✅ File Checking

✅ For Loops

✅ Range Loops

✅ Step Values

✅ Basic Automation

---

# Learning Summary

Today I learned how to make decisions in Bash scripts using if-else conditions and how to automate repetitive tasks using for loops. I also practiced file checking and created a simple backup script, which are useful concepts for Linux administration and DevOps automation.

---

# DevOps Roadmap Progress

```text
✅ Linux Fundamentals
✅ File System
✅ Permissions
✅ Ownership
✅ Package Management
✅ Users & Groups
✅ Processes
✅ Services
✅ SSH & SCP
✅ Bash Basics
✅ Bash Conditions
✅ Bash Loops

✅ Python Variables
✅ Data Types
✅ Input
✅ if/else
✅ For Loop
✅ While Loop
✅ Functions

🔜 Bash While Loop
🔜 Git & GitHub
🔜 Networking
🔜 AWS
🔜 Docker
```

Day 09 Complete 🚀
