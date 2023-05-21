--- 
title: Create simple calculator - Step 4
date: 2023-05-10 12:55:00 +100
categories: [python-tutorial]
tags: [python, learning, tutorial, programming-language]
img_path: /assets/img/Learn_to_Code_in_Just_30_Minutes/
image:
  path: learn_variables_in_python.svg
  alt: "Learn Variables in Python"
---

## Step 4: Learn Variables

### Theory.

What is the variable? 
- Objects with data are stored inside computer memory. 
- In the real world we use a post address when we need to visit some place or a building.
- Computers also use addresses to get access to a particular object in memory and it looks like this `0x00000284DE5A3E20`
- A variable is simply **a name** you give to a memory address where an object is stored.
- It's much simpler to remember that your data is located in a variable with name `data` rather than `0x00000284DE5A3E20`

> We use the equals sign "=" between variable name and an object we want to give this name to.
{: .prompt-info }

Let's use a variable in our first 'hello world' program, for now we simply give it the name "my_variable".
```python
my_variable = "hello world"
print(my_variable)
``` 

Here is what happens:
- We create a new variable and assign a string data to it.
- The print statement looks what memory address *variable*  represents.
- The print statement then fetches the text data in that memory location and outputs it into the terminal.

Let's also modify 'enter your name' program and use a variable to store the data a user enters:

```python
your_name = input("enter your name: ")
print(your_name)
```
Here is what happens:
- We create a new variable `your_name`
- `input("enter your name: ")` asks user to enter name in the Terminal. 
- As soon as user enters it and hits Enter key, input() sends this text to the `your_name` variable.
- The user's name is now stored inside this variable.
- The `print` statement then fetches the text data stored in an address represented by `your_name` and outputs it into the terminal.

> When a user enters their name it's going to be stored as **string**.
{: .prompt-info }


### Practice. 

Let's now start writing our calculator. 

- We want a user to enter two numbers and then print them in the terminal.
- Create first variable which will represent first number and read this data from the Terminal using input() function.
- Similarly, create second variable which will represent second number and read this data from the Terminal.
- Print both numbers using one print statement.  
- The result should look like this:
  ```python
  enter first number: 70
  enter second number: 7
  70 7
  ```

### Solution

```python
number_1 = input('enter first number: ')
number_2 = input('enter second number: ')
print(number_1, number_2)
```
 {% include button.html button_name="Go to the Next Step" button_class="outline-primary" url="/posts/py_calc-step5/" %}