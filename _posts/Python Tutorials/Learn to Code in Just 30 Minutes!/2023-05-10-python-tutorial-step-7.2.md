--- 
title: Step 7.2 - Learn Conditional Statements - the else statement
date: 2023-05-10 12:52:58 +100
categories: [python-tutorial]
tags: [python, learning, tutorial, programming-language]
img_path: /assets/img/Learn_to_Code_in_Just_30_Minutes/
image:
  path: learn_conditionals_in_python.svg
  alt: "Learn Conditionals Python"
---

## Theory: the else statement

We learned, that the `if` statement must always result in `True` and only then Python can execute actions suitable for that event. But, what if we want to execute another set of actions in case the `if` condition results in `False`?  
The `else` statement allows us to achieve this intention.

## Example 

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

![Python learn Conditionals - the if and else statements example visualized](examples/python_learn_conditionals_the_if_and_else_statements_example_visualized.svg)
_Python learn Conditionals - the if and else statements example visualized_

## Practice: the else statement

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

## Solution

```python
number_1 = int(input('enter first number: '))
number_2 = int(input('enter second number: '))
operator = input('enter math operator (+, -, *, /): ')

if operator == '+':
    print('the result is:', number_1 + number_2)
else:
    print('Unknown operator')
```

 {% include next-button.html button_name="Go to the Next Step" button_class="outline-primary" url="/posts/python-tutorial-step-7.3/" %}

