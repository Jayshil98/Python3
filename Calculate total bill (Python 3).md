Define and set variables from user input (casted to a float)


```python
bill = float(input("How much is the meal?"))
tax = float(input("What is the sale tax (percentage)?"))
tip = float(input("How much of a tip (percentage)?"))
```

    How much is the meal?30
    What is the sale tax (percentage)?6
    How much of a tip (percentage)?18
    

Calculate and add tax


```python
#Calculate the tax
tax_amount = (bill * tax) / 100

#Add tax amount to final bill
total = bill + tax_amount
print(total)
```

    31.8
    

Calculate and add tip


```python
#Calculate the tip
tip_amount = (total * tip) / 100

#Add tip amount to the final bill
total = total + tip_amount
```

Round the total to 2 decimal places


```python
total = round(total, 2)
```

Print the final amount


```python
print("The total bill is $", total, sep = '')
```

    The total bill is $37.52
    


```python

```
