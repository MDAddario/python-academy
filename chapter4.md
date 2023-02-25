# Chapter 4: Data structures

Working with variables is fine, but we need data structures to deal with multiple variable situations

```python
x = [1, 2, 3, 4]
y = {'a': True, 'b': False}
```

## Lists

Use lists to store sequences of data

```python
x = []                  # empty list, can also use list()
y = [1]                 # list with a single entry
z = [1, True, 'bacon']  # lists can hold all data types
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
cars = ['audi', 'benz', 'honda']

for car in cars:
    print(car)

for car in cars.sort:
    print(car)

for car in cars.reverse:
    print(car)
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
x = {}                             # empty dict, can also use dict()
x = {'name': 'Charlie'}            # dict with a single entry
x = {'age': 24, 'married': False}  # dicts can hold all data types
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
    print(key, value)

for key in x.keys():
    print(key)

for value in x.values():
    print(value)
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