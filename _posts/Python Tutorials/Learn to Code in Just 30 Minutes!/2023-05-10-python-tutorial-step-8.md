--- 
title: Step 8 - Learn Functions
date: 2023-05-10 12:51:00 +100
categories: [python-tutorial]
tags: [python, learning, tutorial, programming-language]
img_path: /assets/img/Learn_to_Code_in_Just_30_Minutes/
image:
  path: learn_functions_in_python.svg
  alt: "Learn Functions in Python"
---

## Theory.

We have already used two functions: `print()` and `input()`. It's now time to create our own function!

A function is basically **a block of some code** which has a name.  

Why do we need functions? There are two main reasons why you want to create them:
1. You want to hide a complexity of some operations
2. You have repeated blocks of code  

In both cases wrapping some block of code into a function can help to increase **readability** of your code. 

Imagine your friend is a chief and he knows a recipe for baking cookies. He knows that to make the cookies he has to take certain amount of ingredients and then perform some actions with them, like preparing ingredients, making a dough from them, then baking the dough and this will result in delicious cookies. In Python, a function is like asking your friend to cook cookies and at the same time giving the necessary ingredients to your friend, who will then apply his skills to make the cookies for you.

It's the same with functions: you supply input data to a function, the function will do some actions with this data and will produce a result for you.

## Example

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
def print_two_strings(string1, string2):
    merged_string = string1 + string2
    print(merged_string)

print_two_strings('hello ', 'user')
```

> This separate line of code we just wrote above has its own name - *a function call*. 
{: .prompt-tip }

> Note that to execute or *call* a function you need to use parenthesis `()` after a function name. 
{: .prompt-info }

## Practice.

Here are the guidelines for this practice section:
- Re-use the code we wrote in the previous Step 
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
operator = input('enter math operator: +, -, *, / : ')
number_2 = int(input('enter second number: '))

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

 {% include next-button.html button_name="Go to the Next Step" button_class="outline-primary" url="/posts/python-tutorial-step-9/" %}