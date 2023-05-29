--- 
title: Step 9 - Learn the While Loop.
date: 2023-05-10 12:50:00 +100
categories: [python-tutorial]
tags: [python, learning, tutorial, programming-language]
img_path: /assets/img/Learn_to_Code_in_Just_30_Minutes/
image:
  path: learn_the_while_loop_in_python2.svg
  alt: "Learn the While loop in Python"
---

## Theory.

The while loop in Python is like a repetitive task that continues as long as a certain condition remains **True**.

It's similar to driving on a road until you reach a specific destination. Imagine you are on a road trip with your family and driving a car. Your wife wants have a conversation with you and your kids are constantly asking whether we already reached the hotel, and also don't forget to periodically check the fuel level, otherwise you risk to delay your trip. 

Here is the general concept of the While Loop visualized:
![The flow diagram describing the While loop in Python](examples/the_while_loop_flow_diagram_in_python.svg){: width="500"}
_The flow diagram describing the While loop in Python_

### Example #1

Let's go to more practical side of learning the While Loop and write some simple Python code:

```python
num = 0

while num < 5:
    print('current num is: ', num)
    num = num + 1

print('final num is: ', num)
```

In the above code:
- We created a variable `num` with initial value `0`
- In the While loop, using the comparison operator `<` we check whether the value of this variable is **less than** `5`
- If this expression results in True:
  - print the current number
  - increase it by 1
  - go back to the line 3 and check the condition again.

Here is the source code from the first example visualized:
![The flow diagram describing the While loop in Python - Example #1](examples/the_while_loop_flow_diagram_in_python_example.svg){: width="500"}
_The flow diagram describing the While loop in Python - Example #1_


And here is the result
```python
current num is:  0
current num is:  1
current num is:  2
current num is:  3
current num is:  4
final num is:  5
```

### Example #2

> The below part might be confusing, if the explanation is not clear, please leave your question in the comments below.
{: .prompt-danger }

Technically, the while loop condition can just have the **True object** and NO condition check, however in this case you have to make sure that your code can **break** from the loop *when a certain condition happens*. 

> Always test that the break condition can happen, otherwise your program will stuck in endless execution
{:.prompt-warning }

Let's now write the source code:

```python
num = 0

while True:
    num = num + 1
    if num == 5:
        break
    print('current num is: ', num)        

print('final num is: ', num)
```

In the above code:
- We created a variable `num` with initial value `0`
- In the While Loop initial statement, the condition check is replaced by the **True object**
- Since this expression is True itself:
  - increase current num value by 1
  - check if the current num **equals** to 5:
    - if that's the case, exit from the loop immediately and don't go back to the line #3 anymore.
    - if not, continue executing the code which is still left inside the While Loop, and then go back to the beginning of the While Loop again.
  - print the current number

Here is the source code from the second example  visualized:
![The flow diagram describing the While loop in Python - Example #2](examples/the_while_loop_flow_diagram_in_python_example-2.svg){: width="500"}
_The flow diagram describing the While loop in Python - Example #2_


### Practice.

- You'll modify the previously created code to use the While loop now
- You want the calculator to always work and ask a user to perform calculations
- You don't need an explicit exit condition
- The loop is going to end when the program is closed


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

while True:
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
