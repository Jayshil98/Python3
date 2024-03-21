# Open and Read A file

- Create an open_read_file function that opens a given file, reads each line and prints it to the console
    - def open_read_file(file)
    
    
- For this you need to create a .txt file 


```python
def open_read_file(file):
    """Opens the given file, reads each line and prints to the console.
    Closes the given file."""
    
    #open the given file in read mode
    f = open(file, "r")
    print('The type of the stream f is:', type(f), '\n') #print the type of the stream f
    
    cnt = 0
    
    # reads and prints each lines in f, while there is a line to read
    line = f.readline()
    while line:
        print(line, end='')
        line = f.readline()
        
        cnt += 1
        
    print('', '\n')
    print('There are', cnt, 'lines in the file')
    
    f.close()
    
def main():
    open_read_file('news.txt') 
    
if __name__ == '__main__':
    main()
```

    The type of the stream f is: <class '_io.TextIOWrapper'> 
    
    News Anchoring Script Sample 1
    
    INTRO: "Good Evening, I'm Mike and this is Python 3 Programming. We're coming to you from USA. Today is 3/21/2024. Our top TOPICS tonight are..."
    
    TOP STORY: "First, to our headline story. There's a major development in the regional infrastructure project. Officials announced today that the construction of the new highway, considered a vital lifeline for the community, is set to begin next month -- two months ahead of the original schedule. Michelle is on location with the details. Over to you, Michelle." 
    
    There are 5 lines in the file
    
