# Python

## Python Snippets

__using Counter from collections__  
```python
from collections import Counter

cnt = Counter(a)
print(cnt.most_common(3))
```

__Reverse a list__  
```python
a = [5, 4, 3, 2, 1]
print(a[::-1])
```

__Iterating over list contents in reverse efficiently__  
```python
for ele in reversed(a):
    print(ele)
```

__Sort a dictionary by its values with the built-in sorted() function and a 'key' argument.__  
```python
d = {'apple': 10, 'orange': 20, 'banana': 5, 'rotten tomate': 1}
print(sorted(d.items(), key=lambda x: x[1])
```

__Sort using operator.itemgetter as the sort key instead of a lambda__
```python
from operator import itemgetter

print(sorted(d.items(), key=itemgetter(1)))
```

__Sort dict keys by value__  
```python
print(sorted(d, key=d.get))
```

__converts list to comma separated string__
```python
items = ['foo', 'bar', 'xyz']
print(','.join(items))
```

__list of numbers to comma separated__
```python
numbers = [2, 3, 5, 10]
print(','.join(map(str, numbers)))
```

__list of mix data__
```python
data = [2, 'hello', 3, 3.4]
print(','.join(map(str, data)))
```

__merge dict's__  
```python
d1 = {'a': 1}
d2 = {'b': 2}

d1.update(d2)
```

__Remove duplicate items__
```python
from collections import OrderedDict

items = ['foo', 'bar', 'bar', 'foo']
print(list(OrderedDict.fromkeys(items).keys()))
```

## Pythonic Code Tips

__dictionaries for performance__:  
switch using lists to dictionaries

**\__slots\__:**  
use slots to save space in objects making them eliminate the underlying dict

__merge dicts__  
use **kwargs

__yield and generator methods__  
use yields to continously return results and keep the inner variables from generators

__lambda expressions__

__adding iteration to custom types__  
use \__iter\__ combined with yield in a custom type to iterate

__comprehensions and expressions__  
use comprehensions for lists, dicts and sets

__json back and forth__  
Use in files and web services  

__slicing__  
For collections and databases 

__yield + recursion__  
use 'yield from' to get the returned values from a function

__use string formatting with {}__  
inside de braces use indexes, dictionary keys

__keyword arguments__  
require the keyword arguments with * at the first param

## Notes


### PyCharm Visual Debugging

- Cython
- Use python console on execution in a breakpoint
- Check scope with 'self'
- iPython
- 'Annotate types' in debugger

### Documenting Python Code

- use docstrings (""") to describe functions  
- :<variable> to describe variables
- pydoc to generate documentation

