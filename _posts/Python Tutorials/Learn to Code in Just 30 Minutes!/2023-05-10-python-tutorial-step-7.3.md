--- 
title: Step 7.3 - Learn Conditional Statements - the elif statement
date: 2023-05-10 12:52:57 +100
categories: [python-tutorial]
tags: [python, learning, tutorial, programming-language]
img_path: /assets/img/Learn_to_Code_in_Just_30_Minutes/
image:
  path: learn_conditionals_in_python.svg
  alt: "Learn Conditionals Python"
---

## Theory: the elif statement

Alright, we learned that the `if` statement asks only one question and together with the `else` statement we can execute certain actions which would be suitable when an event occurs or it doesn't occur.  

But, what if we wanted to ask multiple questions and do different actions based on their responses?  

In Python we use **the `elif` statement** to address that. 

## Example 

Here is the example where I added `elif` on line 7:
```python
A = 1
B = 2
C = 1
if A == B:
    print("A equals to B event happened")
    D = A + B
elif A == C:
    print("A equals to C event happened")
    D = A + C
else:
    print("A does NOT equal to B or to C")
```

In the above example we do following:
- On first 3 lines create three variables A, B and C.
- On line #4 Python checks if A and B are equal with `==` and it results in False so the lines 5 and 6 will be skipped.
- On line #7 we ask Python if A and C variables are equal, again with the use of the comparison operator `==`
- Since A and C are equal, the lines 8 and 9 will be executed and we'll print a text and then we'll create the
-  variable D.
- Python will skip any code inside the `else` statement.

![Python learn Conditionals - the if and elif and else statements example visualized](examples/python_learn_conditionals_the_if_and_elif_and_else_statements_example_visualized.svg)
_Python learn Conditionals - the if and elif and else statements example visualized_

Here are **a few important concepts** to know:
- The combination of `if`, `elif` and `else` statements forms one **Conditional Block**.
- In one single Conditional block, we can write one if statement, one else statement and multiple elif statements. 
- When have multiple checks with `if` and `elif` statements - as soon as one of them results in True, the rest statements won't be processed.
- Example: Python finds out that a condition in `if` block is True, and therefore it won't be executing `elif` and `else` blocks.
- We can however write multiple Conditional Blocks - each of them starts with `if`. 
  - In this situation Python will check all of those Conditional Blocks.  


## Practice: the elif statement

Let's apply what we've just learned all together.  

Here are the guidelines:
- Re-use the code we previously wrote in Step 8
- We want to use the if, elif and else statement to check what is the math operator.
- Depending on the operator we want to execute the associated operation and print its result.
- If a user enters an invalid operator, we want to handle it and print text 'Unknown operator'.
- An example of the resulting program should look like this:
  ```
    enter first number: 70
    enter second number: 7
    enter math operator (+, -, *, /): -
    the result is: 63
  ```

## Solution

```python
number_1 = int(input('enter first number: '))
number_2 = int(input('enter second number: '))
operator = input('enter math operator: +, -, *, / : ')

if operator == '+':
    print('the result is:', number_1 + number_2)
elif operator == '-':
    print('the result is:', number_1 - number_2)
elif operator == '*':
    print('the result is:', number_1 * number_2)
elif operator == '/':
    print('the result is:', number_1 / number_2)    
else:
    print('Unknown operator')
```


 {% include next-button.html button_name="Go to the Next Step" button_class="outline-primary" url="/posts/python-tutorial-step-8/" %}

