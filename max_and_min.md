# Tuples - Exercise

- Create a max_and_min function that returns a tuple containing the max and min of a given list


- First, create the max_and_min funtion itself


```python
def max_and_min(lst):
    """Returns max and min of given list."""
    
    #return tuple containing max and min of list
    return (max(lst), min(lst))

def main():
    list1 = [10, -1, -34, 56]
    maxandmin = max_and_min(list1)
    
    #first, take a look at the type
    print(type(maxandmin))
    
    #get max from tuple
    max = maxandmin[0]
    
    #get min from tuple
    min = maxandmin[1]
    
    print(max,',',min)
    
if __name__ == '__main__':
    main()
```

    <class 'tuple'>
    56 , -34
    

Another way to do this:


```python
def max_and_min(lst):
    """Returns max and min of given list."""
    
    #return tuple containing max and min of list
    return (max(lst), min(lst))

def main():
    list1 = [10, -1, -34, 56]
    maxandmin = max_and_min(list1)
    
    #first, take a look at the type
    print(type(maxandmin))
    
    #double variable assignment, to get tuple values directly
    maxv2, minv2 = max_and_min(list1)
    print("Maximum value in the list is:", maxv2,'\n',"Minimum value in the list is:", minv2)
    
if __name__ == '__main__':
    main()
```

    <class 'tuple'>
    Maximum value in the list is: 56 
     Minimum value in the list is: -34
    
