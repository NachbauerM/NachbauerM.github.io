# Programming: Python_List comprehension

I try to do one cateogry (6 or 7) Kata on [Codwars](https://www.codewars.com/) to start a working day. For some reason doing this makes me a little more focused for the first "official" task and also it can be a very nice feeling of success early in the day.

Doing those easier Katas, I found that many high ranked solutions are using list comprehension. Apparently trying to write the whole function in one line makes up for an extra challenge. As a programming noob, using list comprehensions is not as intuitive as for loops. So, I noted down some interesting mechanis of list comprehensions.

## Identation in a for loop:
```python
multiplication_table = [[j*i for j in range(1,4)] for i in range(1,4)] 
#This creates lists inside a list, multiplying j(1-3) first with i = 1, then i=2 ... Like with indented for-loop.
multiplication_table
```

## Using a fucntion inside a list comprehension:
```python
def function(x: int)->int:
    return x**2 if x%2==0 else x

d = [function(x) for x in range(1,20) if x >=3]
d
```

## If/else statements in a list comprehension:
```python
s = "wwerhawhngaawejasdfjiasdfgwßehasudladhfasgfkwe"
x = "".join(["1" if x in ("a","e", "i", "o", "u") else "0" for x in s.lower()])
#In list comprehension the logic is sligthly different than usually: First what happens e.g. "1" 
#then the if and else statement. The join mehtod takes a iterable and joins it togehter.
x
```

## Get every second element of a list:
```python
l = [x for x in range(0,11)]
l[0::2]= [x*2 if x*2>10 else x*3 for x in l[0::2]]# changes every second element in the list
l[0::2],l
```

# The enumerate function: Enumerate thakes an iterable and returns tuple pairs (index, value). The index is not the index of the value in the iterable!!!
```python
for index, value in enumerate([x*2 for x in range(0,7)]):
    print(index, value)
```

# List and strings
```python
string = "Python"
list(string)
```
# Count similar items in a list with the count method.
```python
l = [x%2 for x in range(1,10)]
l, l.count(1)
```
