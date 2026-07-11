# Chapter 07 - Operators (Part 1)

## Table of Contents

1. What is an Operator?
2. Why Do We Need Operators?
3. Types of Operators
4. Arithmetic Operators
5. Java Examples
6. Important Notes
7. Common Beginner Mistakes
8. Interview Questions
9. Summary

---

# What is an Operator?

## English
An Operator is a special symbol that performs an operation on one or more operands.
Operators are used to perform mathematical calculations, comparisons and logical operations.

## Hindi
Operator ek special symbol hota hai jo variables ya values par operation perform karta hai.
Java me Operators ka use calculation, comparison aur decision making ke liye kiya jata hai.

---

# What is an Operand?

## English
The values on which an operator performs an operation are called Operands.

Example

```java
int sum = 10 + 20;
```

Here,

10 and 20 are operands.

+ is the operator.

---

## Hindi
Jin values ya variables par Operator kaam karta hai unhe Operands kehte hain.
Example

```java
int sum = 10 + 20;
```

Yahan,
10 aur 20 operands hain.
Aur (+) operator hai.

---

# Why Do We Need Operators?

## English
Operators help us to
- Perform calculations.
- Compare values.
- Make decisions.
- Increase or decrease values.
- Combine conditions.

---

## Hindi
Operators ka use kiya jata hai
- Calculation karne ke liye.
- Values compare karne ke liye.
- Decision lene ke liye.
- Value ko increase ya decrease karne ke liye.
- Multiple conditions check karne ke liye.

---

# Types of Operators

Java provides different types of Operators.

```
Operators

|

|-- Arithmetic Operators

|-- Relational Operators

|-- Logical Operators

|-- Assignment Operators

|-- Unary Operators

|-- Ternary Operator

|-- Bitwise Operators

|-- Shift Operators
```

In this chapter, we will first study Arithmetic Operators.

---

# Arithmetic Operators

Arithmetic Operators are used to perform mathematical calculations.
(Arithmetic Operators ka use mathematical calculations karne ke liye kiya jata hai.)

---

# Types of Arithmetic Operators

| Operator | Name | Example |
|----------|------|----------|
| + | Addition | a + b |
| - | Subtraction | a - b |
| * | Multiplication | a * b |
| / | Division | a / b |
| % | Modulus | a % b |

---

# Addition Operator (+)

The Addition Operator is used to add two numbers.
(Addition Operator ka use do numbers ko jodne ke liye kiya jata hai.)

---

Example

```java
int a = 10;
int b = 20;

System.out.println(a + b);
```

Output

```
30
```

---

# Subtraction Operator (-)

The Subtraction Operator subtracts one number from another.
(Subtraction Operator ek number me se dusre number ko ghatata hai.)

---

Example

```java
int a = 30;
int b = 10;

System.out.println(a - b);
```

Output

```
20
```

---

# Multiplication Operator (*)

The Multiplication Operator multiplies two numbers.
(Multiplication Operator do numbers ka multiplication karta hai.)

---

Example

```java
int a = 5;
int b = 4;

System.out.println(a * b);
```

Output

```
20
```

---

# Division Operator (/)

The Division Operator divides one number by another.
(Division Operator ek number ko dusre number se divide karta hai.)

---

Example

```java
int a = 20;
int b = 5;

System.out.println(a / b);
```

Output

```
4
```

---

# Modulus Operator (%)

The Modulus Operator returns the remainder after division.
(Modulus Operator division ke baad bachne wala remainder return karta hai.)

---

Example

```java
int a = 17;
int b = 5;

System.out.println(a % b);
```

Output

```
2
```

---

# Important Notes
- (+) is used for Addition.
- (-) is used for Subtraction.
- (*) is used for Multiplication.
- (/) is used for Division.
- (%) returns the remainder.

---

# Common Beginner Mistakes

Wrong

```java
System.out.println(10 / 3);
```

Expected Output

```
3.33
```

Actual Output

```
3
```

Reason

Both values are integers.

---

Correct

```java
System.out.println(10.0 / 3);
```

Output

```
3.3333333333333335
```

---

# Interview Questions

## Basic
1. What is an Operator?
2. What is an Operand?
3. How many Arithmetic Operators are there?
4. What is the difference between Division and Modulus?
5. Which operator returns the remainder?

---

## Intermediate
1. Explain Arithmetic Operators with examples.
2. Why does integer division remove the decimal part?
3. Explain the Modulus Operator.
4. What is the difference between '/' and '%'?
5. Give real-life examples of Arithmetic Operators.

---

# Summary
- Operators perform operations on operands.
- Arithmetic Operators perform mathematical calculations.
- Java provides five Arithmetic Operators.
- Modulus returns the remainder.
- Integer division removes the decimal part.

---

# (Part-2)

In Part 2, we will study:
- Assignment Operators
- Relational Operators
- Logical Operators
- Java Programs
- Practice Questions
- Interview Questions

# Assignment Operators

Assignment Operators are used to assign values to variables.
The most commonly used Assignment Operator is (=).

(Assignment Operators ka use variables ko value assign karne ke liye kiya jata hai.
Sabse common Assignment Operator (=) hota hai.)

---

# Types of Assignment Operators

| Operator | Meaning | Example |
|----------|---------|----------|
| = | Assign | a = 10 |
| += | Add and Assign | a += 5 |
| -= | Subtract and Assign | a -= 5 |
| *= | Multiply and Assign | a *= 5 |
| /= | Divide and Assign | a /= 5 |
| %= | Modulus and Assign | a %= 5 |

---

# Assignment Operator (=)

The Assignment Operator assigns a value to a variable.
(Assignment Operator variable ko value assign karta hai.)

Example

```java
int age = 20;

System.out.println(age);
```

Output

```
20
```

---

# Addition Assignment (+=)

It adds the value and stores the result in the same variable.
(Ye variable me value add karke usi variable me store kar deta hai.)

Example

```java
int a = 10;

a += 5;

System.out.println(a);
```

Output

```
15
```

Equivalent To

```java
a = a + 5;
```

---

# Subtraction Assignment (-=)

It subtracts the value and stores the result.
(Ye value ko subtract karke result ko usi variable me store karta hai.)

Example

```java
int a = 20;

a -= 8;

System.out.println(a);
```

Output

```
12
```

Equivalent To

```java
a = a - 8;
```

---

# Multiplication Assignment (*=)

It multiplies the value and stores the result.
(Ye variable ki value ko multiply karke usi variable me store karta hai.)

Example

```java
int a = 5;

a *= 4;

System.out.println(a);
```

Output

```
20
```

Equivalent To

```java
a = a * 4;
```

---

# Division Assignment (/=)

It divides the value and stores the result.
(Ye value ko divide karke result ko usi variable me store karta hai.)

Example

```java
int a = 20;

a /= 5;

System.out.println(a);
```

Output

```
4
```

Equivalent To

```java
a = a / 5;
```

---

# Modulus Assignment (%=)

It stores the remainder in the same variable.
(Ye division ke baad remainder ko usi variable me store karta hai.)

Example

```java
int a = 17;

a %= 5;

System.out.println(a);
```

Output

```
2
```

Equivalent To

```java
a = a % 5;
```

---

# Relational Operators

Relational Operators compare two values.
The result is always either **true** or **false**.

(Relational Operators do values ko compare karte hain.
Inka result hamesha **true** ya **false** hota hai.)

---

# Types of Relational Operators

| Operator | Meaning | Example |
|----------|---------|----------|
| == | Equal To | a == b |
| != | Not Equal To | a != b |
| > | Greater Than | a > b |
| < | Less Than | a < b |
| >= | Greater Than or Equal To | a >= b |
| <= | Less Than or Equal To | a <= b |

---

# Example

```java
int a = 10;
int b = 20;

System.out.println(a == b);
System.out.println(a != b);
System.out.println(a > b);
System.out.println(a < b);
System.out.println(a >= b);
System.out.println(a <= b);
```

Output

```
false
true
false
true
false
true
```

---

# Important Notes
- Assignment Operator assigns values.
- Relational Operators compare values.
- Relational Operators always return boolean values.
- They are mostly used with if-else and loops.

---

# Common Beginner Mistakes
Wrong

```java
if(a = b)
```

Correct

```java
if(a == b)
```

Reason

`=` assigns a value.

`==` compares two values.

---

# Interview Questions

## Basic
1. What is an Assignment Operator?
2. What is the difference between = and ==?
3. What is the purpose of Relational Operators?
4. Which operators return true or false?
5. Name all Relational Operators.

---

## Intermediate
1. Explain Assignment Operators with examples.
2. Explain Relational Operators with examples.
3. Why is == used instead of = in conditions?
4. Where are Relational Operators commonly used?
5. Differentiate Assignment and Relational Operators.

---

# Summary
- Assignment Operators assign values.
- Relational Operators compare values.
- Relational Operators always return true or false.
- = assigns a value, while == compares two values.

---

#  (Part-3)

In Part 3, we will study:
- Logical Operators
- Unary Operators
- Ternary Operator
- Bitwise Operators
- Practice Programs
- MCQs
- Viva Questions
- Interview Questions
- Chapter Summary

# Logical Operators

Logical Operators are used to combine two or more conditions.
The result of a Logical Operator is always either **true** or **false**.

(Logical Operators ka use do ya do se adhik conditions ko combine karne ke liye kiya jata hai.
Inka result hamesha **true** ya **false** hota hai.)

---

# Types of Logical Operators

| Operator | Name | Meaning |
|----------|------|---------|
| && | Logical AND | Returns true if both conditions are true |
| \|\| | Logical OR | Returns true if at least one condition is true |
| ! | Logical NOT | Reverses the result |

---

# Logical AND (&&)

The AND Operator returns **true** only when both conditions are true.
(AND Operator tabhi **true** return karta hai jab dono conditions true ho.)

---

Example

```java
int age = 20;

System.out.println(age >= 18 && age <= 25);
```

Output

```
true
```

---

# Logical OR (||)

The OR Operator returns **true** if at least one condition is true.
(OR Operator **true** return karta hai agar koi bhi ek condition true ho.)

---

Example

```java
int age = 16;

System.out.println(age < 18 || age > 60);
```

Output

```
true
```

---

# Logical NOT (!)

The NOT Operator reverses the result.
True becomes False.
False becomes True.

(NOT Operator result ko ulta kar deta hai.
True ko False aur False ko True bana deta hai.)

---

Example

```java
boolean result = true;

System.out.println(!result);
```

Output

```
false
```

---

# Unary Operators

Unary Operators perform an operation on only one operand.
(Unary Operators sirf ek operand par operation perform karte hain.)

---

# Types of Unary Operators

| Operator | Meaning |
|----------|---------|
| + | Unary Plus |
| - | Unary Minus |
| ++ | Increment |
| -- | Decrement |
| ! | Logical NOT |

---

# Increment Operator (++)

The Increment Operator increases the value by 1.
(Increment Operator value ko 1 se badha deta hai.)

---

Example

```java
int a = 10;

a++;

System.out.println(a);
```

Output

```
11
```

---

# Decrement Operator (--)

The Decrement Operator decreases the value by 1.
(Decrement Operator value ko 1 se kam kar deta hai.)

---

Example

```java
int a = 10;

a--;

System.out.println(a);
```

Output

```
9
```

---

# Ternary Operator

## English
The Ternary Operator is a shortcut for the if-else statement.
Syntax

```java
condition ? expression1 : expression2;
```


## Hindi
Ternary Operator if-else ka short form hai.
Syntax

```java
condition ? expression1 : expression2;
```

---

Example

```java
int age = 20;

String result = (age >= 18) ? "Eligible" : "Not Eligible";

System.out.println(result);
```

Output

```
Eligible
```

---

# Bitwise Operators

## English
Bitwise Operators perform operations on binary bits.
They are mainly used in low-level programming.

## Hindi
Bitwise Operators binary bits par operation perform karte hain.
Inka use mainly low-level programming me hota hai.

---

# Types of Bitwise Operators

| Operator | Meaning |
|----------|---------|
| & | Bitwise AND |
| \| | Bitwise OR |
| ^ | Bitwise XOR |
| ~ | Bitwise Complement |

---

# Important Notes
- Logical Operators work with boolean values.
- Unary Operators work on a single operand.
- Ternary Operator is a short form of if-else.
- Bitwise Operators work on binary values.

---

# Common Beginner Mistakes

Wrong

```java
if(age > 18 & age < 30)
```

Correct

```java
if(age > 18 && age < 30)
```

Reason

`&&` is a Logical AND operator.

`&` is a Bitwise AND operator.

---

Wrong

```java
a = a++;
```

Explanation
This does not increase the value as many beginners expect.
Correct

```java
a++;
```

or

```java
++a;
```

---

# MCQs

### 1. Which operator is used for Logical AND?
A. &
B. &&
C. ||
D. !
Answer
```
B
```

---

### 2. Which operator is known as the Conditional Operator?
A. +
B. %
C. ? :
D. ==
Answer
```
C
```

---

### 3. Which operator increases the value by one?
A. --
B. ++
C. +
D. +=
Answer
```
B
```

---

### 4. Which operator reverses a boolean value?
A. !
B. ++
C. ||
D. ==
Answer
```
A
```

---

### 5. Which operator works on binary bits?
A. %
B. +
C. Bitwise Operators
D. /
Answer
```
C
```

---

# Viva Questions
1. What is a Logical Operator?
2. What is the difference between && and ||?
3. What is the NOT Operator?
4. What is a Unary Operator?
5. Explain Increment and Decrement Operators.
6. What is a Ternary Operator?
7. Why is the Ternary Operator used?
8. What are Bitwise Operators?
9. Where are Bitwise Operators used?
10. Which operator is used as a shortcut for if-else?

---

# Interview Questions

## Basic
1. What are Logical Operators?
2. Explain AND, OR and NOT with examples.
3. What are Unary Operators?
4. Explain the Increment Operator.
5. What is the Ternary Operator?

---

## Intermediate
1. Differentiate Logical AND and Bitwise AND.
2. Explain Prefix and Postfix Increment.
3. Explain Bitwise Operators.
4. Why is the Ternary Operator faster than if-else in simple conditions?
5. Give real-life examples of Logical Operators.

---

# Quick Revision
- Arithmetic Operators → Perform calculations.
- Assignment Operators → Assign values.
- Relational Operators → Compare values.
- Logical Operators → Combine conditions.
- Unary Operators → Work on one operand.
- Ternary Operator → Short form of if-else.
- Bitwise Operators → Work on binary bits.

---

# Chapter Summary
In this chapter, we learned:
- Arithmetic Operators
- Assignment Operators
- Relational Operators
- Logical Operators
- Unary Operators
- Ternary Operator
- Bitwise Operators
- Java Examples
- MCQs
- Viva Questions
- Interview Questions

Operators are one of the most important concepts in Java because they are used in almost every program, including conditions, loops, methods, and object-oriented programming.

---