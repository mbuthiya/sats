## Input and sys.argv

In our applications, we have basically been typing out everything.Now Let us see the different ways to handle user input

### `Input()` function

The `input()` function, is called inside our python application and  prompts the user to pass in an input, which is stored as a string.

Let us create a  new folder in our Lessons directory called Input, and create a new file `input_demo.py` and type in this.

```python
# Getting the name and age of the user

print("What is your name?")
name = input()

print("How old are you?")
age = int(input())

print(name)
print(age)

```
We then  run the file
```bash
$ python3.6 input_demo.py
"What is your name?"
James
"How old are you?"
19

'James'
19
```
Here we are prompting the user, for their name and age, and storing them in variables.
Since `age` is a number we used the `int()` function to convert it to an integer.

### Using the sys module
This module provides variables used or maintained by the interprater. The
`sys.argv`, provides a list of the command line arguments passed when running the program.

```python
# Getting the name and age of the user
import sys

name = sys.argv[1]

print("How old are you?")
age = int(input())

print(name)
print(age)

```
We then run the file
```bash
$ python3.6 input_demo.py James
"How old are you?"
19

'James'
19
```
Here we have first imported the `sys` module. Unlike the previous example, where we used `input()` to get the name of our user. Since the `sys.argv` returns a list
we used `sys.argv[1]`, this simply tells our application to pick the second argument at __index 1__ , when our application is run and store it as variable `name`.

You also notice when we run our application, we added a second argument `James`. This is what is picked by the `name` variable.

We can pass multiple arguments when we run our application.


```python
# Getting the name and age of the user
import sys

name = sys.argv[1]
age = sys.argv[2]

print(name)
print(age)

```
We then run the file
```bash
$ python3.6 input_demo.py James 19
'James'
19
```
Here we pick both the `name` and `age` from the command line arguments passed.

## Input and Type Casting Exercises

1. **Birthday dates**

	Create a program where you prompt a user for his age and return to him the year the person was born. And what year they will turn 80

 2. **Tip Caluclator**

	Create a program that calculates the tip  you could pay the  at a restaurant after a meal. You should be able to input the total bill, tip percentage (15% of total bill), level of satisfaction percentage(how happy were you with the service)

    Formula-example: Bill * 15/100* 10/100 (terrible service)


---
### Lesson 7: [Python Control Flows](./07_python_controlflow.md)
