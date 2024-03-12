Write a program that asks the user for numbers(ints). It computes the average of the numbers. Allows the user to enter -1 to quit the program.


```python
num_list = []
i = 0
playing = True

while(playing == True):
    num = int(input("Enter an int: "))
    
    #test if number is -1, to quit the program
    if (num == -1):
        playing = False
    else:
        #add number to list of numbers
        num_list.append(num)
        i += 1

#get the sum of all entered numbers
num_sum = 0
for num in num_list:
    num_sum += num
    
#calculate the average
num_avg = num_sum / i

print("avg:", num_avg)
    
```

    Enter an int: 3
    Enter an int: 3
    Enter an int: 3
    Enter an int: -1
    avg: 3.0
    


```python
num_list = []
i = 0
playing = True

while(playing == True):
    num = int(input("Enter an int: "))
    
    #test if number is -1, to quit the program
    if (num == -1):
        playing = False
    else:
        #add number to list of numbers
        num_list.append(num)
        i += 1

#get the sum of all entered numbers
num_sum = 0
for num in num_list:
    num_sum += num
    
#calculate the average
num_avg = num_sum / i

print("avg:", num_avg)

```

    Enter an int: 1
    Enter an int: 2
    Enter an int: 3
    Enter an int: -1
    avg: 2.0
    


```python

```
