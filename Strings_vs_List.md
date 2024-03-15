# Strings:
(1) A string is a sequence of characters

(2) A string is kind of like a list - just imagine a string as a list of characters!

(3) Unlike lists, strings are immutable, which means, once defined, you cannot change the individual elements (characters) of a string

(4) For example, if we have a list: my_menu_choices = ['burger', 'fries', 'coke']
- We can  get a single value: main_course = my_menu_choices[0]


```python
#here is a list containing menu choices
my_menu_choices = ['burger', 'fries', 'coke']

#you CAN get an item in the list using an index
main_course = my_menu_choices[0] 
print("First item in the list is:",main_course,"\n")

#you CAN update an item in the list using an index
my_menu_choices[0] = 'cheese burger'
print("Updated list is:",my_menu_choices)
```

    First item in the list is: burger 
    
    Updated list is: ['cheese burger', 'fries', 'coke']
    

- However, if we have a string: my_restaurant_choice = 'McDonalds'

- We can get a single value (character): my_restaurant_choice_third_letter = my_restaurant_choice[2]

- But we can't directly update a single value (character) - this won't work: You will get an error because strings are immutable


```python
#here is a string with my favorite restaurant
my_restaurant_choice = 'Mcdonalds'

#you CAN get a character in the string using an index
my_restaurant_choice_third_letter = my_restaurant_choice[2] 
print(my_restaurant_choice_third_letter) 

#you CANNOT update a character in the string using an index
#this won't work -- you'll get an error
my_restaurant_choice[2] = 'D'
print(my_restaurant_choice[2])
```

    d
    


    ---------------------------------------------------------------------------

    TypeError                                 Traceback (most recent call last)

    <ipython-input-2-9f6ff844a60e> in <module>
          8 #you CANNOT update a character in the string using an index
          9 #this won't work -- you'll get an error
    ---> 10 my_restaurant_choice[2] = 'D'
         11 print(my_restaurant_choice[2])
    

    TypeError: 'str' object does not support item assignment



```python

```
