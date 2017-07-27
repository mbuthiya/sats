## Python Basics


### Python shell

Python comes with a built in  **R-E-P-L** - _Read Evaluate Print Loop_ tool called the Python shell
This is really useful when we want to test out snippets of our code before we put it in the main program.

To access the python shell let's open our terminal and type in `python3.6`

```bash
$ python3.6

Python 3.6.0 (default, Nov 17 2016, 17:05:23)
[GCC 5.4.0 20160609] on linux
Type "help", "copyright", "credits" or "license" for more information.
>>>
```
We know we are in the shell when we see the `>>>` symbols. We type in `python3.6` so that we can tell our machine that we want to use the python 3.6 interpreter.

Let us create a simple  command that prints out "_Hello, Moringa!_"
```python
>>> print("Hello, Moringa!")
'Hello, Moringa!'
```
The `print()` is a python function that simply outputs data to a screen. Functions are just bits of code that perform a certain action.We will revisit functions later on.
The `'Hello, Moringa!'` in python is called a **string**. A string is just a way for python to represent text.  Let's consider more on strings.

### Strings

As we mentioned earlier strings are pythons way to represent textual data.
There are several ways to create strings :
```python
>>>  'This is a string'
This is a string
>>> "This is also a string"
This is also a string

```
In Python we can create strings with either single quotes `('')` or double quotes `("")` and Python treats them as the same thing

We can also create strings that run in multiple lines;

```python
>>>  """This is a string
    that spans several
    lines
"""
This is a string
    that spans several
    lines
```

We use the `(""")` triple quotes sign to create multi-line strings.

We can also join multiple strings using the `+` operator

```python
>>>  'This is a string ' + 'this is also a string'
This is a string this is also a string

```
There are also some string **methods** that add do some actions on the string.

```python
>>>  'This is a string'.upper()
THIS IS A STRING
>>>  'this is a string'.capitalize()
This is a string

>>>  'this is a string     '.strip()
This is a string
```
The `upper()` method is used to transform strings to uppercase. The `capitalize()` method transform the first letter of the string to a capital letter. The `strip()` method removes any trailing spaces in a string.

### Numbers

We can also do some math computations in python
```python
>>> 3 + 2 # addition
5
>>> 31 - 10 # subtraction
21
>>> 3 * 4 # multiplication
12
>>> 12 / 3 # division
4.0
>>> 12 % 5 # modulus
2
>>> 2 ** 4 # Exponential
16

```
Python supports all the basic mathematical operations . Here, we see an new character `#`, This hash or pound sign is python's way to create comments. Anything after the `#` is ignored by the Python interpreter.

We notice something when use the `/` operator it doesn't return a whole number but a number with a decimal point.It is referred to as a **float division**. In Python these are called **floats**.

```python
>>> 30 / 5
6.0
>>> 45 / 9
5.0
>>> 25 // 5
5
```
Here we see some more examples using the `/` to get floats. But we introduce another division operator in Python `//` this divides then rounds down the result and returns a whole number this is called the **integer division**.

---
## Python Basics Exercises

1. **BMI calculator**

	Create a program on the  python shell that allows you to calculate the Body mass index of the person. This is calculated by dividing a person's weight by their height in meters squared.


2. **Car Loans**

	Create a program on the python shell that will calculate how long it would take a person to pay off a car loan of $150,000 if the person only spends 25% of his salary of $15,000 to pay the loan  assuming no-interest is charged.

---
### Lesson 2: [Python Data-types](./02_python_datatypes.md)
