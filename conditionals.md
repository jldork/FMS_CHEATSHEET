## Booleans

Boolean is a fancy term for True or False. ```1 == 1``` is a boolean (True). ```2==1``` is a boolean. If statements use these booleans to figure out what code to run.

```python
is_the_world_sane = (1 + 1 == 2)
print(is_the_world_sane) # prints True

print(not is_the_world_sane) # prints False, because we put "not" in front of the boolean

age = 26
i_am_older_than_30 = age > 30
print(i_am_older_than_30) # prints False
```
You can even combine booleans using ```and``` or ```or```
```
print(is_the_world_sane and i_am_older_than_30) # True and False should return False!
```

## If statements
If statements let you define sections of code to run based on certain conditions
```
if not is_the_world_sane:
    print("1 + 1 does NOT equal 2! Leave!!")
elif i_am_older_than_30: # run only if the first part is false and this is true
    print("The world is sane, but i'm older than 30 - about to hit my midlife crisis")
else: # else does not require a condition
    print("I can enjoy my youth")
```
They can be more complicated if you combine booleans
```
if not i_am_older_than_30 and is_the_world_sane: # True and True evalutes to True
    print("I can enjoy my youth")
```

