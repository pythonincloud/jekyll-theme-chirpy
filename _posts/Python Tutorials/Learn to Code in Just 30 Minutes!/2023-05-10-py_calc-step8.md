--- 
title: Create simple calculator - Step 8
date: 2023-05-10 12:51:00 +100
categories: [python-tutorial]
tags: [python, learning, tutorial, programming-language]
img_path: /assets/img/Learn_to_Code_in_Just_30_Minutes/
image:
  path: learn_functions_in_python.svg
  alt: "Learn Functions in Python"
---

## Step 8: Learn Functions.

### Theory.

We have already used two functions: `print()` and `input()`. It's now time to create our own function!

A function is basically **a block of some code** which has a name.  

Why do we need functions? There are two main reasons why you want to create them:
1. You want to hide a complexity of some operations
2. You have repeated blocks of code  

In both cases wrapping some block of code into a function can help to increase **readability** of your code. 

Let's now create a simple function which takes two strings as input, merges them and then prints output:

```python
def print_two_strings(string1, string2):
    merged_string = string1 + string2
    print(merged_string)
```

In the above code:
- The first line is the function signature:
  - A function always starts with `def` keyword
  - Then you define the function name, in our case it's `print_two_strings`
  - Then you define what input values a function takes
- The second line:
  - Concatenates two strings together in `string1 + string2`
  - Creates a new variable with name `merged_string`
  - The result of concatenation is stored in the variable `merged_string`
- The third line uses the `print` function to show a result in the terminal.

If you will try to run just this block of code nothing is going to happen. That is because we need a separate line of code to execute our function like this:
```python
print_to_strings('hello ', 'user')
```

> This separate line of code we just wrote above has its own name - *a function call*. 
{: .prompt-tip }

> Note that to execute or *call* a function you need to use parenthesis `()` after a function name. 
{: .prompt-info }

### Practice.

Here are the guidelines for this practice section:
- You need to create 4 different functions
- Each of these function performs its own mathematical operation:
  - The first adds two numbers together and prints the result
  - The second subtracts first number from second number and prints the result
  - The third adds multiplies numbers together and prints the result
  - The fourth divides first number by second number and prints the result
- Modify the condition block in previously created code to use these functions.


### Solution
```python
def add(number_1, number_2):
  result = number_1 + number_2
  print(result)

def subtract(number_1, number_2):
  result = number_1 - number_2
  print(result)

def multiply(number_1, number_2):
  result = number_1 * number_2
  print(result)

def divide(number_1, number_2):
  result = number_1 / number_2
  print(result)

number_1 = int(input('enter first number: '))
number_2 = int(input('enter second number: '))
operator = input('enter math operator: +, -, *, / : ')

if operator == '+':
    add(number_1, number_2)
elif operator == '-':
    subtract(number_1, number_2)
elif operator == '*':
    multiply(number_1, number_2)
elif operator == '/':
    divide(number_1, number_2)    
else:
    print('Unknown operator')
```

 {% include button.html button_name="Go to the Next Step" button_class="outline-primary" url="/posts/py_calc-step9/" %}