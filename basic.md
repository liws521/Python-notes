# compared with C
- comments, # or """

## data type
- the integer in Python can be any value, so there is only "int" type that can indicate integer in Python3
    - the octal num in Python is 0o123 while o123 in C
- the string in Python is enclosed by ' or "
- the value of bool type in Python is only True or False, which is same as Golang

- type(a) can get the type of a
- type conversion: int(), float(), str(), chr(), ord()
- using `and or not` instead of `&& || !`
- code block using indentation but not `{}`

## control flow statement
```python
# if statement
if cond1:
    statement1
elif cond2:
    statement2
else
    statement3

# for-in statement
for x in range(2, 101, 2):
    sum += x
# range(begin, end, step), [begin, end)
# the default value of begin is 0 and that of step is 1, so range(101) gets the integers in [0, 101)
# step can less than zero

# while statement
while cond1:
    if cond2:
            break
    if cond3:
            continue
    statement 
```
## widely used data structure
### list
- the data type of values in list can be defferent, even can be another list
```python
mylist = [1, 2, 3]
for v in mylist:
    sum += v

mylist.append(value)
mylist.insert(index, value)
mylist.remove(value) # delete by value, if value is not in mylist, a ValueError exception will be get
mylist.pop(index) # delete by index, if index >= len(mylist), a IndexError exception will be get
del mylist[index]
mylist.clear()
mylist.index(value, [times]) # find the index of "times"-th value
mylist.count(value) # count the times of value
mylist.sort()
mylist.reverse()
mylist2 = [x for x in range(1, 10)]
mylist3 = [x + y for x in 'ABC' for y in '12']
```

# function
```python
# default value is permitted
def add(a=0, b=0):
    return a + b

# variable arguments is allowed
def add2(*args):
    sum = 0
    for v in args:
        sum += v
    return sum
```

# module
- every module has a latent variable '__name__`, if a module is executed by Python interpreter, the name of this module will be '__main__'
```python
from module1 import func1
from module2 import func1
func1() # this func1 is in module2

# or you can use it in this way
import module2 as m2
m2.func2()

if __name__ == '__main__':
    statements
```

- [visualize](https://pythontutor.com/visualize.html#mode=edit)