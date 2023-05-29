--- 
title: Step 6 - Learn how to do Math in Python. 
date: 2023-05-10 12:53:00 +100
categories: [python-tutorial]
tags: [python, learning, tutorial, programming-language]
img_path: /assets/img/Learn_to_Code_in_Just_30_Minutes/
image:
  path: learn_math_in_python.svg
  alt: "Learn how to do Math in Python"
---

## Theory

Python provides a good number of tools which will help you to solve mathematical problems, perform calculations, and analyze data.

The perfect use case is this tutorial where we create a calculator, and the nature of calculator is to perform different mathematical calculations.

Or, let's say you'd like to create a program which'll help you to manage your finances. The program can take your monthly expenses as input and then provide you statistics, how much did you spend on restaurants, groceries, entertainment, etc. 

## Example #1

Doing basic Math in Python is easy. We just write a mathematical expression and that is it. For now, let's learn how to use **the most basic operators: `+`, `-`, `/` and `*`**.

```python
print(2 + 2)
print(2 - 2)
print(2 / 2)
print(2 * 2)
```

Here is what happens:
- We provide two numbers in each line
- We provide different Math operators in each line
- Python performs respective calculation in each line
- The results go to the print functions and printed in the terminal

![Python basic Math operators example visualized](examples/python_basic_math_operators_example_visualized.svg)
_Python basic Math operators example visualized_


> You now learned that the `+` operator has different behavior with strings and numbers:
- The `+` operator **merges strings** together (concatenation).
- The `+` operator performs the addition operation with numbers. 
{: .prompt-tip }

## Example #2

But, what if a number is surrounded by quotes like this `'11'`?  Is it still a number or a string?  

The answer is that in Python it's treated as a string.

To convert this `'11'` to actual numbers we need to use **the int() function** like this:
```python
number = int('11')
```
![Python basic Math with Casting example visualized](examples/python_basic_math_with_casting_example_visualized.svg)
_Python basic Math with Casting example visualized_



> The process of conversion from string to a number and vice versa is called **casting**.
{: .prompt-info }

## Example #3

Now, let's use the int() function to convert strings into numbers while using the input() function.

> Remember, that the input() function stores the user entered data as a **string**.
{: .prompt-danger }

```python
number = input('enter your number: ')
number_casted = int(number)
squared = number_casted * number_casted
print('the squared number is: ' + squared)
```

Here is what happens:
- The `input()` function asks a user to enter a number
- The user entered number is stored in the variable `number` as a **string**
- The `int()` function coverts this stringified number into an actual number
- Python then calculates squared of this number and stores the result in the respective variable
- The `print()` function prints the result in the terminal.


![Python basic Math with Casting and input() function example visualized](examples/python_basic_math_with_casting_and_input_function_example_visualized.svg)
_Python basic Math with Casting and input() function example visualized_


## Practice. 

Let's modify our calculator further: 
- Re-use the code we wrote in the previous Step 
- Calculate sum of two numbers and output it 
- The result should look like this:
  ```
  enter first number: 70
  enter second number: 7
  The sum is:  77
  ```

> Make sure to convert numbers in strings into actual numbers
{: .prompt-tip }

## Solution

```python
number_1 = input('enter first number: ')
number_2 = input('enter second number: ')
number_1_casted = int(number_1)
number_2_casted = int(number_2)

sum_of_two = number_1_casted + number_2_casted
print('The sum is: ', sum_of_two)
```

 {% include next-button.html button_name="Go to the Next Step" button_class="outline-primary" url="/posts/python-tutorial-step-7.1/" %}