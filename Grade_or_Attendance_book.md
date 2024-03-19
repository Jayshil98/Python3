# Grade/Attendance Book

1) Here's a grade/attendance book for a teacher's students
- It contains a dictionary of dictionaries


```python
#Create a dictionary for each student
billy = {
    'name': 'Billy',
    'grades': [100, 80, 70, 100, 89],
    'attendance': [True, True, True, True, True]
}

sarah = {
    'name': 'Sarah',
    'grades': [0, 99, 0, 100, 0],
    'attendance': [True, False, True, False, True]
}

ben = {
    'name': 'Ben',
    'grades': [60, 82, 71, 92, 100],
    'attendance': [False, False, False, False, False]
}

#Add each student to a dictionary using a unique student ID
students = {'1': billy, '2': sarah, '3': ben}

#get number of students
print(len(students)) #number of keys
```

    3
    


```python
#get all student ids
print(students.keys()) #gets all keys in dict
```

    dict_keys(['1', '2', '3'])
    


```python
#Iterate over students
for k in students:
    print('key:', k)
```

    key: 1
    key: 2
    key: 3
    


```python
#get billy's attendance
billy = students['1']
print("Billy's attendance is:", billy['attendance'])
```

    Billy's attendance is: [True, True, True, True, True]
    


```python
#get sarah's grades
sarah = students.get('2')
print("Sarah's grades are:", sarah.get('grades'))
```

    Sarah's grades are: [0, 99, 0, 100, 0]
    


```python
#get all key:value pairs for ben
ben = students.get('3')
items = ben.items() #returns sequence of tuples

#Iterate over student dictionaries
for key, val in items:
    print(key, val)
```

    name Ben
    grades [60, 82, 71, 92, 100]
    attendance [False, False, False, False, False]
    


```python
#get average student grades for all assignments
grades = []
items = students.items() #key:value pair for students

for key, val in items:
    #Iterate over student lists of grades
    for g in val['grades']:
        grades.append(g)
        
#average grade
print('Average grade is:',round(sum(grades)/len(grades)))
```

    Average grade is: 70
    


```python
#another way for getting average student grades for all assignments
grades_concatenated = []
items = students.items() #key:value pairs for students

for key, val in items:
    grades_concatenated += val['grades'] #concatenate list of grades
    
#average grade
print('Average grade is:',round(sum(grades_concatenated)/len(grades_concatenated)))
```

    Average grade is: 70
    
