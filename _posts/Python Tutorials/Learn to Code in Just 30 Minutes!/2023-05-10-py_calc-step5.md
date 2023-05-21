--- 
title: Create simple calculator - Step 5
date: 2023-05-10 12:54:00 +100
categories: [python-tutorial]
tags: [python, learning, tutorial, programming-language]
img_path: /assets/img/Learn_to_Code_in_Just_30_Minutes/
image:
  path: Learn_strings_Concatenation_in_python.svg
  alt: "Learn Strings Concatenation in Python"
---


## Step 5: Learn Strings

### Theory.

Python allows you to merge two or more strings together. There are different methods to do it, but in this tutorial we'll focus on **string concatenation**.

We simply use the `+` sign with string concatenation:
```python
print('my name ' + "is " + "Python")
```
> Notice that I added extra space at the end of `'my name '` and `"is "`. 
> Without them it would result in `"my nameisPython"`.
{: .prompt-warning }

### Practice. 

Let's modify a bit our calculator. 

- Re-use the code we wrote in Step 5
- In line 3 use string concatenation so it will print it like this:  `You entered NUMBER_1 and NUMBER_2`
- Where NUMBER_1 and NUMBER_2 are the actual numbers user enters.
- The result should look like this:
  ```python
  enter first number: 70
  enter second number: 7
  You entered 70 and 7
  ```
### Solution

```python
number_1 = input('enter first number: ')
number_2 = input('enter second number: ')
print('You entered ' + number_1 + ' and ' + number_2)
```
 {% include button.html button_name="Go to the Next Step" button_class="outline-primary" url="/posts/py_calc-step6/" %}