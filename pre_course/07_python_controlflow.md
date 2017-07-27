## Control Flow

Up to now our applications haven't really been that interesting. Let us add some logic to our applications.

### If statements

An if statement runs only when the condition passed to it evaluates to true.
```python
height = 74 #inches
if height > 70 :
    print("You are really tall")

# You are really tall
```
Since  the `height` is above 70 the `if` statement will be called and it will print out the statement. Unlike most programming languages which use `{}` to hold blocks of code, python uses Indents. If we don't indent blocks of our code, we will get errors and our program won't run.

Let us look at some of the comparison operators we will be using in python
1. `>` Greater than
2. `<` Less than
3. `==`Equal to
4. `!=`not equal to
5. `>=` Greater than or equal to
6. `<=`Less than or Equal to
7. `and` Checks if both conditions evaluate to true
8. `or` Checks if at least one condition is true
9. `not` returns the opposite of the condition given

### else

The **else** statement comes right at the end of the `if` statement. It is run only when the if statement is `False`

```python
height = 54 #inches
if height > 70 :
    print("You are really tall")
else:
    print("You are really short")

# You are really short
```
The height is not greater than 70 so the `if` statement would prove `False` and the else statement will be called.

### elif

So what if we had more than one condition  to check for?  We can use `elif` which will allow us to check for multiple conditions

```python
height = 68 #inches
if height > 70 :
    print("You are really tall")
elif height > 60:
    print("You are of average height")

else:
    print("You are really short")

# You are average height
```
Since the height is greater than 60 the `elif` statement  will be executed first.

### Checking for nothing

In python an empty value is automatically considered to be `False`

```python
name = ""
list_a = []

if list_a:
    print("I am an empty list")

```
When we  run this command nothing happens. This is because the `if` statement only runs if the output evaluates to be `True`, and since our list is empty the condition will evaluate to `False`

### Looping

A loop is  a way to execute some piece of code over and over again.
There are 2 kinds of loops in python
1. For loop
2. While loop

#### For loop

A for loop is used when one wants to repeat something `n` times from a list . Just like the if statements, blocks of code in a for loop are indented otherwise they will not run

Here is an example of a  for loop in Python
```python
numbers = [1,2,3,4,5]

for number in numbers:
    print(number)

    1
    2
    3
    4
    5
```

The `for` statement loops through the numbers list,  and stores each individual number in a variable called `number`, then we print out this new variable we have created.
We can also use a Python function called `range()` in our for loops. The range function returns a list for which we can use to loop through.

First let us see how we use the `range()` function by creating a list.
```python
list_a = list(range(0,5))
print(list_a)

 [0,1,2,3,4]
```
The `range()`function can take on 2 parameters, the first one  is the number from where to start the range and the second one is where to stop the range but not including that number.
In our example here,  we start the range at 0 and end it at 5 but we use the list method to convert it to a list and prints out list `[0,1,2,3,4,5]`

```python
# Another example using range()

for i in range(0,7):
    print("I cookies",i)

  I cookies 0
  I cookies 1
  I cookies 2
  I cookies 3
  I cookies 4
  I cookies 5
  I cookies 6

```
Here we created a loop that prints out a string and what number the loop is at.

```python
# Another example using range()

for i in range(0,7):
    print("I cookies",i)

  I cookies 0
  I cookies 1
  I cookies 2
  I cookies 3
  I cookies 4
  I cookies 5
  I cookies 6

```
Let us create another example of a `for` loop with conditions.
```python
numbers = [1, 2, 3, 4, 5]
>for i in numbers:
    if i % 2 == 0:
        print(i)

2,4
```
Here we looped through the numbers list and checked if the number inside the list is fully divisible by 2 and printed out that number.

#### While Loops

Unlike `for` loops `while` loops  run until a certain condition is met.`while` loops are mostly used as counters.

```python
players = 11

while players >= 5 :
    print("The remaining players are",players)
    players -= 1


The remaining players are 11
The remaining players are 10
The remaining players are 9
The remaining players are 8
The remaining players are 7
The remaining players are 6
The remaining players are 5
```

Here we are using a variable called `players` and we are using the `while` loop to print out the numbers of players remaining and decrease the players by one.


---

## Control Flow Exercises

1. **Validator**

	Create a simple log-in application that prompts a user to input a name and password. validate the inputs with the `X string`  methods return an congratulatory message when both inputs are valid

 2. **Magic 8 ball**

	Create the popular magic 8 ball game. Allow a person to input a question, create a random number and based on the random number pick a  response  to the question using `if ` `elif` `else` statements . You can find the responses here :https://en.wikipedia.org/wiki/Magic_8-Ball


---
### Lesson 8: [Python Import](./08_python_break_continue.md)
