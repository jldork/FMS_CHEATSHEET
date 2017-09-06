# Sample code for Fundamentals of Modern Software

## User Input

For these two examples, let's ask the user for their social security number

### The input function
You can use the ```input()``` function built-into python. This will prompt the user at terminal to enter a number
```python
ssn = input('What is your social security number? ')

print("This is my ssn: ", ssn)
```
The corresponding terminal output
```
> python file.py
What is your social security number? 
```
To which you can enter a number that gets stored into the variable ```ssn```
```
> python file.py
What is your social security number? 123-45-6789
This is my ssn: 123-45-6789
```

### Passing system arguments
You can pass system arguments using the ```sys``` library. This expects you to pass an argument after the filename
```python
import sys

arguments = sys.argv

# arguments[0] should be 'file.py'
ssn = arguments[1] # should actually be the social security number

print("This is my ssn: ", ssn)
```
The corresponding terminal output
```
> python file.py 123-45-6789
This is my ssn: 123-45-6789
```
