## Lists

Lists are an array of objects or numbers or strings that are indexed starting at 0
```python
my_list = [1,2,3,4, "five"]

# Index
my_list[0] # This will return 1

# Index
my_list[4] # This will return "five"
```
You add items to a list using the ```.append()``` function
```python
my_list.append('six')
my_list # This will return [1,2,3,4,'five', 'six']
```
which is actually the same as
```python
my_list = my_list + ['six']
my_list # This will return [1,2,3,4,'five', 'six']
```

## For loop
A for loop takes a list, and performs an action over each item in that list  
```python
my_list = [1,2,3]

for number in my_list:
    print("My number: ", number)
    print("number^2: ", number*number)
    print("")
```
This prints an output that says
```
My number: 1
number^2: 1

My number: 2
number^2: 4

My number: 3
number^2: 9
```

You can also build new lists using a for loop. This is called **list comprehension**
```python
my_list = [1,2,3]
squared_list = [number*number for number in my_list] # squared_list = [1,4,9]
```
## While Loops

A while loop keeps checking to see if a condition is met. If the condition is not met, then the code under the while loop doesn't get executed.
```python
while 1 == 1: 
    print("Hi") # This will never stop running. Because 1 equals 1
```
another example
```python
while 1 == 2: 
    print("Bye") # This will not run. 1 == 2 evaluates to False
```
Now for a realistic example:
```python
my_age = 26
while my_age < 30:
   my_age = my_age + 1 
  
print("my age!: ", my_age)
```
Here, the first time we hit this while loop. 
1. Is 26 less than 30?
2. We update my_age to 27 (26 + 1). 
3. Then we check if 27 is less than 30
4. Then we update my_age to 28
5. Then we check if 28 is less than 30
etc. etc.
6. We finally print "my age!: 30"
