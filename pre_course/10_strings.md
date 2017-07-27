## Strings

### String Formatting
This is a way of embedding variables into strings. It is pretty easy to do.

```python
name = "James"
age = 19

print(f"My name is {name} and I am {age} years old")

```
we run this
```bash
$ python3.6 example.py
My name is James and I am 19 years old
```
The `f` before the string stands for  **f-strings** or formatted strings and allow us to put replacement fields `{}` with variable names inside our strings

### Raw strings

A raw string is a special type of string that allows us to ignore all escape characters `\`  and print them out

```python
print('Beyonce\'s lemonade stand')
```
we run this

```bash
$ python example.py
Beyonce's lemonade stand

```
Here we see  a proper use of the escape `\` character, by allowing us to add an apostrophy. But let us create a raw string and see what happens

```python
print(r'Beyonce\'s lemonade stand')
```
we run this

```bash
$ python example.py
Beyonce\'s lemonade stand

```
We notice the `r` before the string. This means `raw` string. And in the output unlike the first example it prints out even the escape character.

### Is x string methods

1. isalpha() - returns True if the string consists of letters only and is not blank
2. isalnum() - returns True if the string consists of numbers and letters and is not blank
3. isdecimal() - returns True if the string contains only numeric characters
4. isspace() - returns True if the string contains only space,tabs or new lines
5. istitle() - returns True if the string contains words that start with uppercase letters

```python
alpha = "I like old music"
password = "K34jndnks"
number_string = "12345"
tabbs = "		"
titles = "I Love Cups"
false_titles = "I love Cups"

print( alpha.isalpha() )
print( password.isalnum() )
print( number_string.isdecimal() )
print( tabbs.isspace() )
print( title.istitle) )
print( false_titles.istitles())
```
When we run this

```bash
$ python3.6 example.py
True
True
True
True
True
False
```
The last print statement was false because not all the words in `false_titles` were in uppercase.

These `xstring ` methods are really useful when you want to do something like password validation

---
## String Exercises

1. **Mad Libs**

Create a mad libs kind of program that allows users to input word descriptions such as a "noun", a "verb", an "adjective" etc and create then display  a funny story from the users input
---
### Lesson 11: [Python Type casting](./11_type_casting.md)
