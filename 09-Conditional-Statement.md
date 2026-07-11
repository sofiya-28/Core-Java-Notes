# Chapter 09 - Conditional Statements (Part 1)

## Table of Contents

1. What are Conditional Statements?
2. Why Do We Need Conditional Statements?
3. Types of Conditional Statements
4. if Statement
5. Flowchart
6. Java Examples
7. Real-Life Examples
8. Important Notes
9. Common Beginner Mistakes
10. Interview Questions
11. Summary

---

# What are Conditional Statements?

## English
Conditional Statements are used to make decisions in a program.
They allow the program to execute different blocks of code depending on whether a condition is true or false.

## Hindi
Conditional Statements ka use program me decision lene ke liye kiya jata hai.
Ye condition ke true ya false hone ke according different code execute karte hain.

---

# Why Do We Need Conditional Statements?

## English
Without Conditional Statements, every statement would execute one after another.
Conditional Statements allow us to execute only the required code.

## Hindi
Agar Conditional Statements na ho, to program ki har statement execute hogi.
Conditional Statements sirf wahi code chalate hain jo condition ke hisaab se zaroori hota hai.

---

# Types of Conditional Statements

Java provides the following Conditional Statements:

```
Conditional Statements

|

|-- if

|-- if-else

|-- else-if Ladder

|-- Nested if

|-- switch
```

---

# if Statement

## English
The `if` statement executes a block of code only when the condition is true.
If the condition is false, the block is skipped.

## Hindi
`if` statement tabhi execute hoti hai jab condition true ho.
Agar condition false ho, to uske andar ka code execute nahi hota.

---

# Syntax

```java
if (condition) {

    // Code to execute

}
```

---

# Flowchart

```
          Condition

             |

        +----+----+

        |         |

      True      False

        |         |

 Execute Code   Skip Code
```

---

# Example 1

```java
public class Demo {

    public static void main(String[] args) {

        int age = 20;

        if (age >= 18) {

            System.out.println("You are eligible to vote.");

        }

    }

}
```

Output

```
You are eligible to vote.
```

---

# Example 2

```java
public class Demo {

    public static void main(String[] args) {

        int marks = 85;

        if (marks >= 33) {

            System.out.println("Pass");

        }

    }

}
```

Output

```
Pass
```

---

# Example 3

```java
public class Demo {

    public static void main(String[] args) {

        int temperature = 40;

        if (temperature > 35) {

            System.out.println("It is a hot day.");

        }

    }

}
```

Output

```
It is a hot day.
```

---

# Real-Life Examples

## Voting Eligibility

```java
if (age >= 18)
```

The person is eligible to vote.

---

## ATM

```java
if (balance >= amount)
```
Money can be withdrawn.

---

## Exam Result
```java
if (marks >= 33)
```

Student is Pass.

---

# Important Notes
- `if` executes only when the condition is true.
- The condition must return `true` or `false`.
- Curly braces `{}` are recommended even for a single statement.
- `if` does nothing when the condition is false.

---

# Common Beginner Mistakes

Wrong
```java
if(age = 18)
```

Correct
```java
if(age == 18)
```

Reason
`=` assigns a value.

`==` compares values.

---

Wrong
```java
if(10)
```

Correct
```java
if(age > 10)
```

Reason
Java requires a boolean condition.

---

# Interview Questions

## Basic
1. What is a Conditional Statement?
2. What is the purpose of the `if` statement?
3. When does an `if` statement execute?
4. What type of value must an `if` condition return?
5. What happens if the condition is false?

---

## Intermediate
1. Explain the `if` statement with an example.
2. Why are Conditional Statements important?
3. Can we write an `if` statement without braces?
4. What is the difference between `=` and `==` inside an `if` statement?
5. Give three real-life examples of the `if` statement.

---

# Summary
- Conditional Statements are used for decision making.
- `if` executes only when the condition is true.
- If the condition is false, the code is skipped.
- The condition must always return a boolean value.

---

# (Part-2)

## Table of Contents

1. if-else Statement
2. Flowchart
3. Java Examples
4. else-if Ladder
5. Flowchart
6. Java Examples
7. Real-Life Examples
8. Important Notes
9. Common Beginner Mistakes
10. Interview Questions
11. Summary

---

# if-else Statement

## English
The `if-else` statement is used when there are only two possible outcomes.
If the condition is true, the `if` block executes.
If the condition is false, the `else` block executes.

---

## Hindi
`if-else` statement tab use hoti hai jab sirf do possible results hote hain.
Agar condition true ho to `if` block execute hota hai.
Agar condition false ho to `else` block execute hota hai.
---

# Syntax

```java
if (condition) {

    // Code if condition is true

} else {

    // Code if condition is false

}
```

---

# Flowchart

```
          Condition

             |

        +----+----+

        |         |

      True      False

        |         |

    if Block   else Block
```

---

# Example 1

```java
public class Demo {

    public static void main(String[] args) {

        int age = 16;

        if (age >= 18) {

            System.out.println("Eligible for Voting");

        } else {

            System.out.println("Not Eligible for Voting");

        }

    }

}
```

Output

```
Not Eligible for Voting
```

---

# Example 2

```java
public class Demo {

    public static void main(String[] args) {

        int number = 10;

        if (number % 2 == 0) {

            System.out.println("Even Number");

        } else {

            System.out.println("Odd Number");

        }

    }

}
```

Output

```
Even Number
```

---

# Example 3

```java
public class Demo {

    public static void main(String[] args) {

        int marks = 28;

        if (marks >= 33) {

            System.out.println("Pass");

        } else {

            System.out.println("Fail");

        }

    }

}
```

Output

```
Fail
```

---

# else-if Ladder

## English
The `else-if` ladder is used when there are multiple conditions.
Java checks the conditions one by one.
As soon as one condition becomes true, its block executes and the remaining conditions are skipped.

## Hindi
`else-if` ladder ka use tab kiya jata hai jab multiple conditions ko check karna ho.
Java conditions ko ek-ek karke check karta hai.
Jis condition ka result pehle true hota hai, uska block execute hota hai aur baaki conditions check nahi hoti.

---

# Syntax

```java
if (condition1) {

    // Code

} else if (condition2) {

    // Code

} else if (condition3) {

    // Code

} else {

    // Default Code

}
```

---

# Flowchart

```
Condition 1

   |

True ------> Execute

   |

False

   |

Condition 2

   |

True ------> Execute

   |

False

   |

Condition 3

   |

True ------> Execute

   |

False

   |

else Block
```

---

# Example

```java
public class Demo {

    public static void main(String[] args) {

        int marks = 75;

        if (marks >= 90) {

            System.out.println("Grade A");

        } else if (marks >= 75) {

            System.out.println("Grade B");

        } else if (marks >= 60) {

            System.out.println("Grade C");

        } else {

            System.out.println("Fail");

        }

    }

}
```

Output

```
Grade B
```

---

# Real-Life Examples

## Weather

```java
if (temperature > 40)
```

Very Hot

```java
else if (temperature > 30)
```

Hot

```java
else
```

Normal Weather

---

## Student Grades

```
90+  → Grade A

75+  → Grade B

60+  → Grade C

Below 33 → Fail
```

---

## Shopping Discount

```
Amount > 5000
↓
20% Discount
Amount > 3000
↓
10% Discount
Otherwise
↓
No Discount
```

---

# Important Notes
- `if-else` is used when there are only two outcomes.
- `else-if` is used when there are multiple conditions.
- Only one block executes in an `else-if` ladder.
- The `else` block is optional but recommended.

---

# Common Beginner Mistakes

Wrong
```java
if (marks >= 90)

System.out.println("A");

else

System.out.println("B");
```

Correct
```java
if (marks >= 90) {

    System.out.println("A");

} else {

    System.out.println("B");

}
```

Reason
Always use braces `{}` for better readability.

---

Wrong
```java
if (marks >= 60) {

}

if (marks >= 75) {

}
```

Correct
```java
if (marks >= 75) {

} else if (marks >= 60) {

}
```

Reason
Using separate `if` statements may execute multiple blocks.

---

# Interview Questions

## Basic
1. What is the difference between `if` and `if-else`?
2. When should we use `else-if`?
3. Can an `if-else` statement have more than two outcomes?
4. Is the `else` block mandatory?
5. How many blocks execute in an `else-if` ladder?

---

## Intermediate
1. Explain the `if-else` statement with an example.
2. Explain the `else-if` ladder with an example.
3. Why is the order of conditions important in an `else-if` ladder?
4. What happens if multiple conditions are true?
5. Give three real-life examples of the `else-if` ladder.

---

# Summary
- `if` is used for a single condition.
- `if-else` is used when there are two possible outcomes.
- `else-if` is used when there are multiple conditions.
- In an `else-if` ladder, only the first true condition executes.
- The `else` block executes only when all conditions are false.

---

# (Part-3)
## Table of Contents

1. Nested if Statement
2. Flowchart
3. Java Examples
4. switch Statement
5. Syntax
6. break Keyword
7. default Case
8. Difference Between if-else and switch
9. Real-Life Examples
10. Important Notes
11. Common Beginner Mistakes
12. Interview Questions
13. Summary

---

# Nested if Statement

## English
A Nested if means writing one `if` statement inside another `if` statement.
It is used when one condition depends on another condition.

## Hindi
Nested if ka matlab hai ek `if` statement ke andar dusri `if` statement likhna.
Iska use tab kiya jata hai jab ek condition dusri condition par depend karti ho.

---

# Syntax

```java
if (condition1) {

    if (condition2) {

        // Code

    }

}
```

---

# Flowchart

```
Condition 1

    |

True

    |

Condition 2

    |

True ------> Execute Code

False -----> Skip

False -----> End
```

---

# Example 1

```java
public class Demo {

    public static void main(String[] args) {

        int age = 20;
        boolean citizen = true;

        if (age >= 18) {

            if (citizen) {

                System.out.println("Eligible for Voting");

            }

        }

    }

}
```

Output

```
Eligible for Voting
```

---

# Example 2

```java
public class Demo {

    public static void main(String[] args) {

        String username = "admin";
        String password = "1234";

        if (username.equals("admin")) {

            if (password.equals("1234")) {

                System.out.println("Login Successful");

            }

        }

    }

}
```

Output

```
Login Successful
```

---

# switch Statement

## English

The `switch` statement is used when we have multiple fixed choices.

Instead of writing many `else-if` conditions, we can use `switch`.

---

## Hindi

`switch` statement ka use tab kiya jata hai jab multiple fixed choices ho.

Bahut saare `else-if` likhne ki jagah `switch` ka use kiya jata hai.

---

# Syntax

```java
switch (expression) {

    case value1:
        // Code
        break;

    case value2:
        // Code
        break;

    case value3:
        // Code
        break;

    default:
        // Default Code

}
```

---

# Example

```java
public class Demo {

    public static void main(String[] args) {

        int day = 3;

        switch (day) {

            case 1:
                System.out.println("Monday");
                break;

            case 2:
                System.out.println("Tuesday");
                break;

            case 3:
                System.out.println("Wednesday");
                break;

            default:
                System.out.println("Invalid Day");

        }

    }

}
```

Output

```
Wednesday
```

---

# break Keyword

## English

The `break` statement terminates the current case.

Without `break`, Java executes the next cases also.

---

## Hindi

`break` current case ko wahi par stop kar deta hai.

Agar `break` na ho, to Java next cases bhi execute karta rahega.

---

# Example Without break

```java
int day = 2;

switch (day) {

    case 1:
        System.out.println("Monday");

    case 2:
        System.out.println("Tuesday");

    case 3:
        System.out.println("Wednesday");

    default:
        System.out.println("Invalid");

}
```

Output

```
Tuesday
Wednesday
Invalid
```

Reason

`break` nahi tha, isliye execution next cases me bhi chala gaya.

---

# Example With break

```java
int day = 2;

switch (day) {

    case 1:
        System.out.println("Monday");
        break;

    case 2:
        System.out.println("Tuesday");
        break;

    case 3:
        System.out.println("Wednesday");
        break;

    default:
        System.out.println("Invalid");

}
```

Output

```
Tuesday
```

---

# default Case

## English

The `default` block executes when no case matches.

It works like the `else` block.

---

## Hindi

Jab koi bhi case match nahi karta, tab `default` execute hota hai.

Ye `else` ki tarah kaam karta hai.

---

# Example

```java
int month = 15;

switch (month) {

    case 1:
        System.out.println("January");
        break;

    case 2:
        System.out.println("February");
        break;

    default:
        System.out.println("Invalid Month");

}
```

Output

```
Invalid Month
```

---

# Difference Between if-else and switch

| if-else | switch |
|----------|---------|
| Used for conditions | Used for fixed choices |
| Can use relational operators (`>`, `<`, `>=`) | Checks only matching values |
| Better for complex conditions | Better for menu-driven programs |
| Slower when many conditions exist | Easier to read with many fixed options |

---

# Real-Life Examples

## ATM Menu

```
1 → Balance

2 → Withdraw

3 → Deposit

4 → Exit
```

`switch` is a good choice.

---

## Traffic Signal

```
Red

Yellow

Green
```

`switch` can be used because choices are fixed.

---

## Student Result

```
marks >= 90
marks >= 75
marks >= 60
```

`if-else` is better because relational operators are required.

---

# Important Notes
- Nested if is used when one condition depends on another.
- switch is useful for fixed options.
- `break` prevents fall-through.
- `default` executes if no case matches.
- Every case should usually end with `break`.

---

# Common Beginner Mistakes

Wrong
```java
case 1

System.out.println("One");
```

Correct
```java
case 1:

    System.out.println("One");
    break;
```

Reason

A colon (`:`) is required after every `case`.

---

Wrong
```java
switch(day)

case 1:
```

Correct
```java
switch(day) {

    case 1:
        break;

}
```

Reason
Cases must be inside curly braces `{}`.

---

# Interview Questions

## Basic
1. What is Nested if?
2. What is a switch statement?
3. Why do we use the break keyword?
4. What is the purpose of the default case?
5. What happens if break is omitted?

---

## Intermediate
1. Explain Nested if with an example.
2. Explain switch with an example.
3. When should we use switch instead of if-else?
4. What is fall-through in a switch statement?
5. Explain the difference between if-else and switch.

---

# Summary
- Nested if means an `if` inside another `if`.
- switch is used for fixed choices.
- `break` stops execution after a matched case.
- Without `break`, the next cases also execute.
- `default` works like the `else` block.

---

#  (Part-4)
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

public class ConditionalDemo {

    public static void main(String[] args) {

        Scanner sc = new Scanner(System.in);

        System.out.print("Enter Your Marks: ");

        int marks = sc.nextInt();

        if (marks >= 90) {

            System.out.println("Grade A");

        } else if (marks >= 75) {

            System.out.println("Grade B");

        } else if (marks >= 60) {

            System.out.println("Grade C");

        } else if (marks >= 33) {

            System.out.println("Pass");

        } else {

            System.out.println("Fail");

        }

        sc.close();

    }

}
```

---

# Sample Output

Input
```
82
```
Output
```
Grade B
```

---

# Practice Programs

## Program 1
Take a number from the user and check whether it is positive or negative.

## Program 2
Take a number and check whether it is even or odd.

## Program 3
Take the user's age and check whether the user is eligible for voting.

## Program 4
Take marks as input and print the grade.

```
90 - 100 → Grade A
75 - 89 → Grade B
60 - 74 → Grade C
33 - 59 → Pass
Below 33 → Fail
```

## Program 5
Take two numbers and print the greater number.

## Program 6
Take three numbers and print the largest number.

## Program 7
Create a simple calculator using switch.
```
1 → Addition
2 → Subtraction
3 → Multiplication
4 → Division
```

## Program 8
Print the day name using switch.

```
1 → Monday
2 → Tuesday
3 → Wednesday
...
7 → Sunday
```

## Program 9
Print the month name using switch.

## Program 10
Create a menu-driven ATM program.

```
1 → Balance
2 → Withdraw
3 → Deposit
4 → Exit
```

---

# MCQs

### 1. Which statement is used for decision making?
A. loop
B. switch
C. if
D. class
Answer
```
C
```

---

### 2. Which statement is used when there are multiple fixed choices?
A. if
B. if-else
C. switch
D. for
Answer
```
C
```

---

### 3. Which keyword stops the execution of a switch case?
A. continue
B. stop
C. break
D. exit
Answer
```
C
```

---

### 4. Which block executes if no case matches?
A. else
B. finally
C. default
D. catch
Answer
```
C
```

---

### 5. Which operator is commonly used in an if condition?
A. ==
B. +
C. *
D. %
Answer
```
A
```

---

### 6. What happens if break is omitted in a switch statement?
A. Compilation Error
B. Program Stops
C. Next cases also execute
D. Nothing happens
Answer
```
C
```

---

### 7. Which statement checks multiple conditions one by one?
A. switch
B. else-if ladder
C. while
D. do-while
Answer
```
B
```

---

### 8. Which statement is used when one condition depends on another?
A. switch
B. Nested if
C. for
D. break
Answer
```
B
```

---

### 9. Which of the following returns a boolean value?
A. age + 5
B. age == 18
C. age * 2
D. age / 2
Answer
```
B
```

---

### 10. Which statement is best for menu-driven programs?
A. if
B. switch
C. while
D. do-while
Answer
```
B
```

---

# Viva Questions
1. What is a Conditional Statement?
2. What is an if statement?
3. What is an if-else statement?
4. What is an else-if ladder?
5. What is Nested if?
6. What is a switch statement?
7. Why is break used?
8. What is the default case?
9. When should we use if-else?
10. When should we use switch?

---

# Interview Questions

## Basic
1. Explain the if statement.
2. Explain if-else with an example.
3. What is an else-if ladder?
4. What is Nested if?
5. Explain switch with an example.

---

## Intermediate
1. Differentiate if-else and switch.
2. What is fall-through in switch?
3. What happens if break is not used?
4. Explain Nested if with a real-life example.
5. Why is switch preferred for menu-driven programs?

---

# Common Beginner Mistakes

### Mistake 1
Wrong

```java
if(age = 18)
```

Correct

```java
if(age == 18)
```

---

### Mistake 2
Wrong

```java
switch(day)

case 1:
```

Correct

```java
switch(day) {

    case 1:
        break;

}
```

---

### Mistake 3
Forgetting break

Wrong

```java
case 1:
    System.out.println("Monday");

case 2:
    System.out.println("Tuesday");
```

Correct

```java
case 1:
    System.out.println("Monday");
    break;

case 2:
    System.out.println("Tuesday");
    break;
```

---

### Mistake 4
Using switch for range conditions.

Wrong

```java
switch(marks >= 90)
```

Correct

```java
if(marks >= 90)
```

Reason

Use `if-else` for ranges and comparisons.

---

# Quick Revision
- `if` → Executes when the condition is true.
- `if-else` → Used when there are two possible outcomes.
- `else-if` → Used for multiple conditions.
- `Nested if` → One if inside another if.
- `switch` → Used for fixed choices.
- `break` → Stops execution of the current case.
- `default` → Executes when no case matches.

---

# Chapter Summary
In this chapter, we learned:

- if Statement
- if-else Statement
- else-if Ladder
- Nested if
- switch Statement
- break Keyword
- default Case
- Java Programs
- Practice Programs
- MCQs
- Viva Questions
- Interview Questions

Conditional Statements are the foundation of decision-making in Java. They are used in almost every real-world application such as ATM systems, login pages, grading systems, menu-driven programs, calculators, and many other applications.

---