# Dictionaries and Files

1) Dictionaries:
- Stores multiple attributes about a single thing

2) Files:
- Can be loaded by python

# Dictionary (Part - 1):

1) A dictionary (dict) is another way to store data, like a list or set, but as unordered key-value pairs

2) A dictionary is a set of keys and corresponding values.
- Dictionaries are also known as hashmaps or associative arrays in other languages (e.g. Java)

3) Dictionaries are extremely useful!
- One use case is for toring several attributes (or data points) about a single thing

4) To create a dict, use comma separated key:value pairs, in between curly braces{}
- keys are simple data types (usually strings or ints)
- values can be of any type

5) Dictionaries are mutable, so once defined, elements can be changed

# Dictionaries (Part - 2)


```python
#Here's a dict with some keys and associated values about a person
person = {'name' : 'Jayshil', 'age' : 26, 'height': 6 * 12 + 2}

#A dictionary has a data type of dict
print(type(person))
```

    <class 'dict'>
    


```python
#We can get the value of a given key by using brackets[]
print(person['name'])
```

    Jayshil
    


```python
#Or, we can use the built-in dict get method
print(person.get('name'))
```

    Jayshil
    


```python
#The get function is good to use, in case the key doesn't exist

#KeyError will be generated if 'state' doesn't exist
print(person['state'])
```


    ---------------------------------------------------------------------------

    KeyError                                  Traceback (most recent call last)

    <ipython-input-4-9cf558e90bc0> in <module>
          2 
          3 #KeyError will be generated if 'state' doesn't exist
    ----> 4 print(person['state'])
    

    KeyError: 'state'



```python
#this will return None (a null value) if 'state' doesn't exist
print(person.get('state'))
```

    None
    


```python
#this will return a default 'PA' if 'state' doesn't exist
print(person.get('state', 'PA'))
```

    PA
    

# Updating a dictionary


```python
# Dictionaries are mutable, so elements can be updated or added

#update value with key 'name'
person['name'] = "John"

#increment value with key 'age'
person['age'] += 1

#add value with key 'college'
person['college'] = True

#add value with key 'city'
person['city'] = "Chicago"

print(person)
```

    {'name': 'John', 'age': 27, 'height': 74, 'college': True, 'city': 'Chicago'}
    


```python
# Check if a key exists in a dictionary
print('college' in person) 
```

    True
    


```python
# Delete elements using the del keyword
del person['college']
print(person)
```

    {'name': 'John', 'age': 27, 'height': 74, 'city': 'Chicago'}
    


```python
# Dictionaries can include other dictionaries or list as values
person['siblings'] = ['James']
person['siblings'].append('Anderson')
print(person)
```

    {'name': 'John', 'age': 27, 'height': 74, 'city': 'Chicago', 'siblings': ['James', 'Anderson']}
    


```python
# Or, we can add the key:value pairs from one dictionary to another using the built-in dictionary update method
person_attributes = {'marital status': 'single', 'children': 0}
person.update(person_attributes)
print(person)
```

    {'name': 'John', 'age': 27, 'height': 74, 'city': 'Chicago', 'siblings': ['James', 'Anderson'], 'marital status': 'single', 'children': 0}
    
