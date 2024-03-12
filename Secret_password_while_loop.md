Secret Password:
- Write a program that uses a while loop to test user input of a secret password. 
- If the user inputs "secret", print "Welcome!" and exit the program. 
- Otherwise, print "Sorry, the password you entered is incorrect.Please try again" and prompt the user again.


```python
password = ""
while password != 'secret':
    password = input('Please enter the password:')
    if password == 'secret':
        print("Welcome!")
    else:
        print("Sorry, Entered password is incorrect. Please try again!!!!")
```

    Please enter the password:Secret
    Sorry, Entered password is incorrect. Please try again!!!!
    Please enter the password:secret
    Welcome!
    


```python

```
