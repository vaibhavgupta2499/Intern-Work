
<p align="center">
   <img src="https://miro.medium.com/max/1200/1*PPIp7twJJUknfohZqtL8pQ.png" alt="Python Programming"
        width="500" height="150">
   <br />
   <b> VARIABLES AND DATATYPES IN PYTHON </b>
   <br />
   <b> This mark down file helps understand VARIABLES and DATATYPES in PYTHON. </b>
   <br />
</p>

---

### 📋 Variables in Python

<p align="justify">
   Variables in Python are identifiers just like in any other programming language. They can be treated off like a name given to a memory location. Once a variable is declared, the memory block could be located using only the variable name. Any operations on that particular memory location have to be performed using the variable name. Variables always need to go through two stages, one is declaration and other one is initialization. Variable declaration deals with assigning the user-defined identifier as a name to a memory location, and initialization is assigning a value to that particular memory location. In general, two stages are combined into a single statement but in most of the programming languages explicit definition of a datatype is necessary, which is not the case with Python.
</p>
<p align="justify">
   Python is not a "statically-typed" language, therefore variable declaration doesn't even exist. A variable is created only when a value is assigned to it. As the variable is being provided with the value it is going to hold beforehand, defining the datatypes is not needed. Just like in any other programming language, if the variable name is used and an operation is performed, the operations' result reflects the value held in the memory location.
</p>
</ br>

<b> Rules for naming variables in Python </b>
<p align="justify">
   All programming languages have certain rules that need to be followed when programmer is working with variables. Python is no different. Almost all the programming languages have similar rules for naming variables, but to be specific the rules to be followed in Python are thereby,
</p>

   - The variable name can only have alpha-numeric characters and an underscore (A-Z, a-z, _).
   - The variable name can begin with a alphabet or an underscore i.e., they cannot begin with a numeric character.
   - Just like in most of the programming languages, variables in Python are case-sensitive.
   - Keywords in Python cannot be used as a variable names.

<p align="justify">
   Python doesn't require explicit datatype definition, but it doesn't limit it to only a particular datatype. When a variable in Python is defined, assigning it to a numeric value, impicitly it means that the variable defined holds numeric data and therefore datatype assigned to this variable would be numeric. But the same variable can be used to hold strings as well, and if a string is assigned to the same variable, the variable now is of the string type. The programmer always can change the value of the variable, which in turn could lead to change in type of the variable, which most of the programming languages fail to provide.
</p>

```
a=10 #assigning a numeric value
>>> print a
10
>>> a= “Hello” #reassigning a string value
>>> print a
Hello
b=c=20 #multiple variable assignment
>>> print(b)
20
>>> print(c)
20
```

---

### 📋 Datatypes in Python

<p align="justify">
   The data type of a variable or object determines which operations can be applied to it. Once a variable is assigned a data type, it can be used for computations in the program. The best thing about Python is that the data type doesn’t need to be defined when declaring a variable. Data types exist, but the variables are not bound to any of them. Languages that act in this way are called "dynamically-typed" languages. The datatypes in Python can be categorized into two,
   
   - Primitive Datatypes
   - Non-Primitive Datatypes (Python specific datatypes)
   
</p>

<p align="center">
   <img src="http://hindiwalo.com/wp-content/uploads/2020/06/Untitled-Document-3-1024x656.png" alt="Datatypes in Python"
        width="700" height="500">
</p>
<b> Primitive Datatypes in Python </b>
</br>
<p align="justify">
   Primitive datatypes can be defined as the most basic datatypes of any programming language. They alongside variables form the building blocks of the program. These are the datatypes upon which non-primitive datatypes are built. Primitive datatypes are mutable in nature, meaning the variable declared using these datatypes can have a change in its value. Primitive datatypes in Python can furthur be classified into four.
   
   - Integer
   - Float
   - Complex
   - String
</p>
<p align="justify">
<b>Integer</b> value is represented by the int class. It contains positive or negative whole numbers (without fraction or decimal). In Python, there is no limit to how long an integer value can be.
</p>
<p align="justify"> 
<b>Float</b> value is represented by the float class. It is a real number with floating point representation. It is specified by a decimal point. Optionally, the character e or E followed by a positive or negative integer may be appended to specify scientific notation. 
</p>
<p align="justify">
<b>Complex Number</b> is represented by the complex class. It is specified as (real part) + (imaginary part)j. If for example, the complex number is 5+5j, real part is 5 and the imaginary part is 5 again.
</p>
<p align="justify">
Like many other popular programming languages, <b>strings</b> in Python are arrays of bytes representing unicode characters. However, Python does not have a character data type, a single character is simply a string with a length of 1. Square brackets can be used to access elements of the string.
</p>

```
a=10 #assigning a integer value
>>> print a
10
>>> print(type(a)) #print the type of a
>>> <class 'int'> #int type

a=10.3 #assigning a float value
>>> print a
10.3
>>> print(type(a)) #print the type of a
>>> <class 'float'>

a=5+3j #assigning a complex value
>>> print a
5+3j
>>> print(type(a)) #print the type of a
>>> <class 'complex'>

a="HELLO" #assigning a string value
>>> print a
HELLO
>>> print(type(a)) #print the type of a
>>> <class 'str'>
```
<p align="justify">
These are only the basic primitive datatypes in Python. But it is not like Python has only these primitive datatypes. There are many more which include boolean, long.. etc. but they are out of scope of this markdown file.
</p>
</br>
<b> Non-Primitive Datatypes in Python </b>
</br>
<p align="justify">
   Non-Primitive datatypes can be defined as the derived datatypes. These are the datatypes which are built upon primitive datatypes. In contrast to primitive datatypes, non-primitive data types not only store values, but a collection of values in different formats. Non-Primitive datatypes in Python can further be classified into four.
   
   - List
   - Tuple
   - Set
   - Dictionary
</p>
<b> Lists </b>
<p align="justify">
Lists are a very useful variable type in Python. A list can contain a series of values. List variables are declared by using brackets [ ] following the variable name. All lists in Python are zero-based indexed. When referencing a member or the length of a list, the number of list elements is always the number shown plus one. Assigning data to a specific element of the list can be done using an index of the list. The list index starts at zero. Lists aren’t limited to a single dimension. Although most people can’t comprehend more than three or four dimensions, lists having multiple dimensions can be declared by separating it with commas.
</p>
<b> List Functions </b>
<p align="justify"> 
<b> append() </b> method adds an item to the end of the list. The method takes a single argument which is added to the end of list. The argument can be a number, string, dictionary, another list, and so on.
</p>
<p align="justify">
<b> index() </b> method returns the index of the specified element in the list. The list index() method can take a maximum of three arguments, element which is the element to be searched,  start(optional) which is the index from which the search starts and end(optional) which is the index at which the search should stop. The list index() method returns the index of the given element in the list. If the element is not found, a ValueError exception is raised. One important thing to note is that index() method only returns the first occurrence of the matching element.
</p>
<p align="justify">
<b> insert() </b> method inserts an element to the list at the specified index. The insert() method takes two parameters, index which indicates the position at which new element has to be inserted and element which is the element to be inserted in the list. If index is 0, the element is inserted at the beginning of the list. If index is 3, the index of the inserted element will be 3 (4th element in the list). All the elements after index are shifted to the right.
</p>
<p align="justify">
<b> count() </b> method returns the number of times the specified element appears in the list. The count() method takes a single argument, element, the element's whose number of occurances need to be counted. The count() method returns the number of times element appears in the list.
</p>
<p align="justify">
<b> remove() </b> method removes the first matching element (which is passed as an argument) from the list. The remove() method takes a single element as an argument and removes it from the list. If the element doesn't exist, it throws ValueError: list.remove(x): x not in list exception.
</p>
<p align="justify">
<b> pop() </b> method removes the item at the given index from the list and returns the removed item. The pop() method takes a single argument (index). The argument passed to the method is optional. If not passed, the default index -1 is passed as an argument (index of the last item). If the index passed to the method is not in range, it throws IndexError: pop index out of range exception. The pop() method returns the item present at the given index. This item is also removed from the list.
</p>

```
List1=[]
List1.append(1) #appending an element into the list
>>>print(List1)
[1]
>>>print(List1.index(1)) #finding the position of 1 in the list using index()
0
List1.insert(2, 1) #inserting an element at index 1 i.e., II position
List1.insert(3, 2) #inserting an element at index 2 i.e., III position
>>>print(List1)
[1, 2, 3]
>>>print(List1.count(1)) #checking the number of occurances of 1 in the list using count()
1
List1.remove(2) #removing an element from the list
>>>print(List1)
[1, 3]
List1.pop(0) #popping element at index 0 i.e., I position (if argument not passed, last item is popped)
>>>print(List1)
[3]
```
</br>
<b> Tuples </b>
<p align="justify">
Tuples are a group of values like a list and are manipulated in similar ways. But, tuples are fixed in size once they are assigned. In Python, the fixed size is considered immutable as compared to a list that is dynamic and mutable. Tuples are defined by parenthesis(). Advantages of using tuples over lists could include some of the following.
   
   - Tuples do not have append or extend method. They are fixed-size and therefore are fast.
   - IN operator can also be used for the same purpose i.e., to check if an element exists or not.
   - Constant set of values need to be defined in a tuple instead of a list always because they are fast.
   - It makes the code safe as tuple offers “write-protect” data that does not change.
</p>
<p align="justify">
All the functions used for a list retreival could be applied to a tuple as well, the only difference being tuple doesn't support append() and extend() because tuples are immutable and extending them or appending items to them is not possible. It doesn't allow insertion of elements as well, i.e., doesn't have an insert(). Removal of elements is also not possible, meaning remove() is not supported as well! When removal is not possible, it is quite explanatory that even pop() is not supported.
</p>

```
Tuple1=('A','B','C','D')
>>>print(Tuple1) #printing the elements of the tuple
('A', 'B', 'C', 'D')
>>>print(Tuple1.index('B')) #finding the position of 'A' in the tuple using index()
1
>>>print(Tuple1.count('C')) #checking the number of occurences of 'C' in the tuple using count()
1
```
</br>
<b> Sets </b>
<p align="justify">
A set is an unordered collection of items. Every set element is unique, that is, no duplications are allowed and must be immutable, that is they cannot be changed once defined. However, a set in itself is mutable. Set offers appending, extending, and removing item capability. Sets can be used to perform mathematical set operations like union, intersection, symmetric difference, etc. A set is created by placing all the items (elements) inside curly braces {}, separated by comma. It can have any number of items and they may be of different types (integer, float, tuple, string). But a set cannot have mutable elements like lists, sets or dictionaries as its elements.
</p>
<b> Set Functions </b>
<p align="justify">
Just like the other two, sets also support appending, inserting, and removal of elements. Some functions specific to sets which could provide high mathematical capabilities are as follows:
</p>
<p align="justify">
<b> difference() </b> method returns the set difference of two sets. If A and B are two sets, the set difference of A and B is a set of elements that exists only in set A but not in B. The difference() method returns the difference between two sets which is also a set but doesn't modify original sets. Set difference could also be found using the '-' operator.
</p>
<p align="justify">
<b> difference_update() </b> updates the set calling the difference_update() method with the difference of sets. If A and B are two sets, the set difference of A and B is a set of elements that exists only in set A but not in B. But the difference is now updated to set A unlike the difference() function. When the code is executed, result will be equal to None, A will be equal to A-B and B will be unchanged.
</p>
<p align="justify">
<b> intersection() </b> method returns a new set with elements that are common to all sets because the intersection of two or more sets is the set of elements that are common to all the sets. The intersection() method returns the intersection of set A with all the sets (passed as arguments). If the argument is not passed to intersection(), it returns a shallow copy of the set (A). Set difference could also be found using the '&' operator.
</p> 
<p align="justify">
<b> intersection_update() </b> updates the set calling intersection_update() method with the intersection of sets. Again, the intersection of two or more sets is the set of elements which are common to all sets. So, if A, B, C are three sets, the set intersection of A, B, C is a set of common elements that exists in set A, in set B and also in set C. When the code is executed, result will be None, A will be equal to the intersection of A, B, and C, the sets B and C remain unchanged.
</p>
<p align="justify">
<b> union() </b> method returns a new set with distinct elements from all the sets. The union of two or more sets is the set of all distinct elements present in all the sets. The union() method returns a new set with elements from the set and all other sets (passed as an argument). If the argument is not passed to union(), it returns a shallow copy of the set. Set union could also be found using the '|' operator.
</p>

```
A = {'18', '5', '88', '12'} #SetA
B = {'18', '9', '0'} #SetB
>>>print(A.difference(B)) #A-B
{'88', '5', '12'}
>>>print(B-A) #B-A using '-' operator
{'0', '9'}
>>>print(A.difference_update(B)) #A-B and A updated to A-B
None
>>>print(A)
{'5', '12', '88'}
A = {'18', '5', '88', '12'} #SetA
>>>print(A.intersection(B)) #A&B
{'18'}
>>>print(B&A) #B&A using '&' operator
{'18'}
>>>print(A.intersection_update(B)) #A&B and A updated to A&B
None
>>>print(A)
{'18'}
A = {'18', '5', '88', '12'} #SetA
>>>print(A.union(B)) #A|B
{'9', '12', '18', '5', '0', '88'}
>>>print(B|A) #B|A using '|' operator
{'18', '5', '88', '0', '12', '9'}
```
</br>
<b> Dictionaries </b>
<p align="justify">
Python dictionary is an unordered collection of items. Each item of a dictionary has a key/value pair. Dictionaries are optimized to retrieve values when the key is known. Creating a dictionary is as simple as placing items inside curly braces {} separated by commas. An item has a key and a corresponding value that is expressed as a pair (key: value). While the values can be of any data type and can repeat, keys must be of immutable type (string, number or tuple with immutable elements) and must be unique. Dictionary can also be created using the built-in dict() function.
</p>
<b> Dictionary Functions </b>
<p align="justify">
<b> items() </b> method returns a view object that displays a list of dictionary's (key, value) tuple pairs. The items() method is similar to dictionary's viewitems() method in Python 2.7. The items() method doesn't take any parameters. It returns a view object that displays a list of a given dictionary's (key, value) tuple pair.
</p>
<p align="justify">
<b> get() </b> method returns the value for the specified key if key is in dictionary. get() method takes maximum of two parameters, the key which is the key to be searched in the dictionary and the value(optional), which is the value to be returned if the key is not found. The default value is None. It returns the value for the specified key if key is in dictionary, None if the key is not found and value is not specified and value if the key is not found and value is specified. The difference between direct access i.e., dictionary['key'] and get() is when the key is not found and we use the direct access method, an expection is raised. That can be avoided by specifying the 'value' attribute of the get() function.
</p>
<p align="justify">
<b> keys() </b> method returns a view object that displays a list of all the keys in the dictionary. The keys() doesn't take any parameters. The keys() returns a view object that displays a list of all the keys. When the dictionary is changed, the view object also reflects these changes.
</p>
<p align="justify">
<b> values() </b> method returns a view object that displays a list of all the values in the dictionary. The values() method doesn't take any parameters. It returns a view object that displays a list of all values in a given dictionary. If the dictionary is updated at any time, the changes are always reflected.
</p>
<p align="justify">
<b> clear() </b> method removes all items from the dictionary. It doesn't take any parameters and returns None.
</p>

```
Dict1 = { 'A': 1, 'B': 2, 'C': 3 }
>>>print(Dict1.items()) #To print all key-value pairs
dict_items([('A', 1), ('B', 2), ('C', 3)])
>>>print(Dict1.get('A')) #To print value of key 'A'
1
>>>print(Dict1.get('D')) #To print value of key 'D' which is non-existent
None
>>>print(Dict1.get('D',0)) #To print value of key 'D' which is non-existent providing a default value
0
>>>print(Dict1.keys()) #To print all the keys
dict_keys(['A', 'B', 'C'])
>>>print(Dict1.values()) #To print all the values
dict_values([1, 2, 3])
>>>print(Dict1.clear()) #To clear the dictionary off
None
```

<p align="justify">
These datatypes have a lot of capabilities and that is the reason Python is so powerful. The capabilities are always acheived making use of functions. It therefore means these non-primitive datatypes have a lot of functions or attributes to be even more specific. Yes, it is true but it is not possible to cover the functionality of all the defined attributes and therefore this markdown file is limiting down the number of functions. Most important functions under each datatype have been explained very clearly.
</p>

   















   








