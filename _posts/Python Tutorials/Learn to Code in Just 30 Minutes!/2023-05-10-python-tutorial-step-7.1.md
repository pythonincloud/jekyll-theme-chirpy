--- 
title: Step 7.1 - Learn Conditional Statements - the if statement
date: 2023-05-10 12:52:59 +100
categories: [python-tutorial]
tags: [python, learning, tutorial, programming-language]
img_path: /assets/img/Learn_to_Code_in_Just_30_Minutes/
image:
  path: learn_conditionals_in_python.svg
  alt: "Learn Conditionals Python"
---

## Theory: Overview

The Conditional Statements together with boolean operators and comparison operators allow us to define the **program flow**. This topic is quite big and there are lots of details to cover which might be overwhelming for a beginner.  
Therefore, in this section we'll cover only part of it, but nevertheless it should give you the sense of how it works. 

So far we've been executing all the lines of code one by one, from top to bottom. However, sometimes we want to skip some lines of our code because we want to use them only under certain circumstances.  
For that we use **the if, elif and else statements**. 

## Theory: the if statement

The "if statement" basically asks a straightforward question which can only result in 'yes' or 'no'. If the answer is 'yes', then it results in **True** value and Python executes actions suitable for this event. If the answer is 'no', it results in **False** value, and the 'if' actions won't be executed.
The True and False values are called **booleans**.

## Example

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
- The comparison operator `==` checks whether values of the two variables are equal.
- If that would be the case, we say "print a text to the screen and create third variable D which is a sum of A and B". 
- Since in the above example variable A is not equal to B, the third line `A == B` will result in False 
- Therefore, the lines 4 and 5 will NOT be executed.

![Python learn conditionals - the if statement example visualized](examples/python_learn_conditionals_the_if_statement_example_visualized.svg)
_Python learn conditionals - the if statement example visualized_



> Don't confuse assignment operator single `=` with comparison operator double `==`.
{: .prompt-warning }


## Practice: the if statement

In the previous step we've successfully created a simple program which can sum two numbers.  
Let's start gradually modifying it to handle different types of mathematical operations and apply what we've just learned.  

Here are the guidelines:
- Re-use the code we wrote in the previous Step 
- Ask a user to enter a mathematical operator  +, -, *, / : 
- Use the `if` statement to check if user enters `+` as the operator
- Don't worry about other operators, we'll learn how to handle them in the next steps
- If user enters `+` as the operator, calculate the sum and print the result
- The result should look like this:
  ```
    enter first number: 70
    enter math operator (+, -, *, /): +
    enter second number: 7
    the result is: 77
  ```

## Solution

```python
number_1 = int(input('enter first number: '))
operator = input('enter math operator (+, -, *, /): ')
number_2 = int(input('enter second number: '))

if operator == '+':
    print('the result is:', number_1 + number_2)
```

 {% include next-button.html button_name="Go to the Next Step" button_class="outline-primary" url="/posts/python-tutorial-step-7.2/" %}

