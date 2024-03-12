Prompt the user for a numerical grade and print the appropriate letter grade
- Get user input of a numerical grade
- Convert the user input to an integer
- Test the range of the number using flow control

Get user input of a numerical grade


```python
grade = input("Enter your grade: ")
```

    Enter your grade: 85
    

Cast to an int


```python
grade = int(grade)
```

Test the range of the number and print the appropriate letter grade


```python
if grade >= 90:
    print('A')
elif grade >= 80:
    print('B')
elif grade >= 70:
    print('C')
elif grade >= 60:
    print('D')
else: 
    print('F')
```

    B
    


```python

```
