## Functions
We have already used functions to perform several tasks like `range` and `print` but  let's learn how to create our own functions in python.

Functions are blocks of code that begin with the `def` keyword
```python
def fun_a():
    print("I have been called")

fun_a()

"I have been called"
```
This example we have created a function with no arguments and in the function we have a print statement that outputs a string

We then went on to call the function and we got our desired output.

#### Passing Arguments
In python you can also pass arguments to functions
```python
def fun_a (a,b):
    print(a+b)

fun_a(1,4)
5
```
Python can also take on **keyword arguments**. These are arguments that are already defined

```python
def fun_a(a = 1,b = 4):
    print(a+b)

fun_a(a=6,b=7);
13
```
Here, we created a function with two `keyword arguments`. When we call the function we changed the values of those arguments to our own values

We could  also call the function without passing any parameters. Then the default keyword arguments values will be passed in

```python
def fun_a(a = 1,b = 4):
    print(a+b)

fun_a();
5
```
#### Creating an Empty function

Sometimes we might want to define a function and not put code in it. This could be for whatever reason like outlining your code.

```python
# Empty function
def fun_a():

```
If we run our code like this, it will give us an error. Python has a keyword called **pass** that can help us here. `pass` allows us to create empty blocks of code because when it runs it returns a null or nothing.

```python
# Empty function
def fun_a():
    pass

```
Now when we run our code it will work perfectly.

#### Functions that return something

Functions can also return values to us

```python
def fun_a (a,b):
    return a+b

sum = fun_a(4,5)

print(sum)
9
```
Here, we use the `return` statement, to get the value from the operation performed in the function.

---
### Lesson 14 [Python Exceptions](./14_exceptions.md)
