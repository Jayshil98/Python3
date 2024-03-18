# Tuple

- An immutable sequence of values
- Unlike lists, which are mutable
- Values included do not need to be all of the same type


```python
direction = ('north', 'south', 'east', 'west')
print(type(direction)) #<class 'tuple'>
```

    <class 'tuple'>
    


```python
possible_grades = 'A', 'B', 'C', 'D', 'E'
print(type(possible_grades))
```

    <class 'tuple'>
    


```python
grades = tuple('ABCDE')
print(type(grades))
```

    <class 'tuple'>
    
