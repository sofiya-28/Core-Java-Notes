#  Chapter 04: Variables 

# (Part 1)

#  Table of Contents (Part 1)

1. What is a Variable?
2. Why Do We Need Variables?
3. Real-Life Example
4. Declaration of Variables
5. Initialization of Variables
6. Declaration vs Initialization
7. Rules for Naming Variables
8. Memory Representation
9. Important Notes
10. Interview Questions

# 1  What is a Variable?

##  English
A **Variable** is a named memory location used to store data temporarily during program execution.
The value stored inside a variable can change during the execution of the program.

##  Hindi
**Variable** memory ka ek named location hota hai jahan hum data ko temporarily store karte hain.
Program chalne ke dauran variable ki value badal bhi sakti hai.

#  Exam Definition
A variable is a named memory location used to store data, and its value can change during program execution.

# 2 Why Do We Need Variables?
Imagine you want to store your age.
Without a variable:

```text
20
```

After one year,

```text
21
```

Agar data ko store hi na karein, to program us value ko yaad nahi rakh sakta.

Variables help us store, update and use data whenever required.

#  Real-Life Example
Imagine a water bottle.

```
Bottle
   │
   ▼
Stores Water
```

Similarly,

```
Variable
   │
   ▼
Stores Data
```
Bottle ka naam alag ho sakta hai.

Variable ka bhi naam hota hai.

Example:

```
age
marks
salary
name
```

# 3 Declaration of Variable

##  English
Variable declaration means creating a variable by specifying its data type and name.
Syntax::
```java
dataType variableName;
```

Example:
```java
int age;
```

##  Hindi
Declaration ka matlab hai variable banana.
Isme hum uska data type aur naam likhte hain.
Example:

```java
int age;
```

Yahan

- int → Data Type
- age → Variable Name

# 4 Initialization of Variable

##  English

Initialization means assigning a value to a variable.

Syntax

```java
variableName = value;
```

Example

```java
age = 20;
```

## Hindi
Initialization ka matlab hai variable ke andar value store karna.

Example:

```java
age = 20;
```

Ab age ke andar 20 store ho gaya.

# 5 Declaration + Initialization Together

Instead of writing two statements,

```java
int age;
age = 20;
```

We can write

```java
int age = 20;
```

This is the most commonly used way.

---

#  Memory Representation

```text
Variable

age

↓

+-------+
|  20   |
+-------+
```

Memory stores the value.

The variable name points to that memory location.

---

# 6 Rules for Naming Variables

*  Variable name can contain:

- Letters (A-Z, a-z)
- Digits (0-9)
- Underscore (_)
- Dollar Sign ($)

Example

```java
studentName
age
_marks
price1
$total
```

* Variable name cannot

Start with a number.

Wrong

```java
int 1age;
```

Correct

```java
int age1;
```

* Spaces are not allowed.

Wrong

```java
student name
```

Correct

```java
studentName
```

* Java Keywords cannot be used.

Wrong

```java
int class;
```

Correct

```java
int studentClass;
```


# Important Notes

- Variable names should be meaningful.
- Java is case-sensitive.

Example

```java
age
Age
AGE
```

All three are different variables.

#  Memory Trick

Remember:

**D → I → U**

```
D → Declare
I → Initialize
U → Use
```

Always follow this sequence while writing programs.

#  Interview Questions (Part 1)

### Basic
1. What is a Variable?
2. Why do we use Variables?
3. What is Variable Declaration?
4. What is Variable Initialization?
5. What is the difference between Declaration and Initialization?
6. Can a variable name start with a number?
7. Is Java case-sensitive?

#  Summary (Part 1)
- Variable is a named memory location.
- Variables store data temporarily.
- Declaration creates a variable.
- Initialization assigns a value.
- Variable names must follow Java naming rules.
- Java is case-sensitive.

# (Prat-2)

# Table of Contents (Part 2)

1. Types of Variables
2. Local Variable
3. Instance Variable
4. Static Variable
5. Scope of Variables
6. Lifetime of Variables
7. Comparison Table
8. Code Examples
9. Real-Life Example
10. Important Notes
11. Interview Questions

# 7 Types of Variables

Java mainly has **three types of variables**.

```
               Variables
                   │
     ┌─────────────┼─────────────┐
     │             │             │
 Local       Instance       Static
 Variable     Variable      Variable
```

# 1. Local Variable

##  English
A Local Variable is declared inside a method, constructor, or block.
It can be used only inside that method.

##  Hindi
Local Variable kisi method ya block ke andar declare kiya jata hai.
Iska use sirf usi method ke andar kiya ja sakta hai.

### Example

```java
public class Student {

    public static void main(String[] args) {

        int age = 20;

     System.out.println(age);

    }

}
```

### Memory Representation

```
main()

│

└── age = 20
```

When the method finishes,
the local variable is automatically destroyed.

# 2. Instance Variable

##  English
An Instance Variable is declared inside a class but outside all methods.
Every object gets its own copy of the instance variable.

## Hindi
Instance Variable class ke andar aur methods ke bahar declare kiya jata hai.
Har object ki apni alag copy hoti hai.

### Example

```java
class Student {

    String name;

}
```

Here,

`name` is an Instance Variable.

### Memory Representation

```
Student Object

+------------+

name = Sofiya

+------------+
```

Another object

```
Student Object

+------------+

name = Rahul

+------------+
```
Both objects have different values.

# 3. Static Variable

##  English
A Static Variable belongs to the class.
Only one copy is shared among all objects.

## Hindi
Static Variable class ka hota hai.
Iski sirf ek hi copy banti hai jo sabhi objects use karte hain.

---

### Example

```java
class Student {

    static String college = "IMS";

}
```

All students will share the same value.

### Memory Representation

```
Class Student

college = IMS

        ▲

 ┌──────┼──────┐

Object1 Object2 Object3
```

#  Real-Life Example

Imagine a school.
Every student has

- Name
- Roll Number

These are different for every student.
* Instance Variables

The school name is the same for everyone.
* Static Variable

A notebook used only during one class is like
* Local Variable

# Comparison Table

| Feature | Local | Instance | Static |
|----------|--------|----------|---------|
| Declared Inside | Method | Class | Class |
| Memory Created | Method Call | Object Creation | Class Loading |
| Shared |  No |  No |  Yes |
| Lifetime | Till Method Ends | Till Object Exists | Till Program Ends |


#  Scope of Variables
## Local Variable:
```
Method Starts
↓
Variable Created
↓
Method Ends
↓
Variable Destroyed
```

## Instance Variable
```
Object Created
↓
Variable Created
↓
Object Destroyed
↓
Variable Destroyed
```

## Static Variable
```
Program Starts
↓
Static Variable Created
↓
Program Ends
↓
Static Variable Destroyed
```

#  Complete Example

```java
class Student {

    static String college = "IMS";

    String name;

    public static void main(String[] args) {

        int age = 20;

        Student s1 = new Student();

        s1.name = "Sofiya";

        System.out.println(age);

        System.out.println(s1.name);

        System.out.println(college);

    }

}
```

# Output
```
20
Sofiya
IMS
```

# Important Notes
- Local Variables do not have default values.
- Instance Variables have default values.
- Static Variables are shared among all objects.
- Local Variables cannot be accessed outside their method.

#  Common Beginner Mistakes
* Using Local Variable outside the method.
* Forgetting to initialize a Local Variable.
* Thinking every object has a different Static Variable.
*  Declaring unnecessary Static Variables.

# Memory Trick
Remember:

### **L I S**
```
L → Local → Method
I → Instance → Object
S → Static → Shared
```

# Interview Questions (Part 2)

### Basic
1. What are the types of variables in Java?
2. What is a Local Variable?
3. What is an Instance Variable?
4. What is a Static Variable?
5. Which variable is shared among all objects?

### Intermediate
1. Differentiate Local, Instance and Static Variables.
2. Explain the lifetime of each variable.
3. Explain the scope of variables.
4. Which variable is stored inside an object?
5. Which variable belongs to a class?

# Summary (Part 2)
- Java has three types of variables.
- Local Variables exist only inside methods.
- Instance Variables belong to objects.
- Static Variables belong to the class.
- Static Variables are shared by all objects.
- Local Variables must be initialized before use.

# (Part-3)

#  Default Values of Variables

##  English
Default values are automatically assigned to **Instance Variables** and **Static Variables** if no value is provided.
Local Variables **do not** get default values.

## Hindi
Agar Instance Variable ya Static Variable ko koi value assign nahi ki jati, to Java automatically unhe default value de deta hai.
Lekin Local Variable ko koi default value nahi milti.

# Default Values Table

| Data Type | Default Value |
|------------|--------------|
| byte | 0 |
| short | 0 |
| int | 0 |
| long | 0L |
| float | 0.0f |
| double | 0.0 |
| char | '\u0000' |
| boolean | false |
| String / Objects | null |

#  Example

```java
class Student {

    int age;
    String name;
    boolean passed;

    public static void main(String[] args) {

        Student s = new Student();

        System.out.println(s.age);
        System.out.println(s.name);
        System.out.println(s.passed);

    }

}
```

# Output

```
0
null
false
```

---

#  Local Variable Example

```java
public class Demo {

    public static void main(String[] args) {

        int age;

        System.out.println(age);

    }

}
```

Output:

```
Compile Time Error
Variable age might not have been initialized.
```

# Important Definitions

## Variable
A Variable is a named memory location used to store data.

## Declaration
Creating a variable by specifying its data type and name.

Example:

```java
int age;
```

## Initialization
Assigning a value to a variable.

Example:

```java
age = 20;
```

## Scope
Scope defines where a variable can be accessed in a program.

## Lifetime
Lifetime is the duration for which a variable exists in memory.

#  Real-Life Example

Imagine a classroom.

- Student Name → Instance Variable
- School Name → Static Variable
- Marks of Today's Test → Local Variable

Today's test marks are useful only for today's class.
Similarly, a Local Variable exists only while its method is running.

# Viva Questions

### Basic Viva

**Q1. What is a Variable?**
**Answer:** A named memory location used to store data.

**Q2. How many types of variables are there in Java?**
**Answer:** Three
- Local
- Instance
- Static

**Q3. Which variable does not have a default value?**
**Answer:** Local Variable.

**Q4. Which variable belongs to an object?**
**Answer:** Instance Variable.

**Q5. Which variable is shared by all objects?**
**Answer:** Static Variable.

# Interview Questions

## Beginner Level
1. What is a Variable?
2. Explain Variable Declaration.
3. Explain Variable Initialization.
4. What is Variable Scope?
5. What is Variable Lifetime?
6. What are Local Variables?
7. What are Instance Variables?
8. What are Static Variables?
9. Which variables get default values?
10. Why must Local Variables be initialized?

## Intermediate Level
1. Differentiate Local, Instance and Static Variables.
2. Explain default values in Java.
3. Explain the memory representation of variables.
4. Explain the scope and lifetime of each variable.
5. Why are Static Variables shared?

#  MCQs

### Q1. Which variable belongs to an object?
- A. Local
- B. Instance.   (Correct)
- C. Static
- D. Final

### Q2. Which variable is shared among all objects?
- A. Local
- B. Instance
- C. Static.      (Correct)
- D. Method

### Q3. Which variable has no default value?
- A. Local.    (Correct)
- B. Instance
- C. Static
- D. Global
- 
### Q4. Which keyword is used to declare a Static Variable?
- A. public
- B. final
- C. static.     (Correct)
- D. private

### Q5. Which of the following is a valid declaration?
- A. int age;      (Correct)
- B. int 1age;
- C. int class;
- D. int student age;

### Q6. Java is ______.
- A. Case Ignored
- B. Case Sensitive.        (Correct)
- C. Machine Language
- D. Assembly Language

### Q7. Which variable exists only inside a method?
- A. Local Variable.       (Correct)
- B. Instance Variable
- C. Static Variable
- D. Global Variable

### Q8. Which variable is created when an object is created?
- A. Local
- B. Instance     (Correct)     
- C. Static
- D. Package

### Q9. Which variable is created when the class is loaded?
- A. Local
- B. Instance
- C. Static.       (Correct)
- D. Constructor

### Q10. Which statement is correct?
- A. Local Variables have default values.
-  B. Instance Variables have default values.      (Correct)
- C. Static Variables have no default values.
- D. Variables cannot store data.

# Practice Questions

### Short Questions
1. Define Variable.
2. What is Variable Declaration?
3. What is Variable Initialization?
4. Explain Local Variable.
5. Explain Instance Variable.
6. Explain Static Variable

### Long Questions
1. Explain all types of Variables with examples.
2. Differentiate Local, Instance and Static Variables.
3. Explain Variable Scope and Lifetime.
4. Write a Java program using all three types of Variables.
5. Explain default values of variables.

#  Common Errors & Solutions

| Error | Reason | Solution |
|--------|---------|----------|
| Using Local Variable without initialization | No default value | Initialize it before use |
| Variable name starts with a number | Invalid identifier | Start with a letter, `_` or `$` |
| Using Java keyword as variable name | Reserved keyword | Choose another name |
| Accessing Local Variable outside method | Scope issue | Use it only inside the method |

#  Exam Tips

* Learn all three types of Variables.

*Remember the difference between **Declaration** and **Initialization**.

*  Practice one program using Local, Instance and Static Variables.
* Learn the default values table for interviews and exams

#  Chapter Summary
- Variables store data in memory.
- Declaration creates a variable.
- Initialization assigns a value.
- Java has three types of variables.
- Local Variables do not have default values.
- Instance and Static Variables have default values.
- Static Variables are shared among all objects.
- Java is case-sensitive.

#  Chapter  Sheet

```
Variables
│

├── Local
│      │
│      └── Method
│
├── Instance
│      │
│      └── Object
│
└── Static
       │
       └── Class
```

### Memory Trick
Remember it as **LIS**.

```
L → Local → Method
I → Instance → Object
S → Static → Shared
```
------

- Chapter 04 Completed Successfully!

> **"Variables are the foundation of every Java program. Master them before moving ahead."**
>   .....Happy Learning.....
-------