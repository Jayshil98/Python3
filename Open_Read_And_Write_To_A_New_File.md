# Open, Read, and Write to New File

- Create an open_read_write_new_file function that copies the text in one file to another file

def open_read_write_new_file(file1, file2):


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
    
def open_read_append_new_file(file1, file2):
    """Opens the first file, and reads all lines into a list.
    Reverses the lines, and appends them to the second file."""
    
    #open the first file in read mode
    with open(file1) as fin:
        
        #read all lines into a list
        lst = fin.readlines()
        
        #reverses the list
        lst.reverse()
        
        #open second file for appending
        fout = open(file2, "a")
        
        #write reversed lines to second file
        fout.writelines(lst)
        
        #close the second file
        fout.close()
        
def open_read_append_same_file(file):
    """Open the given file and reads all lines as a list.
    Appends lines to same file"""
    
    #open the file for reading and writing
    f = open(file, "r+")
    
    #read all lines into a list
    lst = f.readlines()
    
    #updating list for appending back to same file
    lst.insert(0, '\n')
    lst.insert(0, 'Here is some new text')
    lst.insert(0, '\n')
    
    #append the lines back to same file
    f.writelines(lst)
    
    #close file
    f.close()
    
def open_read_write_new_file(file1, file2):
    """Open the given file and reads all text as a string.
    Copies or writes all text to the second file."""
    
    with open(file1) as fin:
        
        #reads all lines as a single string
        text = fin.read()
        
        #opens second file to write mode
        fout = open(file2, 'w')
        
        #write single string to second file
        fout.write(text)
        
        #close second file
        fout.close()
    
def main():
    #open_read_file('news.txt') 
    #open_read_append_new_file('news.txt', 'news_out.txt')
    #open_read_append_same_file('news.txt')
    open_read_write_new_file('news.txt','news_copy.txt')
    
if __name__ == '__main__':
    main()
```
