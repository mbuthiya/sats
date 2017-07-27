## Import

Python comes with a lot of pre written code called **modules** and **packages**
1. A module is a single python file that contains code to do a particular task.
2. A package are made up of one or more modules that are joined to perform a particular task

These modules and packages belong to Python's standard library. They extend Python's functionality, and it is important to learn how to use them.

To use these packages or modules we use the **import** Keyword

Lets try this
```python
import this
```
If you run this file you will see this printed out

```python
Sparse is better than dense.
Readability counts.
Special cases aren't special enough to break the rules.
Although practicality beats purity.
Errors should never pass silently.
Unless explicitly silenced.
In the face of ambiguity, refuse the temptation to guess.
There should be one-- and preferably only one --obvious way to do it.
Although that way may not be obvious at first unless you're Dutch.
Now is better than never.
Although never is often better than *right* now.
If the implementation is hard to explain, it's a bad idea.
If the implementation is easy to explain, it may be a good idea.
Namespaces are one honking great idea -- let's do more of those!
```

This is known as the `Zen of Python` it doesn't do much, but it is a nice way to show you how to import modules.

Let us look at a more useful module `math`

```python
import math

x = math.sqrt(9)
print(x)

y = math.ceil(x)
print(y)


3.0
3
```
Here, we imported  the `math` module and used its `sqrt()` method to square root our number and the `ceil()` method to round up our number.

The syntax to use when you are using module methods is `module_name.method_name(arguments)`

You can also import a module's method directly using **from** keyword

```python
from math import sqrt,ceil

x = sqrt(9)
print(x)

y = ceil(x)
print(y)

3.0
3
```
You notice here the syntax changes. When we use the `from` keyword, we can use the method name directly without referencing the module.


Let us use another fun module called **random**.

```python
import random

# We can generate a random number using the randint method

random_number = random.randint(0,10)

print(random_number)
```
When we run this

```bash
$ python3.6 example.py
4
```
Here used the `import` keyword, to get the random module.  From the module we used its `randint` method and passed in two parameters. When called the method, it returned a random number, from the range provided by the parameters.



---

## Input Exercise

1. **circumference**

    Write a program that calculates the circumference of a wheel. The formular is
    C=2πr. The diameter of the circle should be a random integer generated  by the random module

---
###  Lesson 6: [Python Input](./06_python_input.md)
