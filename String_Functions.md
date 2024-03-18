# String Functions:

- Here are some useful built-in string methods:

1) string.capitalize() – capitalizes first letter of string

2) string.startswith(prefix) – determines if string starts with prefix 

3) string.endswith(suffix) – determines if string ends with suffix 

4) string.isupper() – determines if all characters in the string are uppercase 

5) string.islower() – determines if all characters in the string are lowercase 

6) string.find(str) – determines if str occurs in string

7) string.index(str) – determines index of str in string

8) string.replace(old, new) – replaces all occurrences of old in string with new

9) string.strip() – trims whitespace from beginning and end of string

10) string.upper() - returns uppercased string from given string 

11) string.lower() - returns lowercased string from given string

# split() function:
- split is a useful string method used to split a single string into a list of multiple strings


```python
colors = 'blue,red,green'
colors_list = colors.split(',') #splits string into list of strings using comma separator
print(colors_list)
print(colors_list[2])
```

    ['blue', 'red', 'green']
    green
    

# join() function:
- join creates a single string from a list of multiple strings


```python
separator = ','
new_colors = separator.join(colors_list) #joins list of strings using separator value
print(new_colors)
```

    blue,red,green
    


```python
#here is a string with my favorite restaurant
my_restaurant_choice = 'Mcdonalds'

#convert the string to a list
my_restaurant_choice_list = list(my_restaurant_choice)
#update the third item in the list
my_restaurant_choice_list[2] = 'D'
#covert the list back to a string
my_restaurant_choice = ''.join(my_restaurant_choice_list)

print(my_restaurant_choice)
```

    McDonalds
    
