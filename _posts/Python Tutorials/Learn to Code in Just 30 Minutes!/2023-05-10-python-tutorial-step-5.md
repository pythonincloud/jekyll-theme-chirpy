--- 
title: Step 5 - Learn how to merge Strings
date: 2023-05-10 12:54:00 +100
categories: [python-tutorial]
tags: [python, learning, tutorial, programming-language]
img_path: /assets/img/Learn_to_Code_in_Just_30_Minutes/
image:
  path: Learn_strings_Concatenation_in_python.svg
  alt: "Learn Strings Concatenation in Python"
---

## Theory

Imagine you have a box of puzzle pieces, and each piece contains a part of a picture. To see the complete picture, you need to join all the pieces together. Similarly, when you merge strings in Python, you're essentially combining different pieces of text to form a cohesive whole.

You might be wondering, why do you even need to merge strings? The answer is that very often we need to produce some text, where some pieces are created dynamically. For example, we need to send an email to 100 people. We wrote a core content and we would like to personalize each email by adding someone's name into emails greeting. We can do something like:

```text
Dear {NAME}

We have wonderful news, click here to learn more!

```

There are different methods to merge two or more strings, but in this tutorial we'll focus on **string concatenation**.

## Example #1

With string concatenation method we simply put the `+` sign between strings we would like to merge:
```python
print('my name ' + "is " + "Python")
```

Here is what happens:
- We defined 3 different strings
- All these strings are merged by the `+` sign in the order we have defined
- The merged string then printed by the print() function

![Python Strings concatenation example visualized](examples/python_strings_concatenation_example_visualized.svg)
_Python Strings concatenation example visualized_


> Notice that I added extra space at the end of `'my name '` and `"is "`. 
> Without them it would result in `"my nameisPython"`.
{: .prompt-warning }

## Example #2

Let's now merge strings where one of them is dynamically created by a user. For that we'll use the input() function.

```python
name = input('what is your name?: ')
print('Hello ' + name + '!')
```

Here is what happens:
- We ask a user to enter their name using `input()` function
- The user's name is stored in the `name` variable 
- The name is placed between `Hello ` and `!` strings and then all 3 strings are merged
- The merged string then printed by the print() function

![Python Strings concatenation with input function example visualized](examples/python_strings_concatenation_with_input_function_example_visualized.svg)
_Python Strings concatenation with input function example visualized_


## Practice. 

Let's modify a bit our calculator. 

- Re-use the code we wrote in the previous Step 
- Use string concatenation so it will print it like this:  `You entered NUMBER_1 and NUMBER_2`
- Where NUMBER_1 and NUMBER_2 are the actual numbers a user enters.
- The result should look like this:
  ```python
  enter first number: 70
  enter second number: 7
  You entered 70 and 7
  ```

## Solution
```python
number_1 = input('enter first number: ')
number_2 = input('enter second number: ')
print('You entered ' + number_1 + ' and ' + number_2)
```
 {% include next-button.html button_name="Go to the Next Step" button_class="outline-primary" url="/posts/python-tutorial-step-6/" %}