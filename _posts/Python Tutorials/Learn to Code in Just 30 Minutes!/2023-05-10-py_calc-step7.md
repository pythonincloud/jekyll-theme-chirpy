--- 
title: <i class="fa-solid fa-calculator"></i> Create simple calculator - Step 7
date: 2023-05-10 12:52:00 +100
categories: [python-tutorial]
tags: [python, learning, tutorial, programming-language]
mermaid: true
---

## Step 7: Learn Conditional Statements

### Theory: Overview

The Conditional Statements together with boolean operators and comparison operators allow us to define the **program flow**. This topic is quite big and there are lots of details to cover which might be overwhelming for a beginner.  
Therefore, in this section we'll cover only part of it, but nevertheless it should give you the sense of how it works. 

So far we've been executing all the lines of code one by one, from top to bottom. However, sometimes we want to skip some lines of our code because we want to use them only under certain circumstances.  
For that we use **the if, elif and else statements**. 

### Theory: the if statement

The "if statement" basically asks a straightforward question which can only result in 'yes' or 'no'. If the answer is 'yes', then it results in **True** value and Python executes actions suitable for this event. If the answer is 'no', it results in **False** value, and the 'if' actions won't be executed.
The True and False values are called **booleans**.

Let's now check the example:
```python
A = 1
B = 2
if A == B:
    print("A equals to B event happened")
    D = A + B
```
> Note that there is a lot of whitespaces in the beginning of lines 4 and 5, this is called **a code block** and it's mandatory to have after the 'if', 'elif' or 'else' statements.
{: .prompt-info }

In the above example we do following:
- On the lines 1 and 2 we create two variables A and B.
- On the line 3 we ask Python if two variables are equal with the comparison operator `==`.
- If that would be the case, we say "print a text to the screen and create third variable D which is a sum of A and B". 
- Since in the above example variable A is not equal to B, the third line `A == B` will result in False 
- Therefore, the lines 4 and 5 will NOT be executed.

> Don't confuse assignment operator single `=` with comparison operator double `==`.
{: .prompt-warning }


### Practice: the if statement

In the step 7 we've successfully created a simple program which can add two numbers together.  
Let's start gradually modifying it to handle different types of mathematical operations and apply what we've just learned.  

- Re-use the code we wrote in Step 7 to ask user to enter two numbers
- Ask a user to enter a mathematical operator  +, -, *, / : 
- Use the `if` statement to check if user enters `+` as the operator
- If that the case calculate the sum and print the result
- The result should look like this:
  ```
    enter first number: 70
    enter second number: 7
    enter math operator (+, -, *, /): +
    the result is: 77
  ```

### Solution

```python
number_1 = int(input('enter first number: '))
number_2 = int(input('enter second number: '))
operator = input('enter math operator (+, -, *, /): ')

if operator == '+':
    print('the result is:', number_1 + number_2)
```

### Theory: the else statement

So the if statement must always result in True and only then we can execute actions suitable for that event. But, what if we want to execute another set of actions after the 'if' statement results in False?  
**The else statement** allows us to achieve this intention.

Let's modify the previous example:
```python
A = 1
B = 2
if A == B:
    print("A equals to B event happened")
    D = A + B
else:
    print("A does NOT equal to B")
```

In the above example we do following:
- Create two variables A and B and check if they are equal on the 3rd line. 
- Since they are not equal, lines 4 and 5 won't be executed. 
- Therefore Python checks if there is `else` statement, and we have it present on the 6th line.
- Python then executes line 6 and prints text since it's inside the `else` block.

> The `else` statement cannot be used alone without the `if` statement.
{: .prompt-warning }

### Practice: the else statement

Let's continue writing the calculator.  We're going to use the `else` statement as an indication that user didn't enter a math operator we have expected `+, -, *, /`. Therefore we want to handle this situation and print `Unknown operator`.

Here are the guidelines:
- Re-use the code we wrote in Step 8
- Write the else statement, its block should just print `Unknown operator`
- The result should look like this:
  ```
    enter first number: 70
    enter second number: 7
    enter math operator (+, -, *, /): ^
    Unknown operator
  ```

### Solution

```python
number_1 = int(input('enter first number: '))
number_2 = int(input('enter second number: '))
operator = input('enter math operator (+, -, *, /): ')

if operator == '+':
    print('the result is:', number_1 + number_2)
else:
    print('Unknown operator')
```

 {% include button.html button_name="Go to the Next Step" button_class="outline-primary" url="/posts/py_calc-step8/" %}