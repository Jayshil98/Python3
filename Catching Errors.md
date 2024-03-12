```python
number = input("Please input an integer.")
```

    Please input an integer.20.5
    

Try to cast the input


```python
try:
    number = int(number)
#Catch the raised exception if there is an error
except ValueError as e:
    print("Your input is not an integer.")
    print(e)
#Otherwise, there is no error
else:
    print(str(number) + "is indeed an integer!")
```

    Your input is not an integer.
    invalid literal for int() with base 10: '20.5'
    


```python
number = input("Please input an integer.")
```

    Please input an integer.20
    


```python
try:
    number = int(number)
#Catch the raised exception if there is an error
except ValueError as e:
    print("Your input is not an integer.")
    print(e)
#Otherwise, there is no error
else:
    print(str(number) + " is indeed an integer!")
```

    20 is indeed an integer!
    


```python

```
