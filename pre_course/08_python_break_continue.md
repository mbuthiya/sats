### Break

The `break` statement allows us to "break out" of loops, after a certain condition has been met.

```python
number = 0
while True:
    print("I Love candy "+ str(number))
    number +=1
    if number == 7 :
        break


```
When we run this code

```bash
$ python3.6 example.py

I Love candy 0
I Love candy 1
I Love candy 2
I Love candy 3
I Love candy 4
I Love candy 5
I Love candy 6

```
The loop runs and prints out our statement but when `number` is equal to `7` the loop stops.

### Continue

The **`continue`** statement is also used in loops. It tells Python to ignore anything that comes under it, and jump back to the top of the loop.

```python
while True:
    print("Type password")
    password = input()

    if password != "password":
        continue
        print("Not correct")
    else:
        print("You printed password")
        break

```

This code will create a loop where we are prompted to type in the word `password`. Notice how the `print()` statement directly under the `continue` is not executed.
This is because every time continue is called it jumps back up to the top of the loop


---
### Lesson 9: [Python Lists and Dictionaries](./09_list_dict.md)
