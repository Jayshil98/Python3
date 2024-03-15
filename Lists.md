# Lists:

(1) Type of data structures in Python

(2) Most common sequence

(3) Mutable

Syntax:
- list1 = ['1', 'dog', 'cat', 789]
    - Specify comma separated values in between square brackets []
    - Each items in list starts with index 0


```python
list1 = ['1', 'dog', 'cat', 789]
print(list1[1])
```

    dog
    


```python
print(list1[4])
```


    ---------------------------------------------------------------------------

    IndexError                                Traceback (most recent call last)

    <ipython-input-2-827113708aff> in <module>
    ----> 1 print(list1[4])
    

    IndexError: list index out of range



```python
list1.append("hello")
```


```python
print(list1)
```

    ['1', 'dog', 'cat', 789, 'hello']
    


```python
print(len(list1))
```

    5
    


```python
list1.pop()
```




    'hello'




```python
print(list1)
```

    ['1', 'dog', 'cat', 789]
    


```python
list1.insert(2, 'inserted item')
print(list1)
```

    ['1', 'dog', 'inserted item', 'cat', 789]
    

# Lists - More Operations:

(1) You can add lists

(2) You can multiply lists


```python
ls1 = [2, 3, 4]
ls2 = [7, 8, 9]
ls3 = ls1 + ls2
print("ls3 =", ls3)
```

    ls3 = [2, 3, 4, 7, 8, 9]
    


```python
#This creates a new list ls4 with the values of ls3 repeated three times
ls4 = ls3 * 3
print("ls4 =", ls4)
```

    ls4 = [2, 3, 4, 7, 8, 9, 2, 3, 4, 7, 8, 9, 2, 3, 4, 7, 8, 9]
    

# List Functions:


```python
ls1 = [2, 3, 4]
ls2 = [7, 8, 9]
```


```python
#Appends values of ls2 to the end of ls1
ls1.extend(ls2)
for l in ls1:
    print(l)
```

    2
    3
    4
    7
    8
    9
    

# Slicing Lists:

- You can get a slice of a list by using a colon (:)

- Format: [start_index:end_index]
    - start_index and end_index are both optional
    - start_index is the index of the first value (included in slice)
    - end_index is the index of the last value (not included in slice)


```python
my_list = ['b', 'a', 'm', 'n', 'a', 's']

#Gets the values from index 2 to index 4
print("Values from index 2 to index 4:", my_list[2:5], "\n") 

#Gets the value from index 4 to the last index in the list
print("Values from index 4:", my_list[4:], "\n") 

#Gets all elements
print("Values from element 1 till end:", my_list[:], "\n")

#Gets all elements for index 1 to index 3. Means index -4 is not included 
print("Values from index 1 to index 3:", my_list[:-4], "\n")

#true copy of my_list
copy_my_list = my_list[:]
print("Is copy_my_list is my_list:", copy_my_list is my_list, "\n")
print("Is copy_my_list == my_list:", copy_my_list == my_list)
```

    Values from index 2 to index 4: ['m', 'n', 'a'] 
    
    Values from index 4: ['a', 's'] 
    
    Values from element 1 till end: ['b', 'a', 'm', 'n', 'a', 's'] 
    
    Values from index 1 to index 3: ['b', 'a'] 
    
    Is copy_my_list is my_list: False 
    
    Is copy_my_list == my_list: True
    

# Updating Lists


```python
odd_numbers = [2, 4, 6, 8]

#update single element at index 0
odd_numbers[0] = 1
print("Updated list:",odd_numbers)

#update multiple elements with slice
odd_numbers[1:4] = [3, 5, 7]
print("Updated list after slicing:",odd_numbers)
```

    Updated list: [1, 4, 6, 8]
    Updated list after slicing: [1, 3, 5, 7]
    
