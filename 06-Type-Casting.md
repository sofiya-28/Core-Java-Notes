# Chapter 06 - Type Casting (Part 1)

# What is Type Casting?

## English
Type Casting is the process of converting one data type into another data type.
In Java, sometimes we need to convert a value from one data type to another. This conversion is called Type Casting.

---

## Hindi
Type Casting ka matlab hai ek data type ko doosre data type me convert karna.
Jab hume kisi value ko ek data type se doosre data type me badalna hota hai, tab hum Type Casting ka use karte hain.

---

# Why Do We Need Type Casting?

## English
Type Casting is required when:

- Converting one data type into another.
- Performing mathematical calculations.
- Passing values to methods.
- Saving memory.
- Avoiding compilation errors.

---

## Hindi
Type Casting ki zarurat tab padti hai jab:

- Ek data type ko dusre data type me convert karna ho.
- Mathematical calculations karni ho.
- Kisi method me different data type ki value pass karni ho.
- Memory ko efficiently use karna ho.
- Compilation errors se bachna ho.

---

# Real-Life Example

Imagine two water bottles.
Bottle 1 Capacity = 500 ml
Bottle 2 Capacity = 2 Litres
You can easily pour water from the small bottle into the large bottle.
But if you pour water from the large bottle into the small bottle, some water may overflow.
Java follows the same concept while converting one data type into another.

---

# Types of Type Casting

Java supports two types of Type Casting.

```
              Type Casting

                   |

        ----------------------

        |                    |

    Widening            Narrowing

    (Implicit)          (Explicit)
```

---

# Widening Type Casting (Implicit)

## English
Widening Type Casting means converting a smaller data type into a larger data type.
Java performs this conversion automatically.
No casting operator is required.

---

## Hindi
Widening Type Casting me chhote data type ko bade data type me convert kiya jata hai.
Ye conversion Java automatically kar deta hai.
Isme casting operator lagane ki zarurat nahi hoti.

---

# Conversion Order

```
byte
↓
short
↓
int
↓
long
↓
float
↓
double
```

---

# Example 1

```java
int number = 100;

double value = number;

System.out.println(value);
```

Output

```
100.0
```

Explanation
Java automatically converts the integer value into a double value.
No data is lost.

---

# Example 2

```java
byte age = 20;
int value = age;

System.out.println(value);
```

Output

```
20
```

Explanation
Java automatically converts byte into int.

---

# Example 3

```java
char ch = 'A';

int ascii = ch;

System.out.println(ascii);
```

Output

```
65
```

Explanation

Java converts the character into its Unicode value automatically.

---

# Memory Representation

```
int number = 100
↓
double value = 100.0
```

Memory size increases but the original value remains unchanged.

---

# Advantages of Widening
- Automatic conversion.
- No data loss.
- Safe conversion.
- No casting operator required.
- Easy to understand and use.

---

# Important Notes
- Widening is also known as Implicit Type Casting.
- Java performs widening automatically.
- Data loss does not occur during widening.
- Smaller data types are converted into larger data types.

---

# Common Beginner Mistakes

Wrong

```java
double value = (double)10;
```

Correct

```java
double value = 10;
```

Reason

Casting is not required because Java performs widening automatically.

---

Wrong

```java
int number = 15.5;
```

Correct

```java
int number = (int)15.5;
```

Reason

A decimal value cannot be stored directly in an int variable.

---

# Interview Questions

## Basic
1. What is Type Casting?
2. Why do we use Type Casting?
3. How many types of Type Casting are there?
4. What is Widening Type Casting?
5. Is Widening automatic?

---

## Intermediate
1. Explain Widening Type Casting with an example.
2. Why is Widening called Implicit Type Casting?
3. Is data lost during Widening?
4. Explain the conversion order of Widening.
5. Give three real-life examples of Widening.

---

# Summary
- Type Casting means converting one data type into another.
- Java supports Widening and Narrowing Type Casting.
- Widening converts a smaller data type into a larger data type.
- Widening is automatic.
- No data loss occurs during Widening.

---

#  (Part-2)
# Narrowing Type Casting (Explicit)

## English
Narrowing Type Casting means converting a larger data type into a smaller data type.
Java does not perform this conversion automatically.
We must use the casting operator.
Since a larger data type is converted into a smaller one, data loss may occur.

---

## Hindi
Narrowing Type Casting ka matlab hai bade data type ko chhote data type me convert karna.
Java is conversion ko automatically nahi karta.
Iske liye hume casting operator `( )` ka use karna padta hai.
Kyuki bada data type chhote data type me convert hota hai, isliye data loss ho sakta hai.

---

# Syntax

```java
dataType variable = (dataType) value;
```

Example

```java
int number = (int) 15.8;
```

---

# Conversion Order

```
double
↓
float
↓
long
↓
int
↓
short
↓
byte
```

---

# Example 1

```java
double number = 25.89;

int value = (int) number;

System.out.println(value);
```

Output

```
25
```

Explanation

The decimal part (.89) is removed.

Only the integer part is stored.

---

# Example 2

```java
double marks = 89.75;

float result = (float) marks;

System.out.println(result);
```

Output

```
89.75
```

Explanation
Java converts double into float using the casting operator.
Some precision may be lost because float stores fewer decimal digits than double.

---

# Example 3

```java
int number = 130;

byte value = (byte) number;

System.out.println(value);
```

Output

```
-126
```

Explanation

The value changes because the range of byte is

```
-128 to 127
```

Since 130 is outside the byte range, the stored value becomes **-126**.

This is called **Overflow**.

---

# Data Loss

## English
During Narrowing Type Casting, some information may be lost.
For example, decimal values are removed when converting double into int.

---

## Hindi
Narrowing Type Casting me data ka kuch hissa lose ho sakta hai.
Jaise double ko int me convert karne par decimal part remove ho jata hai.

---

# Example

```java
double price = 99.99;

int value = (int) price;

System.out.println(value);
```

Output

```
99
```

The decimal value **.99** is removed.

---

# Overflow
Overflow occurs when a value is larger than the storage capacity of a data type.

Example

```java
int number = 140;

byte value = (byte) number;

System.out.println(value);
```

Output

```
-116
```

Since byte cannot store 140, the value changes after conversion.

---

# Memory Representation

```
double number = 45.99
↓
(int)
↓
45
```

The decimal part is removed after casting.

---

# Difference Between Widening and Narrowing

| Widening | Narrowing |
|-----------|------------|
| Small Data Type → Large Data Type | Large Data Type → Small Data Type |
| Automatic | Manual |
| Safe | Risky |
| No Data Loss | Data Loss Possible |
| Casting Operator Not Required | Casting Operator Required |

---

# Advantages of Narrowing
- Reduces memory usage.
- Useful when only smaller values are needed.
- Helps in specific programming situations.

---

# Disadvantages of Narrowing
- Data loss may occur.
- Precision may decrease.
- Overflow may happen.
- Manual casting is required.

---

# Important Notes
- Narrowing is also called Explicit Type Casting.
- Java never performs Narrowing automatically.
- The casting operator is mandatory.
- Data loss is possible.
- Overflow can occur if the value exceeds the range of the target data type.

---

# Common Beginner Mistakes

Wrong

```java
double number = 45.8;

int value = number;
```

Compilation Error

---

Correct

```java
double number = 45.8;

int value = (int) number;
```

---

Wrong

```java
float value = 12.5;
```

Correct

```java
float value = 12.5f;
```

---

# Interview Questions

## Basic
1. What is Narrowing Type Casting?
2. Why is Narrowing called Explicit Type Casting?
3. Is Narrowing automatic?
4. Why do we use the casting operator?
5. Can data loss occur during Narrowing?

---

## Intermediate
1. Explain Narrowing with an example.
2. What is Overflow?
3. Why is Narrowing considered risky?
4. Differentiate Widening and Narrowing.
5. What happens when a double is converted into an int?

---

# Summary
- Narrowing converts a larger data type into a smaller data type.
- It requires the casting operator.
- Data loss may occur.
- Overflow is possible.
- Narrowing should be used carefully.

---

# (Part-3)
# Complete Java Program

```java
public class TypeCastingDemo {

    public static void main(String[] args) {

        // Widening Type Casting
        int number = 100;
        double value = number;

        System.out.println("Widening Type Casting");
        System.out.println("int Value : " + number);
        System.out.println("double Value : " + value);

        System.out.println();

        // Narrowing Type Casting
        double price = 99.99;
        int result = (int) price;

        System.out.println("Narrowing Type Casting");
        System.out.println("double Value : " + price);
        System.out.println("int Value : " + result);

    }

}
```

---

# Output

```
Widening Type Casting
int Value : 100
double Value : 100.0

Narrowing Type Casting
double Value : 99.99
int Value : 99
```

---

# Real-Life Examples

## Example 1
Suppose a student's marks are stored as an integer.

```java
int marks = 95;

double percentage = marks;
```

Java automatically converts the integer into a decimal number.
This is Widening Type Casting.

---

## Example 2
Suppose an online shopping application calculates the total price.

```java
double totalPrice = 499.99;

int roundedPrice = (int) totalPrice;
```

Output

```
499
```

The decimal value is removed.

This is Narrowing Type Casting.

---

# Practice Programs

## Program 1

Convert int into double.

```java
int number = 50;

double value = number;

System.out.println(value);
```

---

## Program 2

Convert double into int.

```java
double number = 45.67;

int value = (int) number;

System.out.println(value);
```

---

## Program 3

Convert char into int.

```java
char ch = 'A';

int ascii = ch;

System.out.println(ascii);
```

---

## Program 4

Convert long into int.

```java
long population = 1400000000L;

int value = (int) population;

System.out.println(value);
```

---

## Program 5

Convert float into int.

```java
float price = 19.95f;

int value = (int) price;

System.out.println(value);
```

---

# MCQs

### 1. Type Casting means
A. Creating Variables
B. Converting one data type into another
C. Printing Output
D. Creating Objects
Answer
```
B
```

---

### 2. Which Type Casting is automatic?
A. Narrowing
B. Explicit
C. Widening
D. Manual
Answer
```
C
```

---

### 3. Which operator is used in Explicit Type Casting?
A. {}
B. []
C. ()
D. <>
Answer
```
C
```

---

### 4. Which Type Casting may cause data loss?
A. Widening
B. Narrowing
C. Implicit
D. Automatic
Answer
```
B
```

---

### 5. What is the output?

```java
double num = 20.9;

int value = (int) num;

System.out.println(value);
```

A. 20.9

B. 21

C. 20

D. Compilation Error

Answer

```
C
```

---

# Viva Questions
1. What is Type Casting?
2. Why do we use Type Casting?
3. What are the two types of Type Casting?
4. What is Widening Type Casting?
5. What is Narrowing Type Casting?
6. Why is Narrowing called Explicit Type Casting?
7. What is Overflow?
8. What is Data Loss?
9. Which Type Casting is safer?
10. Why does Widening not cause data loss?

---

# Interview Questions

## Basic
1. Define Type Casting.
2. What is Widening Type Casting?
3. What is Narrowing Type Casting?
4. Why do we use the casting operator?
5. Is Widening automatic?

---

## Intermediate
1. Explain Widening with an example.
2. Explain Narrowing with an example.
3. What is Overflow in Java?
4. Why can Narrowing cause data loss?
5. Differentiate Widening and Narrowing.

---

# Common Beginner Mistakes
Using Narrowing without the casting operator.

Wrong

```java
double number = 25.5;

int value = number;
```

Correct

```java
double number = 25.5;

int value = (int) number;
```

---

Thinking that Widening requires casting.

Wrong

```java
double value = (double)10;
```

Correct

```java
double value = 10;
```

---

Using float without the suffix 'f'.

Wrong

```java
float price = 15.5;
```

Correct

```java
float price = 15.5f;
```

---

# Quick Revision
- Type Casting converts one data type into another.
- Java supports Widening and Narrowing Type Casting.
- Widening is automatic.
- Narrowing requires the casting operator.
- Widening does not cause data loss.
- Narrowing may cause data loss.
- Overflow occurs when the value exceeds the range of the target data type.

---

# Chapter Summary
In this chapter, we learned:

- What is Type Casting?
- Why Type Casting is required.
- Widening Type Casting.
- Narrowing Type Casting.
- Casting Operator.
- Data Loss.
- Overflow.
- Java Programs.
- Practice Programs.
- MCQs.
- Viva Questions.
- Interview Questions.

Type Casting is an important Java concept that helps programmers convert values between different data types safely and efficiently.

---
