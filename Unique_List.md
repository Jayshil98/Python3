Define a function unique_list that takes a list of numbers as a parameter and returns a new list with unique values
- Create a new empty list
- Use a for loop to iterate over the provided list of numbers 
- Add values to the new list if they don't already exist in the new list
- Return the new list!


```python
def unique_list(l):
    """Returns a list of unique values from given list l."""
    
    x = []
    
    #iterate over provided list
    for a in l:
        #check if number is in new list
        if a not in x:
            #add it to new list
            x.append(a)
            
    return x

print(unique_list([1,2,3,3,4,4,5,5,6,6,8,9,10]))
```

    [1, 2, 3, 4, 5, 6, 8, 9, 10]
    


```python

```
