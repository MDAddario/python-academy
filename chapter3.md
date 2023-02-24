# Chapter 3: Control flow

There are many constructs that help us write useful code. We first have conditionals

```python
x = 3
if (x == 1):
    print('a')
elif (x == 2):
    print('b')
else:
    print('c')
```

Then we also have loops

```python
x = 5
while (x > 0):
    print(x)
    x -= 1

for x in range(5):
    print(x)
```

And very importantly, we have functions

```python
def add_seven(x):
    return x + 7
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
