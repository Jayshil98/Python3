# Writing to a File

- Writing Streams

(1) stream.write(string)
    - Writes a single string to a file

(2) stream.writelines(list_of_strings)
    - Writes a list of strings to a file

(3) stream.close()
    - Close the stream when you are done

# Closing a File

- You should always close a file when you are done using it
    - You can't open it again until it has been closed
    - If you were writing to it, an unclosed file may be incomplete
    
    
- If you don't explicitly close a file, the computer's operating system SHOULD close the file for you, but IT'S NOT GUARANTEED
    - To be safe, close your files!


```python
#Here's one way to close a file

#opens the file and stores file object as stream
#stream = open(<my_file>, 'w') 

#closes the file object
#stream.close()
```


```python
#Here's another way to close a file using a with statement

#opens the file and stores file object as stream
#with open(<my_file>, 'w') as stream:

#with will automatically close the file for you after the statements have been executed
```
