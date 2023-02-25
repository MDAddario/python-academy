# Chapter 1: Data types and variables

There are four basic data types in Python

```python
x = 1       # int   -> whole numbers
y = 3.14    # float -> decimal numbers
z = 'bacon' # str   -> text
w = True    # bool  -> true or false
```

You can **cast** variables to convert from one data type to another, when sensible

```python
x = int('3')     # x = 3     (type = int)
y = float('3.5') # y = 3.5   (type = float)
z = str(3.5)     # z = '3.5' (type = str)
w = int('bacon') # ERROR: this doesn't make sense
```

Variables can be also used to set other variables

```python
x = 3
y = x
print(y) # 3
```

When using one of the 4 basic data types, changing one variable will never change another variable

```python
x = 3
y = x
x = 5
print(x) # 5
print(y) # 3
```
Here are two functions that are very useful to know

```python
x = input('Give me content: ') # Read user input
print(x)                       # Display output

type() # me too!!
```

Please note that `input()` will always return a `str`

```python
when_you_have = 3
long_variable_names = 4
you_should_name = 5
them_like_this = 6
```

# Exercise 1

Write a program that asks the user for input and then prints out `Simon says: [x]`, where `[x]` is the input that the user typed.

```
bacon cheese
Simon says: bacon cheese
```

# Exercise 2

Write a program that asks the user for an integer and then prints out `The magic number is [x]`, where `[x]` is the number that the user typed plus 5.

```
7
The magic number is 12
```
