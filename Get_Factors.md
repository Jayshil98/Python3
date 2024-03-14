Define a function get_factors that takes an integer as a parameter and returns a list of factors of that number
- Basically, find the numbers between 1 and the given integer that divide the number evenly


```python
def get_factors(x):
    """Returns a list of factors of given number x."""
    
    factors = []
    
    #iterate over range from 1 to number x
    for i in range(1, x + 1):
        #check if i divide number x evenly
        if (x % i == 0):
            factors.append(i)
            
    return factors

print(get_factors(21))
```

    [1, 3, 7, 21]
    


```python
print(get_factors(256))
```

    [1, 2, 4, 8, 16, 32, 64, 128, 256]
    


```python

```
