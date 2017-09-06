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
```
my_list = [1,2,3]
squared_list = [number*number for number in my_list] # squared_list = [1,4,9]
```
