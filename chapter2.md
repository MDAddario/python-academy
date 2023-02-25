# Chapter 2: Operators and logic

Operators take two inputs and return a single output. The behaviour of operators depends on what data types you are using.

```python
1 + 2                # 3
2.3 + 3.6            # 5.9
'bacon ' + 'cheese'  # 'bacon cheese'
```

`str`s are just weird

```python
'h' + 'j'   # 'hj'
'h' * 4     # 'hhhh'
'h' == 'j'  # false
```

`int`s and `float`s can use arithmetic operators

```python
1 + 2
3 - 4
5 * 6
7 / 8
9 // 10
11 % 12
```

`int`s and `float`s can also use comparison operators

```python
1 < 2
3 <= 4
5 > 6
7 >= 8
9 == 10
11 != 12
```

there is a cute syntax for operations where a variable updates itself

```python
x, y, z = 0, 0, 0

x = x + 2
x += 2

y = y * 2
y *= 2

z = z // 2
z //= 2 
```

`bool`s can use logical operators

```python
True and False
True or False
not True
```

Use brackets when you are unsure of the **order of operations**

```python
( (not True) and (not False) ) and False
```

# Exercise 1

We are going to use the magic number 42. Write a program that accepts an integer input from the user, and tells the user whether their number is below, above, or equal to the magic number.

# Exercise 2

Write a program that accepts two float inputs from the user. If at least one input is greater than 13.0, print 'cash money'. If both inputs are less than 5.0, print 'recession'. 