- Set a variable name to the value of your first name and last name
- Print the substring containing just your first name, without counting the letters in your first name
    - Hint: Use the built-in string index method to locate the space


```python
name = 'Jayshil Khajanchi'

#get index of single space between first name and last name
first_space = name.index(' ')

#get substring of name using slice
#first name only
print(name[0:first_space])
```

    Jayshil
    
