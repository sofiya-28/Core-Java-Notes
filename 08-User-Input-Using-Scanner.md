# Chapter 08 - User Input Using Scanner Class (Part 1)

## Table of Contents

1. What is User Input?
2. Why Do We Need User Input?
3. Scanner Class
4. Importing Scanner Class
5. Creating Scanner Object
6. Reading Integer Input
7. Java Example
8. Important Notes
9. Common Beginner Mistakes
10. Interview Questions
11. Summary

---

# What is User Input?

## English
User Input means taking data from the user while the program is running.
Instead of using fixed values inside the program, the user can enter values at runtime.

## Hindi
User Input ka matlab hai program chalne ke samay user se data lena.
Fixed values likhne ki jagah user khud value enter karta hai.

---

# Why Do We Need User Input?

## English
User Input makes programs dynamic and interactive.
It allows users to enter different values every time the program runs.
Without User Input, the program always works with fixed values.

## Hindi
User Input program ko dynamic aur interactive banata hai.
Har baar program chalane par user alag-alag values enter kar sakta hai.
Agar User Input na ho, to program hamesha fixed values ke sath hi chalega.

---

# What is Scanner Class?

## English
Scanner is a predefined class in Java.
It is used to take input from the keyboard.
The Scanner class belongs to the `java.util` package.

## Hindi
Scanner Java ki ek predefined class hai.
Iska use keyboard se input lene ke liye kiya jata hai.
Scanner Class `java.util` package ka part hai.

---

# Importing Scanner Class
Before using Scanner, we must import it.
Syntax

```java
import java.util.Scanner;
```

---

## English
The import statement tells Java to use the Scanner class.

## Hindi
Import statement Java ko batata hai ki Scanner Class ka use karna hai.

---

# Creating Scanner Object

Syntax
```java
Scanner sc = new Scanner(System.in);
```

---

## English
Here,
- Scanner → Class Name
- sc → Object Name
- new → Creates a new object
- System.in → Takes input from the keyboard

## Hindi
Yahan,
- Scanner → Class ka naam hai.
- sc → Object ka naam hai.
- new → Naya object banata hai.
- System.in → Keyboard se input leta hai.

---

# Reading Integer Input

Syntax
```java
int number = sc.nextInt();
```

---

## English
`nextInt()` is used to read an integer value from the keyboard.

## Hindi
`nextInt()` ka use keyboard se integer value lene ke liye kiya jata hai.

---

# Example Program

```java
import java.util.Scanner;

public class UserInput {

    public static void main(String[] args) {

        Scanner sc = new Scanner(System.in);

        System.out.print("Enter Your Age: ");

        int age = sc.nextInt();

        System.out.println("Your Age is: " + age);

    }

}
```

---

# Sample Output
```
Enter Your Age: 20

Your Age is: 20
```

---

# Program Explanation

## English
- Import the Scanner class.
- Create a Scanner object.
- Ask the user to enter age.
- Read the input using `nextInt()`.
- Display the entered value.

---

## Hindi
- Scanner Class ko import kiya.
- Scanner ka object banaya.
- User se age maangi.
- `nextInt()` se input liya.
- Input ko screen par print kiya.

---

# Memory Representation

```
Keyboard
↓
20
↓
Scanner Object (sc)
↓
age = 20
↓
Output Screen
```

---

# Important Notes
- Scanner is used for keyboard input.
- Scanner belongs to the `java.util` package.
- Always import Scanner before using it.
- Create a Scanner object before taking input.
- `nextInt()` reads integer values.

---

# Common Beginner Mistakes

Wrong
```java
Scanner sc = Scanner(System.in);
```

Correct
```java
Scanner sc = new Scanner(System.in);
```

Reason
The `new` keyword is required to create an object.

---

Wrong
```java
int age = nextInt();
```

Correct
```java
int age = sc.nextInt();
```

Reason
`nextInt()` must be called using the Scanner object.

---

Wrong
```java
Scanner sc = new Scanner();
```

Correct
```java
Scanner sc = new Scanner(System.in);
```

Reason
`System.in` is required for keyboard input.

---

# Interview Questions

## Basic
1. What is User Input?
2. What is Scanner Class?
3. Which package contains the Scanner Class?
4. Why do we import Scanner?
5. What does `nextInt()` do?

---

## Intermediate
1. Explain the Scanner Class with an example.
2. What is the purpose of `System.in`?
3. Why do we use the `new` keyword?
4. How do you create a Scanner object?
5. What happens if Scanner is not imported?

---

# Summary
- User Input allows users to enter values while the program is running.
- Scanner is a predefined class in Java.
- Scanner belongs to the `java.util` package.
- `new Scanner(System.in)` creates a Scanner object.
- `nextInt()` is used to read integer input from the keyboard.

---

# (Part-2)

In Part 2, we will study:

## Table of Contents

1. Reading Different Types of Input
2. next()
3. nextLine()
4. nextFloat()
5. nextDouble()
6. nextBoolean()
7. Reading Character Input
8. Difference Between next() and nextLine()
9. Important Notes
10. Common Beginner Mistakes
11. Interview Questions
12. Summary

---

# Reading Different Types of Input

## English
The Scanner class provides different methods to read different types of data.
Each method is used for a specific data type.

## Hindi
Scanner Class alag-alag data types ke liye alag methods provide karti hai.
Har method kisi specific data type ka input lene ke liye use hota hai.

---

# next()

## English
The `next()` method is used to read a single word.
It stops reading when a space is found.

## Hindi
`next()` method sirf ek word input leta hai.
Jaise hi space aata hai, input lena band kar deta hai.
---

Example

```java
import java.util.Scanner;

public class Demo {

    public static void main(String[] args) {

        Scanner sc = new Scanner(System.in);

        System.out.print("Enter Your Name: ");

        String name = sc.next();

        System.out.println(name);

    }

}
```

Input
```
Sofiya
```

Output
```
Sofiya
```

---

# nextLine()

## English
The `nextLine()` method reads an entire line.
It accepts spaces also.

## Hindi
`nextLine()` method poori line ko read karta hai.
Ye spaces ko bhi accept karta hai.

---

Example

```java
import java.util.Scanner;

public class Demo {

    public static void main(String[] args) {

        Scanner sc = new Scanner(System.in);

        System.out.print("Enter Full Name: ");

        String name = sc.nextLine();

        System.out.println(name);

    }

}
```

Input
```
Sofiya Malik
```

Output
```
Sofiya Malik
```

---

# nextFloat()

## English
The `nextFloat()` method is used to read float values.

## Hindi
`nextFloat()` method float value lene ke liye use hota hai.

---

Example

```java
Scanner sc = new Scanner(System.in);
float marks = sc.nextFloat();
System.out.println(marks);
```

Input
```
89.5
```

Output
```
89.5
```

---

# nextDouble()

## English
The `nextDouble()` method is used to read double values.

## Hindi
`nextDouble()` method double value lene ke liye use hota hai.

---

Example

```java
Scanner sc = new Scanner(System.in);
double salary = sc.nextDouble();
System.out.println(salary);
```

Input
```
35000.75
```

Output
```
35000.75
```

---

# nextBoolean()

## English
The `nextBoolean()` method reads boolean values.
It accepts only `true` or `false`.

## Hindi
`nextBoolean()` method boolean value leta hai.
Ye sirf `true` ya `false` accept karta hai.

---

Example

```java
Scanner sc = new Scanner(System.in);
boolean result = sc.nextBoolean();
System.out.println(result);
```

Input
```
true
```

Output
```
true
```

---

# Reading Character Input

## English
Scanner does not provide a `nextChar()` method.
To read a character, use `next().charAt(0)`.

## Hindi
Scanner me `nextChar()` method nahi hota.
Character input lene ke liye `next().charAt(0)` ka use kiya jata hai.

---

Example

```java
Scanner sc = new Scanner(System.in);
char grade = sc.next().charAt(0);
System.out.println(grade);
```

Input
```
A
```

Output
```
A
```

---

# Difference Between next() and nextLine()

| next() | nextLine() |
|----------|------------|
| Reads one word | Reads complete line |
| Stops at space | Accepts spaces |
| Used for single word | Used for full sentence |

---

Example

Input
```
Sofiya Khan
```

Using
```java
sc.next();
```

Output
```
Sofiya
```

Using
```java
sc.nextLine();
```

Output
```
Sofiya Malik
```

---

# Important Notes
- `next()` reads one word.
- `nextLine()` reads the complete line.
- `nextFloat()` reads float values.
- `nextDouble()` reads double values.
- `nextBoolean()` reads true or false.
- `next().charAt(0)` reads a single character.

---

# Common Beginner Mistakes

Wrong
```java
char ch = sc.nextChar();
```

Correct
```java
char ch = sc.next().charAt(0);
```

Reason
Scanner Class does not contain the `nextChar()` method.

---

Wrong
```java
String name = sc.next();
```

Input
```
Sofiya Malik
```

Output
```
Sofiya
```

Correct
```java
String name = sc.nextLine();
```

Output
```
Sofiya Malik
```

Reason

`next()` reads only one word.
`nextLine()` reads the complete line.

---

# Interview Questions

## Basic
1. What is the difference between `next()` and `nextLine()`?
2. Which method reads an integer?
3. Which method reads a float value?
4. Which method reads a boolean value?
5. Does Scanner provide a `nextChar()` method?

---

## Intermediate
1. Explain `nextLine()` with an example.
2. Why is `next().charAt(0)` used?
3. Which Scanner method accepts spaces?
4. Explain the difference between `next()` and `nextLine()`.
5. Name five Scanner methods used for input.

---

# Summary
- `next()` reads one word.
- `nextLine()` reads the complete line.
- `nextFloat()` reads float values.
- `nextDouble()` reads double values.
- `nextBoolean()` reads boolean values.
- `next().charAt(0)` is used to read a character.

---

# (Part-3)

## Table of Contents

1. Complete Java Program
2. Practice Programs
3. MCQs
4. Viva Questions
5. Interview Questions
6. Common Beginner Mistakes
7. Quick Revision
8. Chapter Summary

---

# Complete Java Program

```java
import java.util.Scanner;

public class ScannerDemo {

    public static void main(String[] args) {

        Scanner sc = new Scanner(System.in);

        System.out.print("Enter Your Name: ");
        String name = sc.nextLine();

        System.out.print("Enter Your Age: ");
        int age = sc.nextInt();

        System.out.print("Enter Your Height: ");
        float height = sc.nextFloat();

        System.out.print("Enter Your Percentage: ");
        double percentage = sc.nextDouble();

        System.out.print("Are You a Student (true/false): ");
        boolean student = sc.nextBoolean();

        System.out.print("Enter Your Grade: ");
        char grade = sc.next().charAt(0);

        System.out.println();

        System.out.println("----- Student Details -----");
        System.out.println("Name : " + name);
        System.out.println("Age : " + age);
        System.out.println("Height : " + height);
        System.out.println("Percentage : " + percentage);
        System.out.println("Student : " + student);
        System.out.println("Grade : " + grade);

        sc.close();

    }

}
```

---

# Sample Output

```
Enter Your Name: Sofiya
Enter Your Age: 20
Enter Your Height: 5.3
Enter Your Percentage: 87.5
Are You a Student (true/false): true
Enter Your Grade: A

----- Student Details -----

Name : Sofiya
Age : 20
Height : 5.3
Percentage : 87.5
Student : true
Grade : A
```

---

# Practice Programs

## Program 1
Take the user's name as input and print a welcome message.

Example
```
Welcome Sofiya
```

---

## Program 2
Take two integers as input and print their sum.

## Program 3
Take the length and breadth of a rectangle as input and calculate its area.
Formula
```
Area = Length × Breadth
```
## Program 4
Take the radius of a circle as input and calculate the area.
Formula
```
Area = 3.14 × r × r
```

## Program 5
Take a student's name, roll number and percentage as input and print them.

## Program 6
Take a character as input and print it.

## Program 7
Take a boolean value as input and print it.

---

# MCQs

### 1. Which package contains the Scanner class?
A. java.lang
B. java.io
C. java.util
D. java.math
Answer
```
C
```

---

### 2. Which keyword is used to create a Scanner object?
A. create
B. new
C. object
D. class
Answer
```
B
```

---

### 3. Which method reads an integer?
A. next()
B. nextInt()
C. nextLine()
D. nextDouble()
Answer
```
B
```

---

### 4. Which method reads a complete line?
A. next()
B. nextChar()
C. nextLine()
D. nextWord()
Answer
```
C
```

---

### 5. Which method is used to read a character?
A. nextChar()
B. next()
C. next().charAt(0)
D. getChar()
Answer
```
C
```

---

### 6. Which method reads a double value?
A. nextFloat()
B. nextDouble()
C. nextDecimal()
D. nextNumber()
Answer
```
B
```

---

### 7. Which method reads a boolean value?
A. nextBoolean()
B. nextBool()
C. next()
D. nextLine()
Answer
```
A
```

---

### 8. Which object is generally used for keyboard input?
A. Scanner
B. String
C. System
D. Math
Answer
```
A
```

---

### 9. Which statement imports the Scanner class?
A.
```java
import java.lang.Scanner;
```
B.
```java
import java.util.Scanner;
```
C.
```java
import Scanner;
```
D.
```java
include Scanner;
```
Answer
```
B
```

---

### 10. Which method should be called after using Scanner to release resources?
A. stop()
B. end()
C. close()
D. finish()
Answer
```
C
```

---

# Viva Questions
1. What is User Input?
2. What is the Scanner class?
3. Which package contains the Scanner class?
4. Why do we import Scanner?
5. How do you create a Scanner object?
6. What is the purpose of System.in?
7. What is the difference between next() and nextLine()?
8. Which method reads an integer?
9. Which method reads a character?
10. Why do we use close()?

---

# Interview Questions

## Basic
1. Explain the Scanner class.
2. Why is Scanner used in Java?
3. What is System.in?
4. Explain nextInt() with an example.
5. Explain nextLine() with an example.

---

## Intermediate
1. Explain the difference between next() and nextLine().
2. Why is next().charAt(0) used for character input?
3. What happens if Scanner is not imported?
4. Why should we close the Scanner object?
5. Explain different Scanner methods with examples.

---

# Common Beginner Mistakes

### Mistake 1

Wrong

```java
Scanner sc = Scanner(System.in);
```

Correct

```java
Scanner sc = new Scanner(System.in);
```

---

### Mistake 2

Wrong

```java
char ch = sc.nextChar();
```

Correct

```java
char ch = sc.next().charAt(0);
```

---

### Mistake 3

Wrong

```java
String name = sc.next();
```

Input

```
Sofiya Malik
```

Output

```
Sofiya
```

Correct

```java
String name = sc.nextLine();
```

Output

```
Sofiya Khan
```

---

### Mistake 4

Wrong

```java
Scanner sc = new Scanner(System.in);

// Input

int age = sc.nextInt();
String name = sc.nextLine();
```

Problem

`nextLine()` may read the leftover newline character instead of the actual input.

Correct

```java
Scanner sc = new Scanner(System.in);

int age = sc.nextInt();
sc.nextLine();

String name = sc.nextLine();
```

---

# Quick Revision
- Scanner is used for taking input from the keyboard.
- Scanner belongs to the `java.util` package.
- Import Scanner before using it.
- Create an object using `new Scanner(System.in)`.
- `nextInt()` reads integer values.
- `nextFloat()` reads float values.
- `nextDouble()` reads double values.
- `nextBoolean()` reads boolean values.
- `next()` reads one word.
- `nextLine()` reads the complete line.
- `next().charAt(0)` reads a single character.
- Use `close()` after completing input.

---

# Chapter Summary
In this chapter, we learned:
- What is User Input
- Scanner Class
- Importing Scanner
- Creating Scanner Object
- Integer Input
- Float Input
- Double Input
- Boolean Input
- Character Input
- String Input
- Difference Between next() and nextLine()
- Java Programs
- Practice Programs
- MCQs
- Viva Questions
- Interview Questions

The Scanner class is one of the most frequently used classes in Java because almost every interactive program requires user input.

---