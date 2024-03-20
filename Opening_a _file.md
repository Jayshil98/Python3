# Opening a File

- For opening a file in python, we do 3 things:

1) Open the file

2) Use the file means read, write and append to the file

3) Close the file

# For opening a file:

- open(path_to_file, mode)


    - path_to_file:
    

        - Name or path to file
        

    - mode:
    

        - 'r' to read the file
        

        - 'w' to write to the file
        

        - 'a' to append to the end of the file
        

        - 'r+' to read and write to the file at the same time

# Basics of the File Open Method Modes

(1) "r": Read Mode (Default)

    - Opens a file for reading
    
    - Returns an error if the file doesn't exist


```python
# Format: open(<my_file> , 'r')
#Note: This is the default mode, so, you can leave out the optional 'r' like so: open(<my_file>)
```

(2) "w": Write Mode

    - Opens a file for writing
    
    - Removes all old data if the file already exists


```python
# Format: open(<my_file>, 'w')
```

(3) "a": Append Mode

    - Opens a file for appending
    
    - Creates the file if it doesn't exist


```python
# Format: open(<my_file>, 'a')
```

(4) "r+": Read/Write Mode

    - Opens a file for reading and writing at the same time
    
    - Returns an error if the file doesn't exist
    
    - Does not remove old data from the file


```python
# Format: open(<my_file>, 'r+')
```
