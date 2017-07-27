## Slicing

Slicing is act of getting subsets or parts of strings,lists or tuples. Let's get "slicing".


```python
greetings = 'Hello, Moringa!'

part_one = greetings[0:5]
print(part_one)

```
When we run this we get:
```bash
$ python3.6 example.py
Hello
```
A slice statement  is enclosed with `[]` square brackets and has two parts first is the position where to start slicing  and second is the position to stop but not including that position.

`[start:stop]`

In the example above, we sliced the `greetings` variables, took the characters in the first 5 indexes and stored them in the variable `part_one`

You can also use negative indexes when slicing.

```python
greetings = 'Hello, Moringa!'

part_one = greetings[-8:-1]
print(part_one)

```
When we run this we get:
```bash
$ python3.6 example.py
Moringa
```
In this code we start slicing counting backwards and get `Moringa` as our output

```python
greetings = 'Hello, Moringa!'

part_one = greetings[0:]
print(part_one)

```
When we run this we get:
```bash
$ python3.6 example.py
Hello, Moringa!

```
We can also choose not to specify the start or end point of our slices. In this example, Python assumes that we want to slice from index `0`, to the last item and automatically fills in that value.

We can also slice lists

```python
number = [1,2,3,4,5,6,7,8,9]
four_digits = number[:4]
print(four_digits)

```
When we run this we get:
```bash
$ python3.6 example.py
[1,2,3,4]

```
Here we did not specify the beginning of our slice and python automatically filled that in to be at index `0`.

---
### Lesson 13 [Python Functions](./13_functions.md)
