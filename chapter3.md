# Chapter 3: Control flow

There are many constructs that help us write useful code

## Conditionals

Perform different operations depending on whether a condition is `True` or `False`

```python
x = 3
if x == 1:
    print('a')
elif x == 2:
    print('b')
else:
    print('c')
```

## Loops

`for` loops allow you to iterate for every element in some range

```python
for x in range(5):
    print(x)
```

`while` loops continue while the condition remains `True`

```python
x = 3
while (x > 0):
    x -= 1
```

loops can instantly terminate all future iterations with a `break` statement

```python
for i in range(1_000_000):
    if (i*3 == 27):
        print(f'27 divided by 3 is {i}')
        break                             # we have found our answer
                                          # we don't care about future iterations of i
```

loops can also instantly terminate just the current iteration with a `continue` statement

```python
for i in range(2, 10):
    if i % 2 == 1:    # skip all the odd numbers
        continue
    print(i // 2)
```

## Functions

Functions help us with avoiding duplicate code

```python
def complain():
    print('i dislike eggs')

complain()
complain()
```

They can return values to us

```python
def seven():
    return 7

x = seven()
```

We can also pass arguments to functions

```python
def average(x, y):
    return (x + y) / 2

x = average(3, 5)
```

Have as many `return`s as you want

```python
def coffee(amount):
    if amount < 5:
        return 'low'
    if amount < 10:
        return 'average'
    return 'high'
```

Return as many values as you want

```python
def party_pack():
    return 1, 1.0, 'beans', True

a, b, c, d = party_pack()
```

# Exercise 1

1. Asks the user to enter an integer.
2. Determines if the number is even or odd.
3. If the number is even, divides it by 2 and prints the result.
4. If the number is odd, multiplies it by 3 and adds 1, then prints the result.
5. Repeats steps 2-4 with the new number until the number is 1.

# Exercise 2

Write a function with one argument that returns True if the argument is even, and False if the argument is odd

# Exercise 3

Compute the sum of all numbers from 300 to 600
