# Chapter 05 - Data Types (Part 1)

## What is a Data Type?

A **Data Type** defines the type of data that a variable can store.

It tells the Java compiler:
- What type of value will be stored.
- How much memory should be allocated.
- What operations can be performed on that value.
In simple words,

> A Data Type tells Java what kind of information a variable contains.

## Why Do We Need Data Types?
Imagine you have different containers.
-  Milk Bottle → Stores Milk
-  Water Bottle → Stores Water
-  Book Shelf → Stores Books

Each container is designed for a specific purpose.
Similarly,
Every variable in Java stores a specific type of data.

Without Data Types,
- Java cannot reserve memory.
- Java cannot perform calculations correctly.
- Java cannot understand what kind of value is stored.

## Example

```java
int age = 20;
double salary = 55000.75;
char grade = 'A';
boolean passed = true;
```

Here,
- age stores an integer.
- salary stores a decimal value.
- grade stores one character.
- passed stores true or false.

## Memory Representation

```
Computer Memory

+---------------------+
| age = 20            |
+---------------------+

+---------------------+
| salary = 55000.75   |
+---------------------+

+---------------------+
| grade = 'A'         |
+---------------------+

+---------------------+
| passed = true       |
+---------------------+
```
Every variable occupies memory according to its Data Type.

# Types of Data Types

Java has two types of Data Types.

```
               Data Types
                    |
        -------------------------
        |                       |
 Primitive Data Types    Non-Primitive Data Types
```

# 1. Primitive Data Types

Primitive Data Types are predefined by Java.
These Data Types store values directly.
Java has **8 Primitive Data Types.**

| Data Type | Description |
|-----------|-------------|
| byte | Small Integer |
| short | Short Integer |
| int | Integer |
| long | Large Integer |
| float | Decimal Number |
| double | Large Decimal Number |
| char | Single Character |
| boolean | True or False |


## Features of Primitive Data Types

- Built into Java.
- Store actual values.
- Faster than Non-Primitive Data Types.
- Fixed memory size.
- Cannot call methods.

Example

```java
int marks = 95;
char grade = 'A';
boolean pass = true;
```

# 2. Non-Primitive Data Types

Non-Primitive Data Types are also called **Reference Data Types.**
They do not store actual data directly.
Instead,
they store the reference (address) of an object.
Examples:

- String
- Array
- Class
- Object
- Interface

Example

```java
String name = "Sofiya";
```

Here,

"name" stores the reference of the String object.

## Features of Non-Primitive Data Types

- Created by programmers or Java.
- Store object references.
- Size is not fixed.
- Can call methods.
- More powerful than Primitive Data Types.

Example

```java
String city = "Ghaziabad";

System.out.println(city.length());
```

# Primitive vs Non-Primitive

| Primitive | Non-Primitive |
|------------|---------------|
| Stores actual value | Stores object reference |
| Fixed size | Variable size |
| Faster | Slightly slower |
| Built into Java | Created using Classes |
| Cannot call methods | Can call methods |


# Real-Life Example

Imagine a school.
Primitive Data Types are like simple boxes.

```
Roll Number
Age
Marks
Grade
```

Non-Primitive Data Types are like complete files.

```
Student Record
↓
Name
Address
Phone
Subjects
Attendance
```

Primitive stores one simple value.
Non-Primitive stores a complete object.

#  Important Points
- Every variable must have a Data Type.
- Java is a Strongly Typed Language.
- Primitive Data Types store values directly.
- Non-Primitive Data Types store object references.
- Java provides 8 Primitive Data Types.

# Common Beginner Mistakes
*  Thinking String is a Primitive Data Type.

* Writing

```java
Int age = 20;
```

Correct

```java
int age = 20;
```

Java is case-sensitive.


* Using double values inside int.

Wrong

```java
int price = 12.5;
```

Correct

```java
double price = 12.5;
```

# Interview Questions

### Basic
1. What is a Data Type?
2. Why do we need Data Types?
3. How many types of Data Types are there?
4. What is the difference between Primitive and Non-Primitive Data Types?
5. Is String a Primitive Data Type?

### Intermediate
1. Why is Java called a Strongly Typed Language?
2. Explain Primitive Data Types with examples.
3. Explain Reference Data Types.
4. Why are Non-Primitive Data Types called Reference Types?
5. Which Data Type is more memory efficient?

# Summary
- Data Type defines the type of value a variable can store.
- Java has two categories of Data Types.
- Primitive Data Types store actual values.
- Non-Primitive Data Types store object references.
- Choosing the correct Data Type improves memory usage and program performance.

# (Part-3)

# Primitive Data Types in Detail

Java provides **8 Primitive Data Types**.

They are:

1. byte
2. short
3. int
4. long
5. float
6. double
7. char
8. boolean

---

# 1. byte

The **byte** data type is used to store small integer values.

### Size

```
1 Byte (8 Bits)
```

### Range

```
-128 to 127
```

### Default Value

```
0
```

### Example

```java
public class ByteExample {

    public static void main(String[] args) {

        byte age = 20;

        System.out.println(age);

    }

}
```

### Memory Diagram

```
byte age = 20

+--------+
|   20   |
+--------+
```

### Uses

- Saving memory
- File handling
- Network programming

---

# 2. short

The **short** data type stores integer values larger than byte.

### Size

```
2 Bytes (16 Bits)
```

### Range

```
-32,768 to 32,767
```

### Default Value

```
0
```

### Example

```java
short salary = 25000;

System.out.println(salary);
```

### Memory Diagram

```
short salary

+------------+
|   25000    |
+------------+
```

### Uses

- Medium-sized numbers
- Memory optimization

---

# 3. int

The **int** data type is the most commonly used integer type in Java.

Whenever we store whole numbers,

we generally use **int**.

### Size

```
4 Bytes (32 Bits)
```

### Range

```
-2,147,483,648

to

2,147,483,647
```

### Default Value

```
0
```

### Example

```java
int marks = 95;

System.out.println(marks);
```

### Memory Diagram

```
int marks

+------------+
|     95     |
+------------+
```

### Uses

- Roll Number
- Age
- Marks
- Employee ID
- Product Quantity

---

# 4. long

The **long** data type stores very large integer values.

When int is not enough,

we use long.

### Size

```
8 Bytes (64 Bits)
```

### Default Value

```
0L
```

### Example

```java
long population = 1400000000L;

System.out.println(population);
```

**Note**

Always write **L** or **l** after long values.

Preferred

```java
long number = 9876543210L;
```

---

### Memory Diagram

```
long population

+--------------------+
|   1400000000L      |
+--------------------+
```

### Uses

- Population
- Bank Transactions
- Large IDs

---

# Integer Data Types Comparison

| Data Type | Size | Range |
|-----------|------|----------------|
| byte | 1 Byte | -128 to 127 |
| short | 2 Bytes | -32,768 to 32,767 |
| int | 4 Bytes | -2,147,483,648 to 2,147,483,647 |
| long | 8 Bytes | Very Large Integer |

---

# Important Notes

- byte uses the least memory.
- int is the most commonly used integer data type.
- long is used for very large values.
- Use long only when int cannot store the value.

---

# Common Beginner Mistakes

❌ Forgetting **L** after long value.

Wrong

```java
long number = 9876543210;
```

Correct

```java
long number = 9876543210L;
```

---

❌ Using byte for very large numbers.

Wrong

```java
byte age = 200;
```

Correct

```java
int age = 200;
```

---

# Interview Questions

### Basic

1. Which integer Data Type is used most frequently?
2. What is the size of byte?
3. What is the size of int?
4. Why do we use long?
5. What is the range of byte?

---

### Intermediate

1. Differentiate byte and short.
2. Differentiate int and long.
3. Why do we write L after long values?
4. Which integer Data Type is memory efficient?
5. When should we use long instead of int?

---

# Summary

- byte → Small Integer
- short → Medium Integer
- int → Most Common Integer Type
- long → Large Integer Values

Choose the smallest suitable Data Type to improve memory efficiency.

---

## Next Part

In **Part 3**, we will study:

- float
- double
- char
- boolean
- Default Values
- Primitive Data Types Table
- Java Programs
- MCQs
- Viva Questions
- Interview Questions
- Chapter Summary

# (Part-3)
