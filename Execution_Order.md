Note:
- _ _ name _ _ has 2 underscores before and after "name"
- _ _ main _ _ has 2 underscores before and after "main"

Before executing code in a module (file), Python will define a few special variables
- If the Python interpreter is running the files as the main program, it sets the special _ name _ variable to have a value "_ main _"
- If the file is being imported from another module, _ name _ will be set to that module's (file's) name

To direct the Python interpreter when it first reads a file, add the following conditional (to the bottom) of your script:
- if _ name _ == " _ main _ ":
    
    main()
    
- This will run the main function, if the file is loaded as the main program


```python

```
