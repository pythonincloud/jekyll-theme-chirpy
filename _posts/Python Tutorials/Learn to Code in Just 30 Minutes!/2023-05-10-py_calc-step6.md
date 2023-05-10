--- 
title: <i class="fa-solid fa-calculator"></i> Create simple calculator - Step 6
date: 2023-05-10 12:53:00 +100
categories: [python-tutorial]
tags: [python, learning, tutorial, programming-language]
mermaid: true
---

## Step 6: Learn how to do Math in Python. 

### Theory.

Doing Math in Python is easy. We just write a mathematical expression and that is it. For now, let's learn how to use **the most basic operators: `+`, `-`, `/` and `*`**.
```python
print(2 + 2)
print(2 - 2)
print(2 / 2)
print(2 * 2)
```

You now learned that the `+` operator has different behavior with strings and numbers:
- The `+` operator **merges strings** together (concatenation).
- The `+` operator performs the addition operation with numbers. 

But what if a number is surrounded by quotes like this `'11'`? 
Is it still number or a string?  

The answer is that in Python it's treated as a string regardless of operation.

To convert this `'11'` to actual numbers we need to use **the int() statement** like this:
```python
number = int('11')
```
> The process of conversion from string to a number and vice versa is called **casting**.
{: .prompt-info }

### Practice. 

- Re-use the code we wrote in Step 6 to ask user to enter two numbers
- Calculate sum of two numbers and output it 
- The result should look like this:
  ```
  enter first number: 70
  enter second number: 7
  The sum is:  77
  ```

> Make sure to convert numbers in strings into actual numbers
{: .prompt-tip }

### Solution

```python
number_1 = input('enter first number: ')
number_2 = input('enter second number: ')
number_1_casted = int(number_1)
number_2_casted = int(number_2)

sum_of_two = number_1_casted + number_2_casted
print('The sum is: ', sum_of_two)
```

 {% include button.html button_name="Go to the Next Step" button_class="outline-primary" url="/posts/py_calc-step7/" %}