# Sets
- A set is an unordered collection 
    - The order doesn't matter and can't be specified
    - It does not support things like indexing
    
    
- A set does not allow repeated eleements
- Values included do not need to be all of the same type
- Sets are mutable, so once defined, elements can be changed

To create a set, create a list of comma-separated values within curly braces{}


```python
fruit = {'apple', 'orange', 'apple', 'pear', 'orange', 'banana'}
print("type is:",type(fruit))
print("set of fruits are:",fruit)
```

    type is: <class 'set'>
    set of fruits are: {'apple', 'orange', 'pear', 'banana'}
    

You can also create a set from a string or from a list using Python's built-in set function


```python
a = 'abracadabra'
a_set = set(a) #unique letters in string a
print(a_set)
```

    {'d', 'b', 'c', 'a', 'r'}
    


```python
b = [1, 2, 1, 3, 4, 5, 5, 6, 2, 7, 8, 10]
b_set = set(b) #unique numbers in list b
print(b_set)
```

    {1, 2, 3, 4, 5, 6, 7, 8, 10}
    

Note, an empty set cannot be written as {}
- Instead, use the set funtion
    - empty_set = set()

Iterating over and updating a set


```python
#You can iterate over a set to get the values

a = 'abracadabra'
a_set = set(a) #unique letters in string a

b = [1, 2, 1, 3, 4, 5, 5, 6, 2, 7, 8, 10]
b_set = set(b) #unique numbers in list b

for c in a_set:
    print(c, end='')
    
for n in b_set:
    print(n, end='')
```

    dbcar1234567810


```python
#Add an element to a set
a_set.add('c')
print(a_set)
```

    {'d', 'b', 'c', 'a', 'r'}
    


```python
#Remove an element from a set
b_set.remove(10)
print(b_set)
```

    {1, 2, 3, 4, 5, 6, 7, 8}
    
