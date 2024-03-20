# Reading A File

- You can use a stream to read lines from a file

    (1) read: Reads an entire file as a string
        - lines = stream.read() 
        #reads all text in the file
        
    (2) readline: Reads a file line by line. Each line is read as a string
        - line = stream.readline() 
        #reads one line in the file
        
    (3) readlines: Reads all lines in a file as a list. Each line in the list will be a string.
        - lines_lst = stream.readlines() 
        #reads all lines in the file as a list
        
    (4) With the above methods, you must remember to close the stream when you are done.
        - stream.close() 
        #closes the file object
        
        

# Reading a File - Newline Characters

- Lines that are read in from a file contain a newline \n character at the end


- You can use rstrip() to remove the \n at the end of lines you read in


- For eaxample, if using readline to read a single line of text


    - line = stream.readline()
      line.rstrip() #removes whitespace, including \n characters, at the end
      
- Or, if iterating over a stream directly


    - for line in open(file, "r"):
      line.rstrip() #removes whitespace, including \n characters, at the end
