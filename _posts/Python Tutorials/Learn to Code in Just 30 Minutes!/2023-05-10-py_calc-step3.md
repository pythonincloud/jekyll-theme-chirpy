--- 
title: <i class="fa-solid fa-calculator"></i> Create simple calculator - Step 3
date: 2023-05-10 12:56:00 +100
categories: [python-tutorial]
tags: [python, learning, tutorial, programming-language]
mermaid: true
---

## Step 3: Learn how to enter data in Terminal

### Theory

Since we're going to create a calculator, we somehow need to interact with user - ask them to enter numbers, and then provide a result.  

Let's now learn how to enter data in the terminal using Python. For that we use the **input()** function. 

About `input()`:
- We can put some text inside the `input()` function. 
- It will print this text first, and then will wait for user text data.
- You have to press the Enter key to actually execute it.

Example:

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

### Practice

Let's now practice how to enter data. 

- Ask a user to enter two numbers
- Use two `input()` statements for that
- The result should look like this:
  ```python
  enter first number: 70
  enter second number: 7
  ```

### Solution

```python
input('enter first number: ')
input('enter second number: ')
```

 {% include button.html button_name="Go to the Next Step" button_class="outline-primary" url="/posts/py_calc-step4/" %}