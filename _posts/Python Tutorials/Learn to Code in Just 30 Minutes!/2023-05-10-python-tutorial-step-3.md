--- 
title: Step 3 - Learn how to enter data in Terminal
date: 2023-05-10 12:56:00 +100
categories: [python-tutorial]
tags: [python, learning, tutorial, programming-language]
img_path: /assets/img/Learn_to_Code_in_Just_30_Minutes/
image:
  path: learn_how_to_enter_data_in_terminal.svg
  alt: "Learn how to enter data in terminal"
---

## Theory

Since we're going to create a calculator, we somehow need to interact with a user - ask them to enter numbers, and then provide a result.  

Let's now learn how to enter data in the terminal using Python. For that we use the **input()** function. 

**About** `input()`:
- We can put some text inside the `input()` function. 
- It will print this text first, and then will wait for user text data.
- You have to press the Enter key to actually execute it.

## Example

1. Run the below code:
```python
input('enter your name: ')
```
2. Enter your name and hit the enter key.

Here is what happens:
- As you noticed nothing happens after you hit the enter key.  
- The program just stops.  
- This is expected since we don't yet use the name we entered in the program.  
- To actually use the entered name we need to learn about **variables** in the next step.

python_input_function_example_visualized

![Python Input function example visualized](examples/python_input_function_example_visualized.svg)
_Python Input function example visualized_

## Practice

Let's now practice how to enter data. 

- Ask a user to enter two numbers
- Use two `input()` statements for that
- The result should look like this:
  ```python
  enter first number: 70
  enter second number: 7
  ```

## Solution

```python
input('enter first number: ')
input('enter second number: ')
```

 {% include next-button.html button_name="Go to the Next Step" button_class="outline-primary" url="/posts/python-tutorial-step-4/" %}