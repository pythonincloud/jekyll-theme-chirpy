--- 
title: Create simple calculator - Step 2
date: 2023-05-10 12:57:00 +100
categories: [python-tutorial]
tags: [python, learning, tutorial, programming-language]
img_path: /assets/img/Learn_to_Code_in_Just_30_Minutes/
image:
  path: learn_how_to_print_data_in_python.svg
  alt: "Learn how to Print data in terminal"
---

## Step 2: Learn how to print data in Terminal

### Theory

In this tutorial we're going to use the **terminal** in order to interact with our program.  
You should be already familiar with Graphical User Interface (GUI) as you see it everywhere in modern world: 
- It's the graphical interface of OS  in Windows or Mac
- or a browser are GUI based.  

Terminal is also an interface to interact with your computer, but it's **text based**. It allows us to input data or output data in text format. 

Let's now learn how to output some data with Python and write our first program.  
In Python it's very simple, for that we use **the `print()` statement**.

> As you might have guessed, the print command prints something. But don't worry, it doesn't require a **physical printer** to do its job, instead it's going to print text in your **Terminal**.
{: .prompt-info }

Let's write the first program:
1. Open the VS Code.
2. Navigate to File -> Open Folder. 
3. Create a new folder with name `code` and open it.
4. On the right hand side click to Explorer
5. Right click on the empty space and select "New File"
6. Give the file a name, for example "test.py"
7. In the editor type the text below 
8. Click to the Run Python File button on the right top corner.
9. The result will be in the bottom part of VS Code - this is **Terminal**.

```python
print('hello world') 
```

> Note, that the text data in Python is called **string** and it's always surrounded by **quotes**.
{: .prompt-info }

> Congratulations, you wrote your first Python program 
{: .prompt-tip }

More about `print`:
- The `print` statement we just used is in fact a **function**
- You can execute a function by adding a pair of parenthesis `()` to it like this `print()`
- Functions can take input values which are called **arguments**
- The arguments are always inserted **inside the parenthesis**
- We're going to learn more about the functions later in this tutorial
- The `print` function can be used to print almost any type of data in Python: text, numbers, objects and so on
- If you just want to print a new line with no text simply use it with no arguments like this `print()`
- The print function in fact can take multiple arguments or values, you just need to separate them by `,`

Example of print function with two arguments:

```python
print('hello world', "hello universe") 
```

Note that we used single quotes to surround `'hello world'` and double quotes in `"hello universe"`. 
> In Python you can use either single or double quotes, but remember to put the same type of quotes at the beginning and the end of a string.
{: .prompt-info }

### Practice 

Since we're going to create a calculator, we need to print results on the screen. Let's now pretend we have already calculated them. 

- The results are the numbers 77, 11 and 17
- For each number print 'the result is: ' and then the number
- Make sure to supply two arguments to the `print` function: first is text and the second is the number

### Solution

```python
print('the result is: ', 77)
print('the result is: ', 11)
print('the result is: ', 17)
```

 {% include button.html button_name="Go to the Next Step" button_class="outline-primary" url="/posts/py_calc-step3/" %}