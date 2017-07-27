## Type casting

Type casting is the act of converting one type of data to another, so as to manipulate it in some way. Let's see an example of this.

```python
# print out user's name and age
name = "James"
age = 19

print("My name is "+name+" I am "+ age+" years old")
```
Let us run this code and see what happens.

```bash
$ python3.6 example.py

Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
TypeError: must be str, not int

```
Here we see we get a `TypeError`, because python cannot concatenate a string with an integer. To use the `age` variable we need to convert it to a string.


```python
# print out u users name and age
name = "James"
age = 19

print("My name is "+name+" I am "+ str(age)+" years old")
```
Let us run this code and see what happens.

```bash
$ python3.6 example.py

My name is James I am 19 years old

```
In this example we enclose the `age` variable in a function called `str()`. The `str()` function converts the `age` from an integer to a string.

There are other type conversion methods:
1. `int()` converts what is passed to an integer.
2. `float()` converts what is passed to a float.

Let us see more examples of this

```python
name = "James"
age = 19
weight = '79' # Killograms

age_weight_ratio = int(weight)/age

print(age_weight_ratio)

```
Run this
```bash
$ python3.6 example.py
4.157894736842105

```
Here we converted string `weight`,  to an integer and divided it by `age`.

---
### Lesson 12: [Python Slicing](./12_slice.md)
