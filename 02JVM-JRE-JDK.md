#  Chapter 2: JVM, JRE, JDK & Java Compilation Process

#  Table of Contents
1. Introduction
2. What is JVM?
3. What is JRE?
4. What is JDK?
5. Difference Between JVM, JRE & JDK
6. Java Compilation Process
7. Platform Independence
8. Real-Life Example
9. Memory Diagram
10. Interview Questions
11. MCQs
12. Practice Questions
13. Summary

# 1️  Introduction

Whenever we write a Java program, the computer **cannot understand Java code directly**.
Java code must be converted into **Machine Code (0 & 1)** before execution.
Three important components help us:

- JVM
- JRE
- JDK

# 2️ What is JVM?
##  English
JVM (Java Virtual Machine) is a virtual machine that executes Java Bytecode and converts it into Machine Code.
It is responsible for running Java programs.

## 🇮🇳 Hindi
JVM (Java Virtual Machine) ek virtual machine hai jo Java Bytecode ko Machine Code me convert karti hai aur Java Program ko execute karti hai.

##  Responsibilities of JVM
- Loads Class Files
- Verifies Bytecode
- Executes Program
- Converts Bytecode into Machine Code
- Memory Management
- Garbage Collection

##  JVM Diagram

```
Bytecode (.class)
        │
        ▼
+----------------+
|      JVM       |
+----------------+
        │
        ▼
 Machine Code
        │
        ▼
      Output
```

# 3️ What is JRE?

## English
JRE (Java Runtime Environment) provides the environment required to run Java applications.
It contains:

- JVM
- Java Libraries
- Supporting Runtime Files

## 🇮🇳 Hindi
JRE Java Program ko run karne ke liye environment provide karta hai.
Isme JVM aur Java Libraries hoti hain.

##  Formula

```
JRE = JVM + Libraries + Runtime Files
```

# 4️ What is JDK?

## English
JDK (Java Development Kit) is used to develop, compile and run Java programs.
It contains

- JRE
- JVM
- Compiler
- Debugger
- Development Tools

## 🇮🇳 Hindi
JDK Java Developer ke liye complete package hai.
Iski help se hum Java Program likh sakte hain, compile kar sakte hain aur run bhi kar sakte hain.

##  Formula

```
JDK = JRE + Development Tools
```

# Relationship Diagram

```
+--------------------------------------+
|                 JDK                  |
|                                      |
|   +------------------------------+   |
|   |             JRE              |   |
|   |                              |   |
|   |      +----------------+      |   |
|   |      |      JVM       |      |   |
|   |      +----------------+      |   |
|   |     Libraries + Runtime      |   |
|   +------------------------------+   |
| Compiler • Debugger • Tools          |
+--------------------------------------+
```
# 5️ Difference Between JVM, JRE & JDK

| Feature | JVM | JRE | JDK |
|----------|-----|-----|-----|
| Full Form | Java Virtual Machine | Java Runtime Environment | Java Development Kit |
| Used For | Run Bytecode | Run Java Program | Develop Java Program |
| Compiler | ❌ | ❌ | ✅ |
| JVM Included | — | ✅ | ✅ |
| Libraries | ❌ | ✅ | ✅ |
| Development Tools | ❌ | ❌ | ✅ |

---

# 6️ Java Compilation Process

## Step 1

Write Java Program

```
Hello.java
```

↓

## Step 2

Compile

```
javac Hello.java
```

↓

## Step 3

Compiler generates

```
Hello.class
```

↓

## Step 4

JVM loads Bytecode

↓

## Step 5

JVM converts Bytecode into Machine Code

↓

## Step 6

Output

# Java Compilation Flow

```
Java Source Code (.java)
          │
          ▼
Java Compiler (javac)
          │
          ▼
Bytecode (.class)
          │
          ▼
        JVM
          │
          ▼
Machine Code
          │
          ▼
        Output
```

# 7️ Why Java is Platform Independent?

Java Compiler always generates **Bytecode**.
Every Operating System has its own JVM.
Therefore the same Bytecode can run everywhere.
This is called
> **Write Once Run Anywhere (WORA)**

#  Real-Life Example
Imagine you write a letter in English.
Different countries understand different languages.
A translator converts the letter into the local language.

Similarly

```
Java Program
      │
      ▼
   Bytecode
      │
      ▼
      JVM
      │
      ▼
Machine Language
```

JVM acts as a Translator.

#  Important Points

✅ JVM executes Bytecode.
✅ JRE provides Runtime Environment.
✅ JDK is used for Development.
✅ JDK contains JRE.
✅ JRE contains JVM.

#  Exam Notes

Remember these formulas:

```
JRE = JVM + Libraries

JDK = JRE + Development Tools
```

# Common Mistakes

wrong:    JVM compiles Java code.
Right:    Compiler compiles Java code.
          JVM executes Bytecode.

Wrong:    JRE contains Compiler.
Right:    Compiler is available inside JDK.

# Interview Questions

## Basic
1. What is JVM?
2. What is JRE?
3. What is JDK?
4. What is Bytecode?
5. What is javac?

## Intermediate
1. Explain Java Compilation Process.
2. Why is Java Platform Independent?
3. Difference between JVM and JRE.
4. Difference between JDK and JRE.
5. Explain JVM Architecture (Basic).

#  MCQs
### Q1. JVM is used for
A. Writing Java Code
B. Compiling Java Code
C. Executing Bytecode    (Correct)
D. Creating Variables

### Q2. Which tool compiles Java Program?
A. JVM
B. JRE
C. javac    (Correct)
D. java

### Q3. Which contains JVM?
A. Compiler
B. Bytecode
C. JRE       (Correct)
D. Source Code

### Q4. JDK contains
A. JVM Only
B. JRE Only
C. JRE + Development Tools     (Correct)
D. Bytecode

#  Practice Questions
1. Define JVM.
2. Define JRE.
3. Define JDK.
4. Explain Java Compilation Process.
5. Draw JVM, JRE and JDK Diagram.
6. Why Java is Platform Independent?

#  Quick Revision
✔ JVM → Executes Bytecode
✔ JRE → Runtime Environment
✔ JDK → Development Kit
✔ javac → Compiler
✔ java → Runs Program
✔ Bytecode → .class
✔ Source File → .java

#  Summary
- JVM executes Java Bytecode.
- JRE provides runtime environment.
- JDK is used to develop Java applications.
- Java Compiler converts .java into .class.
- JVM converts Bytecode into Machine Code.
- Java is Platform Independent because of JVM.

-----