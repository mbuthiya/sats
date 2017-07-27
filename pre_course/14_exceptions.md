## Exceptions and Error Handling

In technical terms **Exception Handling**  is the mechanism for stopping normal program flow and continuing it at some surrounding code block.

Simply put it is the art of spotting fatal errors that may come up in our applications and handling those errors.

Right now an error breaks our application.

create a new Folder called Error-Handling  and inside create a file `handle.py`

```python

def get_age():
	print("How old are you ")
	age = int(input())
	return age

print(get_age())

```

Let's take this simple application for example where we get the age of a user

```bash
$ python3.6 handle.py
How old are you
19
19
```
The program works fine if we enter a number. But what if a user enters a name

```bash
$ python3.6 handle.py
How old are you
nineteen

Traceback (most recent call last):
  File "testapp.py", line 6, in <module>
    input_age = get_age()
  File "testapp.py", line 3, in get_age
    age = int(input())
ValueError: invalid literal for int() with base 10: 'age'

```
We get a ValueError  because we put in a non integer string and the int() constructor cannot convert the string to integer.

This error is difficult to understand. Let us create a more understandable error message

```python
def get_age():
    print("How old are you ")
    try:
        age = int(input())
        return age
    except ValueError:
        return "That was not a valid input"
```

We use the `try\except ` block to handle errors. Inside the `try` block we  put in code that may throw an Error and in the `except` block we catch the thrown error and provide code to handle that error.

#### Programmer Errors

There are some error that are caused by programmers themselves. These errors should not be handled but fixed.

1. **`IndentationError`** - When you fail to separate code blocks properly
2. **`NameError`** - when you call an undefined variable function or method
3. **`TypeError`** - when you try and perform operations on unrelated types

---

### Hey its time for  [Feedback](https://goo.gl/forms/f7C8z6fAq459Oofj2)
