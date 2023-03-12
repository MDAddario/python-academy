# Chapter 4: Data structures

Variables are great, but when we want to handle lots of data, it can be more convenient to use data structures

```python
x = [1, 2, 3, 4]
y = {'a': True, 'b': False}
```

## Lists

Use lists to store sequences of data

```python
x = []                  # empty list
y = [1]                 # list with one entry
z = [1, True, 'bacon']  # list with multiple data types
```

Access specific elements with indices

```python
x = ['a', 'b', 'c']
y = x[0]             # y == 'a', begins at zero
z = x[1]             # z == 'b', increments by one
w = x[-1]            # w == 'c', can index backwards also
```

Lists can be dynamically populated

```python
x = list()         # x == []
x.append(1)        # x == [1]
x.extend([2, 3])   # x == [1, 2, 3]
```

They also pair nicely with for loops

```python
cars = ['benz', 'audi', 'honda']

for car in cars:
    print(car)             # 'benz', 'audi', 'honda'

for car in sorted(cars):
    print(car)             # 'audi', 'benz', 'honda'

for car in reversed(cars):
    print(car)             # 'honda', 'audi', 'benz'
```

If statements check for non-emptyness

```python
x = []
if x:
    print('there is at least one element in your list')
else:
    print('your list is empty')
```

## Dictionaries

Use dictionaries to store data you organize by a `str` key

```python
x = {}                             # empty dict
x = {'name': 'Charlie'}            # dict with one entry
x = {'age': 24, 'married': False}  # dict with multiple data types
```

Access specific elements with `str` keys

```python
x = {'name': 'Carl', 'age': 7}
y = x['age']                    # y == 7
z = 'name'
w = x[z]                        # w == 'Carl'
```

Dictionaries can be dynamically populated

```python
x = dict()            # x == {}
x['food'] = 'burger'  # x == {'food': 'burger'}
x['sauce'] = False    # x == {'food': 'burger', 'sauce': False}
```

They also pair nicely with for loops

```python
x = {'Carl': 68, 'Reginald': 47, 'Ben': -4}

for (key, value) in x.items():
    print(key, value)          # ('Carl', 68), ('Reginald', 47), ('Ben', -4)

for key in x.keys():
    print(key)                 # 'Carl', 'Reginald', 'Ben'

for value in x.values():
    print(value)               # 68, 47, -4
```

If statements check for non-emptyness

```python
x = {}
if x:
    print('there is at least one (key, value) pair in your dict')
else:
    print('your dict is empty')
```
___

## Exercise 1

Using lists, create a program that accepts inputs from the user until the user types `'stop'`. After stopping, print out the entire history of what the user has typed.

## Exercise 2

Using lists, create a program that accepts inputs from the user until the user types `'stop'`. After stopping, print out the entire history of what the user has typed, in reverse order.

## Exercise 3

Using the following list:

```python
x = [13, 5, 3, 49, 6, 17]
```

Compute (a) the average of all the integers, (b) the difference between the largest and the smallest integers, and (c) the difference between the first and the last integers.

## Exercise 4

Using the following list:

```python
x = [13, -5, 14, -6, -7, 31, -42]
```

Create two new lists that contain only the positive integers and only the negative integers from the list `x`.

## Exercise 5

Using the following dict:

```python
test_scores = {'Alex': 72, 'Michael': 100, 'Jake': 98, 'Daniel': 26}
```

Create a program that accepts an input name from the user, and prints out the test score that that student has received.

## Exercise 6

Using the following dict:

```python
test_scores = {'Alex': -72, 'Michael': 100, 'Jake': -98, 'Daniel': 26}
```

You see that some test scores are wrongly reported. Given you know that the numbers are correct, and that the sign simply needs to be flipped, correct all negative test scores in the above dict.

## Exercise 7

Using the following dict:

```python
test_scores = {'Alex': 72, 'Michael': 100, 'Jake': 98, 'Daniel': 26}
```

Create a program that accepts an input name from the user, and prints out whether the name is present in the above dictionary.

## Exercise 8

Using the following dict:

```python
test_scores = {'Alex': -72, 'Michael': 100, 'Jake': -98, 'Daniel': 26}
```

Create two new dictionaries that contain only positive test scores and only negative test scores from `test_scores`.

## Exercise 9

Using the following list of dicts:

```python
friends = [
    {'name': 'Michael', 'age': 38, 'car': 'Tesla', 'married': False},
    {'name': 'Jake',    'age': 32, 'car': 'Audi',  'married': True},
    {'name': 'Alex',    'age': 24, 'car': 'Jeep',  'married': True},
    {'name': 'Daniel',  'age': 67, 'car': 'Tesla', 'married': True},
]
```

Determine (a) the average age of the married men, (b) how many men own `Tesla`s, (c) how many married men own `Tesla`s.

## Exercise 10

Using the following dict of lists:

```python
stock_prices = {
    'Tesla': [98, 99, 110, 30],
    'Apple': [70, 80, 90, 100],
    'Meta':  [30, 20, 80, 90],
}
```

Determine (a) what stock grew the most from start to finish, (b) what stock had the greatest average stock price, (c) how many stocks never went past a value of 99.
