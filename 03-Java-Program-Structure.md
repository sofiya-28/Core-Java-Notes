#  Chapter 03: Java Program Structure (Part 1)
# (part-1)

#  Table of Contents (Part 1)

1. What is Java Program Structure?
2. Why Do We Need Program Structure?
3. Basic Structure of a Java Program
4. Explanation of Every Component
5. Understanding the `main()` Method
6. Program Execution Flow
7. Real-Life Example
8. Memory Trick
9. Important Notes
10. Quick Interview Questions

---

# 1 What is Java Program Structure?

##  English
A Java Program Structure is the standard format or layout of a Java program.
It defines how different parts of a Java program are arranged so that the Java compiler can understand and execute it correctly.
Every Java program follows a fixed structure.

##  Hindi
Java Program Structure ka matlab hai **Java program likhne ka standard format**.
Is format ki help se compiler samajhta hai ki program kahan se start hoga aur kis order me execute hoga.
Har Java program ek fixed structure follow karta hai.

#  Exam Definition
**Java Program Structure** is the standard layout of a Java program that contains package declaration, import statements, class declaration, methods, and program statements.

# 2  Why Do We Need Program Structure?
Imagine you want to build a house.
Without a proper design,

 Rooms may overlap.

 Doors may be missing.

 The house will not be built properly.

Similarly,
If we don't follow Java Program Structure,
- Compiler gets confused.
- Errors occur.
- Program cannot execute properly.
Therefore,

> **Program Structure makes the code organized, readable and executable.**

#  Real-Life Example
Suppose you want to write an exam.
First,
✔ Write your Roll Number
Then,
✔ Write your Name
Then,
✔ Start writing answers.
If you directly start writing answers,
the teacher may reject your answer sheet.
Similarly,
Java also expects a  proper sequence.

# 3 Basic Structure of a Java Program
```java
package packageName;

import packageName.*;

public class ClassName {

    public static void main(String[] args) {

        // Statements

    }

}
```

#  Java Program Structure Diagram

```
                 Java Program

                      │
     ┌────────────────┼────────────────┐
     │                │                │
 Package          Import          Class
                                      │
                                      ▼
                          main() Method
                                      │
                                      ▼
                              Statements
                                      │
                                      ▼
                                 Output
```

# 4 Components of Java Program
A Java program mainly consists of the following components.

| Component | Required | Purpose |
|-----------|----------|---------|
| Package | Optional | Organizes classes |
| Import | Optional | Imports predefined classes |
| Class | Mandatory | Blueprint of program |
| main() Method | Mandatory | Starting point of execution |
| Statements | Mandatory | Instructions for execution |


# 5  Package Declaration
## English
Package is used to organize Java classes.
It helps in managing large projects.
Syntax:

```java
package mypackage;
```

## Hindi
Package ka use classes ko organize karne ke liye kiya jata hai.
Agar project bada ho,
to package code ko manage karne me help karta hai.

### Important Point
Package declaration should always be the first statement in a Java program.

# 6 Import Statement

## English
Import statement allows us to use predefined Java classes without writing their complete package names.
Example:

```java
import java.util.Scanner;
```

## Hindi
Import statement ki help se hum Java ki predefined classes ko use kar sakte hain.
Jaise
Scanner class.

### Why Scanner?
Scanner is used to take input from the user.
Without import,
Java compiler cannot recognize Scanner.

# 7 Class Declaration
## English
A class is a blueprint for creating objects.
Every Java program must contain at least one class.
Syntax:

```java
class Student
{

}
```

## Hindi
Class ek blueprint hoti hai.
Object isi class se bante hain.
Har Java program me kam se kam ek class zaroor hoti hai.

#  Why Class is Necessary?
Java is an Object-Oriented Programming Language.
Everything is written inside a class.
Without a class,
Java program cannot execute.

# 8 Understanding the main() Method
This is the most important part of every Java program.
Syntax:

```java
public static void main(String[] args)
{

}
```
This method is called automatically by the JVM when the program starts.

## Hindi
main() Java program ka entry point hai.
Execution hamesha isi method se start hoti hai.
Program me chahe kitni bhi methods ho,
JVM sabse pehle **main()** ko hi call karta hai.

#  Important Point
> **No main() Method = No Program Execution**

#  Memory Trick

Remember the order using:

### **P I C M S**
```
P → Package
I → Import
C → Class
M → main()

S → Statements
```

#  Interview Questions

### Basic
**Q1. What is Java Program Structure?**
**Q2. Why is Program Structure important?**
**Q3. Which component is mandatory in Java?**
**Q4. What is the purpose of Package?**
**Q5. What is the purpose of Import statement?**
**Q6. Why is Class necessary in Java?**
**Q7. Which method is called first by JVM?**

#  Summary 
- Java follows a fixed program structure.
- Package organizes classes.
- Import allows using predefined classes.
- Every Java program must contain a class.
- Execution always starts from the `main()` method.
- Statements are written inside the `main()` method.
- The correct order is: **Package → Import → Class → main() → Statements.

# (part-2)  

#  Table of Contents (Part 2)

1. Complete Explanation of `main()` Method
2. First Java Program
3. Line-by-Line Explanation
4. Java Comments
5. Rules for Writing Java Programs
6. Java Naming Conventions
7. Program Execution Flow
8. Common Beginner Mistakes
9. Important Notes
10. Quick Interview Questions

# 9 Complete Explanation of `main()` Method

The syntax of the `main()` method is:

```java
public static void main(String[] args)
{
    // Statements
}
```

This is the entry point of every Java application.
When we run a Java program, **JVM always calls the `main()` method first.**

# Understanding Every Keyword

## 1. public

`public` is an access modifier.
It allows the JVM to access the `main()` method from anywhere.
(`public` ek Access Modifier hai.
 Ye JVM ko `main()` method ko access karne ki permission deta hai.)

## 2. static

`static` means the method belongs to the class, not to an object.
Therefore, JVM can call it without creating an object.
(`static` ka matlab hai ki method class ka hissa hai.
Isliye object banaye bina bhi JVM ise call kar sakti hai.)

---

## 3. void

`void` means the method does not return any value.
(`void` ka matlab hai ki method koi value return nahi karta.)

## 4. main

`main` is the predefined method name recognized by JVM.
Program execution always starts from this method.
(`main` ek predefined method hai. Program ki execution hamesha isi method se start hoti hai.)

## 5. String[] args

It stores command-line arguments passed to the program.
Beginners usually don't use it in simple programs, but it is required in the method signature.
(Ye command-line arguments ko store karta hai.
Abhi beginners isse use nahi karte, lekin `main()` method me ise likhna zaroori hota hai.)

#  Memory Trick
Remember:
**PSVMS**

```
P → Public
S → Static
V → Void
M → Main
S → String[] args
```

# 10 First Java Program

```java
public class HelloWorld {

    public static void main(String[] args) {

        System.out.println("Hello, World!");

    }

}
```

# Output

```
Hello, World!
```

# Line-by-Line Explanation

### Line 1

```java
public class HelloWorld
```
A class named **HelloWorld** is created.

### Line 2

```java
{
```

Opening brace indicates the beginning of the class.

### Line 3

```java
public static void main(String[] args)
```
The JVM starts executing the program from this method.

### Line 4

```java
{
```

Beginning of the `main()` method.

### Line 5

```java
System.out.println("Hello, World!");
```

Prints the message on the console.

### Line 6

```java
}
```

End of the `main()` method.

### Line 7
```java
}
```
End of the class.
# 1(1) Java Comments
Comments are used to explain the code.
The compiler ignores comments.

## Single-Line Comment

```java
// This is a comment
```


## Multi-Line Comment

```java
/*
This is
a multi-line
comment
*/
```
## Documentation Comment

```java
/**
 * Documentation Comment
 */
```

This is mainly used while creating Java APIs and professional projects.

#  Hindi
Comments ka use code ko samjhane ke liye kiya jata hai.
Compiler comments ko ignore kar deta hai.

# 1(2) Rules for Writing Java Programs

✔ File name and public class name must be the same.

Example:

```
HelloWorld.java
```

```java
public class HelloWorld
```

✔ Every Java statement ends with a semicolon (`;`).

Example:

```java
System.out.println("Hello");
```

✔ Java is Case Sensitive.

Example:

```java
main
```

and

```java
Main
```

are different.
✔ Curly braces `{}` define blocks of code.

✔ Every Java program must have at least one class.

# 1(3) Java Naming Conventions
Following naming conventions makes the code clean and professional.

| Element | Convention | Example |
|----------|------------|---------|
| Class | PascalCase | StudentDetails |
| Method | camelCase | calculateMarks() |
| Variable | camelCase | studentName |
| Constant | UPPER_CASE | MAX_SIZE |
| Package | lowercase | java.util |

#  Real-Life Example
Imagine a school.
- Package → School Building
- Class → Classroom
- Method → Teacher
- Statements → Instructions given by the Teacher
Without a classroom, teaching cannot happen.
Similarly, without a class, Java code cannot run.

#  Program Execution Flow

```
Program Starts
       │
       ▼
 JVM Searches main()
       │
       ▼
 main() Method Found
       │
       ▼
 Executes Statements
       │
       ▼
 Program Ends
```

#  Common Beginner Mistakes

 Writing `Main` instead of `main`
 Forgetting `static`
 Forgetting semicolon (`;`)
 File name different from public class name
 Missing curly braces
 Writing code outside the class

#  Important Notes

- `main()` is the entry point of every Java application.
- Java is case-sensitive.
- A public class name should match the file name.
- Comments improve code readability.
- `System.out.println()` prints output and moves the cursor to the next line.

#  Interview Questions 

### Basic
1. Why is the `main()` method important?
2. What is the purpose of the `public` keyword?
3. Why do we use `static` in `main()`?
4. What is the meaning of `void`?
5. What is `String[] args`?

### Intermediate
1. Explain every keyword of the `main()` method.
2. Why should the file name match the public class name?
3. What is the difference between single-line and multi-line comments?
4. What happens if the `main()` method is missing?

# (part-3)

#  Important Definitions   (Java Program Structure)

Java Program Structure is the standard layout of a Java program that helps the compiler understand and execute the program correctly.
(Java Program Structure ek standard format hai jisme Java program likha jata hai, taaki compiler usse sahi tarike se samajh aur execute kar sake.)

## Package

A package is a collection of related Java classes and interfaces.
(Package related classes aur interfaces ka collection hota hai.)

## Import

Import is used to access predefined classes from Java libraries.
(Import ka use Java ki predefined classes ko use karne ke liye kiya jata hai.)

## Class

A class is a blueprint used to create objects.
(Class ek blueprint hoti hai jiske basis par objects banaye jate hain.)

## main() Method

The `main()` method is the entry point of every Java application.
(`main()` method Java program ka starting point hota hai.)

#  Real-Life Example

Think of a school.

```
School
   │
   ▼
Classroom
   │
   ▼
Teacher
   │
   ▼
Students
```

Similarly,

```
Package
   │
   ▼
Class
   │
   ▼
main() Method
   │
   ▼
Statements
```

Everything follows a proper order.


#  Viva Questions

### Basic Viva

**Q1. What is Java Program Structure?**
**Answer:**
It is the standard format of writing a Java program.

**Q2. Which method is executed first in Java?**
**Answer:**
`main()` Method.

**Q3. Why is `main()` called the entry point?**
**Answer:**
Because JVM starts executing the program from the `main()` method.

**Q4. Is Package compulsory?**
**Answer:**
No.

**Q5. Is Import compulsory?**
**Answer:**
No.

**Q6. Is Class compulsory?**
**Answer:**
Yes.

**Q7. Is `main()` compulsory?**
**Answer:**
Yes, for standalone Java applications.

# Interview Questions

## Beginner Level
1. Explain Java Program Structure.
2. What is the role of the `main()` method?
3. Explain the `public` keyword.
4. Explain the `static` keyword.
5. Explain the `void` keyword.
6. What is `String[] args`?
7. Why is Java case-sensitive?
8. Explain Java comments.
9. Why should the file name and class name be the same?
10. What is the purpose of `System.out.println()`?

## Intermediate Level
1. Explain every component of a Java program.
2. Explain the execution flow of a Java program.
3. Differentiate Package and Import.
4. What happens if the `main()` method is removed?
5. Can we write multiple classes in one Java file?

#  MCQs

### Q1. Which method is the entry point of a Java program?
- A. start()
- B. execute()
- C. main()     (Correct)
- D. run()

### Q2. Which keyword allows JVM to access the `main()` method?
- A. static
- B. public    (Correct)
- C. private
- D. final

### Q3. Which keyword means "no return value"?
- A. null
- B. return
- C. void     (Correct)
- D. static

### Q4. Java is a ______ language.
- A. Case Insensitive
-  B. Case Sensitive      (Correct)
- C. Machine
- D. Assembly

### Q5. Which statement prints output?
- A. print.output()
- B. output.print()
- C. System.out.println()    (Correct)
- D. display()

### Q6. Which symbol ends a Java statement?
- A. :
- B. ,
- C. ;        (Correct)
- D. .

### Q7. Which of the following is mandatory?
- A. Package
- B. Import
- C. Class     (Correct)
- D. Documentation Comment

### Q8. Which comment is used for documentation?
- A. //
- B. /*
- C. /**      (Correct)
- D. #

### Q9. Java is ______.
- A. Case Ignored
- B. Case Sensitive    (Correct)
- C. No Case
- D. None

### Q10. JVM starts execution from:
- A. Constructor
- B. Class
- C. main()    (Correct)
- D. Package

# Practice Questions

### Short Questions
1. Define Java Program Structure.
2. Explain Package.
3. Explain Import.
4. What is a Class?
5. What is the purpose of `main()`?

### Long Questions
1. Explain the complete Java Program Structure with a diagram.
2. Explain every keyword of the `main()` method.
3. Write a Java program to print "Hello World".
4. Explain Java comments with examples.
5. Explain Java naming conventions.

# Common Errors & Solutions

| Error | Reason | Solution |
|--------|---------|----------|
| Main instead of main | Case-sensitive language | Write `main` correctly |
| Missing semicolon | Statement not terminated | Add `;` |
| File name mismatch | File and class names differ | Keep both names same |
| Code outside class | Invalid program structure | Write code inside the class |
| Missing braces | Incorrect block structure | Use `{}` properly |

#  Exam Tips

Remember the order:

```
Package
   ↓
Import
   ↓
Class
   ↓
main()
   ↓
Statements
```

#  Chapter Summary

- Java follows a fixed program structure.
- Package organizes related classes.
- Import allows using predefined classes.
- Class is mandatory.
- `main()` is the entry point.
- Execution always starts from the `main()` method.
- Java is case-sensitive.
- Every statement ends with a semicolon (`;`).

#  Quick Revision

✔ Java Program Structure
✔ Package
✔ Import
✔ Class
✔ main()
✔ public
✔ static
✔ void
✔ String[] args
✔ Comments
✔ Naming Conventions
✔ Execution Flow
✔ Case Sensitive
✔ Semicolon (`;`)

#  Chapter Sheet

```
Java Program
│
├── Package (Optional)
├── Import (Optional)
├── Class (Mandatory)
│
└── main() Method (Mandatory)
│
└── Statements
↓
Output
```
> Complete chapter03<
----