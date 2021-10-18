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
 - Read a remote file and process the text (requests.get(), from urllib.request import urlopen)
 - count()
 - Function (def:)
 - import matplotlib.pyplot as plt (plt.plot(x,y), plt.show())
 - import numpy as np (np.arange(start, stop, step)
 - np.cos(), np.sin()
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
 - print("Hello", "World") Have Blank
 - print("Hello" + "World") No Blank
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
 
 
