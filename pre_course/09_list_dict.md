### Lists

**Lists**  are another python data type. They are the equivalent of arrays in other languages. A Python list can store any kind of value even nested lists.

```python
my_list = []
my_other_list =list()
```
We can create a list using square brackets `[]` or using the `list()` function .

```python
list_a = ["a","b","c","d"] # list of strings
list_b = [1,2,3,4,5,6] # list of numbers
list_c = [1,"west",34,"longitude"] # mixed list
list_d = [ ["a","b","c","d"],[1,2,3,4,5,6],[1,"west",34,"longitude"]] #nested list
```

As we can see with the code above we can create a list that holds similar types of items ie _strings or numbers_ or we can mix the types of data stored in our list.
We can even nest our lists with other lists.

We can Join two lists using the `extend()` method.

```python
list_a = ["a","b","c","d"]
list_b = [1,2,3,4,5,6]
# Joining list_b to list_a
list_a.extend(list_b)

print(list_a)
# ["a","b","c","d",1,2,3,4,5,6]

```
Here we have joined `list_b` to `list_a` and this creates new values to `list_a`. We can also append values to a list using the `append()` method.

```python
list_a = ["a","b","c","d"]
print(list_a)
# ["a","b","c","d"]
list_a.append("e")
print(list_a)
# ["a","b","c","d","e"]
```
Here we append a single value to the list.

We can also arrange list items in place using the `reverse()` and  `sort()` methods.
```python
list_a = ["a","b","c","d"]
list_a.reverse()

print(list_a)

# ['d', 'c', 'b', 'a']

```
Here we use the `reverse()` method to reverse the list.

```python
list_a = [1,3,4,8,5,7,6,2]
list_a.sort()

print(list_a)

# [1, 2, 3, 4, 5, 6, 7, 8]
```

The `sort()` method arranges items in order.




### Tuples

Tuples are Like lists the main difference between tuples and lists is that tuples are **immutable** - their values cannot be changed once created.

```python
tuple_a = ("a","b","c","d") # tuple of strings
tuple_b = (1,2,3,4,5,6) # tuple of numbers
tuple_c = [1,"west",34,"longitude"] # mixed tuple
tuple_d = tuple() #empty tuple
```
We can create a tuple using parentheses `()` or we can use the `tuple()` function

### Dictionary

Another really powerful data structure in python is the dictionary.Like lists, dictionaries store collections of many values of different types. Unlike indexes for lists - which are integers and start from 0, Dictionary indexes don't have to be integers. They can be  of different data types Like strings.  Indexes in Dictionaries are called **keys**

You can create dictionaries in two ways
```python
# Creating empty dictionaries
my_dict = {}
my_dict = dict()

# Example
my_cat = {'name':'Mr sniffles','age':18, 'color':'black'}

```


In the example above, we created a new dictionary that stores details about `my_cat` .
We can fetch data from a dictionary by using our key as the index.
```python
cat_name = my_cat['name']
print(cat_name)

'Mr sniffles'
```
Unlike lists dictionaries are unordered since the indexing does not start at [0]. We will see what that means later on

You can also add items to a dictionary by defining a new key and assigning it a value
```python
birthdays = {"John":"August 1","Marcus":"April 8"}
birthdays["mary"] = "September 14"
print(birthdays)

{"John":"August 1","Marcus":"April 8","Mary":"September 14"}

```
Here we had a dictionary with the birthday of 2 people `John` and	`Marcus` then we added `mary` to our birthday dictionary.

We can also get the individual keys in the dictionary  using the `keys()`method
```python
birthday = {"John":"August 1","Marcus":"April 8","Mary":"September 14"}

print(birthday.keys())

dict_keys(['John', 'Marcus', 'Mary'])

```
The `keys()` method creates a `dict_keys` object that holds a list of all the keys
You can convert them into a list using the `list()` function

```python
birthday = {"John":"August 1","Marcus":"April 8","Mary":"September 14"}

print(list(birthday.keys()))

['John', 'Marcus', 'Mary']

```
#### setdefault() method

When dealing with a dictionary, you might want to set up placeholder values to keys, before you do any operation on them, to prevent getting unnecessary errors.

For example we want to create an application that counts every character in an input string

```python

print("Enter a string")

input_string = input()

characters = {}

```
We prompt the user for an input. Then we create an empty dictionary that will store each individual character and how many times it has been used

```python
print("Enter a string")

input_string = input()

characters = {}

for character in input_string:
	characters.setdefault(character,0)
```
Here we use a `for` loop to iterate through each individual character in the string.
Then we use the `setdefault()` method to create a key for each character if the character does **not** exist in the dictionary. Then sets the default value for each as `0`.

```python
print("Enter a string")

input_string = input()

characters = {}

for character in input_string:
	characters.setdefault(character,0)
    characters[character] = characters[character] + 1

print(characters)
```
Lastly we target the key that matches the character and add one to the value everytime the character is encountered.


When we run this

```bash
$ python3.6 example.py
Enter a string
James is awesome

{' ': 3, 'J': 1, 'a': 2, 'e': 3, 'i': 1, 'm': 2, 'o': 2, 's': 4, 'w': 1}

```
---

## List and Dictionary Exercises

1. **Magic 8 ball**  

	Recreate the Magic 8 ball exercise using lists instead of `if` statements

 2. **Feature Phones**

	Create a program that allows a user to enter text and then you calculate how many clicks it takes for a user to input the text ignore uppercase and special characters

 	![Phone Keypad](https://i.stack.imgur.com/hHq4v.jpg)

    Example If a user inputs ***"James"*** the output should be ***10***


---
### Lesson 10: [Python Strings](./10_strings.md)
