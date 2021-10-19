# Py1 Overview  
  
### Introdution  
 - Python - 가독성, 간단성, 확장성

### Run OS or magic commands in code cell
 - current folder name (present working directory) - %pwd (pwd, !pwd)
 - list of files in the current folder = %ls, !dir (!ls)
 - contents of a file - !type <filename> (!cat <filename>)

### Run Python code
 - Arithmetic
 - variables (or names)
 - input()
 - List (indexing, slicing, sort)
 - set
 - reading a web page
   > requests.get()
 - Read a remote file and process the text 
   > from urllib.request import urlopen
 - count()
 - Function (def:)
 - import matplotlib.pyplot as plt (plt.plot(x,y), plt.show())
 - import numpy as np (np.arange(start, stop, step)
  > np.cos(), np.sin()
 - from matplotlib.image import imread (img=imread(), plt.imshow(img))
 - Class and Object(instance) (class Person(object):, def __init--(self, var))
 - %%writefile mycode.py
 - %load mycode.py
 - Shell  
 ![image](https://user-images.githubusercontent.com/68910144/137792855-26354613-9ec9-4c0b-9a27-41c59c29ef67.png)  
 ![image](https://user-images.githubusercontent.com/68910144/137792930-7beb52fa-e6a8-4b63-afdb-d96085ce7c8f.png)  

 
 ---
 
# Py2 DataTypes

### Revisit cell magic commands  
 ![image](https://user-images.githubusercontent.com/68910144/137795189-eec22e42-798c-45db-b6e8-88c595ca2be8.png)  
 ![image](https://user-images.githubusercontent.com/68910144/137795221-5852c718-a3ba-494e-9ad8-8564ca407dd5.png)  

#DataTypes and Operarions
 - int
 - float
 - str
 - bool
 - complex
   
 - list
 - tuple
 - dict
 - set
 - range
 
 ### int
 - 제곱 **
 - there is no longer a limit to the value of integers
 
 ### casting
 - int()
 - float()
 - str()
 
 ### float
 - truncate (round), close to zero
 
 ### string
 - ' '
 - " \n"
 - """ """ (can multiple line)
  > print("Hello", "World") Have Blank
  > print("Hello" + "World") No Blank
 - outside single-quote, inside double-quote (changeable)
 
 ### Strings and Arrays
 - Start is 0 in array
 - last is -1  and len(list)-1 in array
 - slicing (not include stop)
 
 ### Arithmetic Operations
 - ( )
 - **
 - *
 - /
 - // (몫)
 - %
 - +, -
 
 ### Simple Math Functions
 - abs() (절댓값)
 - round() (반올림)
 - max( , key=?) (reutrn max-value)
 - min( , key=?) (return min-value)
 
 ### bool
 - operators (or, and, not)
 - using chained comparison
 - print(5<10 or xxx>20) short-circuit evalution
 - Name error, Type error, True, False
 
 ### Range is a special object in Python
 - range(start, stop, step) stop is not include
 
 
 input() -> string
 len() and indexing  
 ![image](https://user-images.githubusercontent.com/68910144/137809012-d2af93a8-1283-4f0e-bc92-f37149579046.png)  
 ![image](https://user-images.githubusercontent.com/68910144/137809084-632d69e5-2afd-468f-af08-9d175133e0f8.png)  
 ![image](https://user-images.githubusercontent.com/68910144/137809134-fa9f0faa-0ccc-4fdb-860b-d2c2b2cb21f4.png)  
 
 
 ---
 
# Py3 Iteration
  _list, tuple, dictionary, set_
  
  ### Iteration using for loop (for, while)
  - List = mutable, ordered
  - for x in list:
  - for x in "apple":
  - for x in list[0]:
  - break statement
  - nested loops
  - print( , sep=?, end=?)
  - print("{:02d}".format(hour))
  - for x, y in zip(X, Y)
  
  ### Enumerate()
  - syntax: enumerate(iterable, start=0)
    > iterable = object that supprts iteration
    > start = index value (counter is to be started, by default it is 0)


---

# Py4 Function
  __block of code which only runs when it is called__  
  __ Pass by value as parameter__  
  
  ### Arbitrary arguments
  - receive a tuple of arguments
  - *parameter-name  
   > ![image](https://user-images.githubusercontent.com/68910144/137818232-ed52bce8-f7e2-48c3-9139-be97a5ef1963.png)  
  
  ### Keyword arguments
  - arguments syntax: key = value
   > ![image](https://user-images.githubusercontent.com/68910144/137818914-99ba0be9-0c37-4701-b4ec-71838aa9e826.png)  
  
  ### Arbitrary Keyword arguments
  - **parameter name
  - receive syntax: key = value
   > ![image](https://user-images.githubusercontent.com/68910144/137819006-23239064-d127-424f-92b4-d11116d09263.png)  
  
  ### Default Paramenter Value
  - can call the function withut arguments
  
  ### Passing a list as an argument
  __can send any data types of argument to a function (String, Number, List, Dictionary etc.)__
  __it will be treated as the same data type inside the function__
   > ![image](https://user-images.githubusercontent.com/68910144/137819378-74b319f7-c349-4f6c-a616-4a4ed8a55460.png)  
  
  ### Return Values
   > ![image](https://user-images.githubusercontent.com/68910144/137819455-6b18ed9d-b697-49a5-b6b8-1357193d0a47.png)  
  
  
  ascii_lowercase & ascii_uppercase which are defined in string module
   > ![image](https://user-images.githubusercontent.com/68910144/137824936-d6f4de05-ffcf-448b-ae24-7427e04d455b.png)  


---

# Py5 String
  - single, double, triple quotes
  - len()
  
  ### Slice a single character
  - for i in range(len(str)): str[i]
  - for ch in str: ch
  
  ### Slice substring
  - syntax: var[lower:upper:step]
  - a[start:end] start~end-1
  - a[start:] start~
  - a[:end] ~end
  - a[:] *a copy of the whole list*
  - a[start:end:step] start~end-1, by step
  
  ### Slice - immutability of strings
  - s[0] = 'j' *TYPE ERROR*
   > t = s.replace('h', 'j')
   > s = 'j' + s[1:]
  
  ### String methods
  - count()
  - find (first occurrence, not == -1)
  - rfind (highest index, not == -1)
  - replace(old, new, count), default is all
  - 


---

# Py6 List
  __sequences of objects__
  __can contain a mix of any type of objects__
  __one of the workhorse data structures__
  
  ### Lists are mutable
  - can change the second element into uppercase
  
  ### Maling a list
  - list.append()
  - list += [x]
  
  ### indexing
  __same wqy as strings__
  - using list indexing (for i in range(len(rainbow)))
  - using list iterable (for color in rainbow)
  - using enumerating list (for i, color in enumerate(rainbow))
  
  ### Slicing
  - syntax: var[lower:upper:step]
  - replace elements with
  - delete elements
  - copying elements
   > b = a (얕은 복사)
   > b = a[:] (깊은 복사)
  
  ### Tuple
  - immutable
  - a[0] = a[0].upper() *TYPE ERROR*
  
  ### List Method
  - append(element)
  - extend(list)
  - inplace addition
  - count()
  - index(element) 
   > return index
  - insert(index)
   > insert(2, 'pink')
   > list[2:3] = ['pink', 'yellow']
  - remove(index)
   > remove(2)
   > list[2:3] = []
  - pop(index)
   > return value
  - sort()
   > in-place
   > don't want to modify -> use sorted()
  - reverse
   > in-place
  
  ### Operations on Lists
  - len()
  - sorted(), sorted(list, reverse = True), sorted(list, key = len)
  - del
  - in
  - not in


---

# Py7 Listcomp
  
  ### List comprehension
  - syntax: [expression for variable in iterable (if condition)]
  - kinds
   > list comprehension
   > set comprehension
   > dictionary comprehension
  
  ### Loop and Comprehension
  
  ### List Comprehension vs Loop
  - list comprehension is faster than loop
  
  ### Dictionary
  - construct a dictionary from a list
   > alist = [(), (), ()]
   > store = dict(alist)
  - list(store.keys())
  - list(store.values())
  - for k, v in store.item():
  
  ### Dict Comprehension
  - for k, v in zip(list1, list2):
