
![Python](https://camo.githubusercontent.com/531b82c3b02c0b77a94498070b5890ce41ee94a572502f3db741d15bf45f9cb3/68747470733a2f2f6d69726f2e6d656469756d2e636f6d2f6d61782f313230302f312a505049703774774a4a556b6e666f685a71744c3870512e706e67)




# Operators & Operation in Python

In this , you'll learn everything about different types of operators in Python, their syntax and how to use them with examples.

## Table Of Contents


  - [**Introduction**](#introduction)
  - [**Types Of Operator**](#types-of-operator)
    - [Arithmetic Operators](#arithmetic-operators)
    - [Relational *(Comparison)* Operators](#relational-comparison-operators)
    - [Assignment Operators](#assignment-operators)
    - [Logical Operators](#logical-operators)
    - [Membership Operators](#membership-operators)
    - [Bitwise Operators](#bitwise-operators)
    - [Identity Operators](#identity-operators)
  - [**Precedence of Operators**](#precedence-of-operators)
  - [**Any All in Python**](#any-all-in-python)
    - [Any](#any)
    - [All](#all)
  - [**Conclusion**](#conclusion)



## **Introduction**

An **Operator** in Python are special symbol in Python that is used to perform specific mathematical or logical operation on values. In normal , we can say that it is symbols that designate that some sort of computation should be performed.
The values that the operators work on are called **operands**.<br>

 For example :- 
 ```python
 >>> 2+3
     5
 ```
*Here in the above  expression , + (plus) sign is the operator that performs addition. 2 and 3 are the operands and 5 is the output of the operation..*<br> 

Python supports several kinds of operators
whose categorisation is briefly explained in below  section.

## **Types Of Operator**

Python language supports the following types of operators.


  - [Arithmetic Operators](#arithmetic-operators)
  - [Relational *(Comparison)* Operators](#relational-comparison-operators)
  - [Assignment Operators](#assignment-operators)
  - [Logical Operators](#logical-operators)
  - [Membership Operators](#membership-operators)
  - [Bitwise Operators](#bitwise-operators)
  - [Identity Operators](#identity-operators)
  
Let us have a look on all operators one by one in below section .

## **Arithmetic Operators**

Python supports arithmetic operators that are used to perform the four basic arithmetic operations as well as modular division, floor division and exponentiation.<br>




|   Operator       |    Operation  |  Description  | Syntax |
| :-------------: | :-----------: | :-----------: | :---: |
| + | Addition    | Adds the two numeric values on either side of the operator<br> This operator can also be used to concatenate two strings on either side of the operator          |  x +y |
| - | Subtraction    | Subtracts the operand on the right from the operand on the left<br>            | x - y |
| * | Multiplication    | Multiplies the two values on both side of the operator<br>Repeats the item on left of the operator if first operand is a string and second operand is an integer value            | x * y |  
| / | Division    | Divides the operand on the left by the operand on the right and returns the quotient<br>     |  x / y |
| % | Modulus    | Divides the operand on the left by the operand on the right and returns the remainder<br>    |  x % y *(remainder of  x / y)* |
| // | Floor Division    | Divides the operand on the left by the operand on the right and returns the quotient by removing the decimal part. It is sometimes also called integer division<br>  | x // y |
| ** | Exponent   | Performs exponential (power) calculation on operands. That is, raise the operand on the left to the power of the operand on the right<br>        |  x ** y *(x to the power y)* |


### **Examples of Arithmetic Operator**

```python
  # Initialize The Value
    >>> a = 9
    >>> b = 4

  # Addition of numbers  
    >>> add = a + b  

  # Subtraction of numbers  
    >>> sub = a - b  

  # Multiplication of number  
    >>> mul = a * b  

  # Division(float) of number  
    >>> div1 = a / b  
     
  # Division(floor) of number  
    >>> div2 = a // b  

  # Modulo of both number  
    >>> mod = a % b  

   # Power 
    >>> p = a ** b 
   
    >>> print(add)  
    >>> print(sub)  
    >>> print(mul)  
    >>> print(div1)  
    >>> print(mod) 
    >>> print(div2)
    >>> print(p) 
```
### **Output**

```Python
      13
      5
      36
      2.25
      2
      1
      6561
```


## **Relational *(Comparison)* Operators**

Relational operator compares the values of the operands
on its either side and determines the relationship among them .


| Operator | Operation                              |                                                                                                                                        Description                                                                                                                                       | Example                           |
|----------|----------------------------------------|:----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------:|-----------------------------------|
|    ==    | Equals to                              | If the values of two operands are equal, then the condition is True,otherwise it is false                                                                                                                                                                                                | x == y                  |
| !=       | Not equal to                           | If values of two operands are not equal,then condition is True, otherwise condition is false                                                                                                                                                                                             | x != y                   |
| >        | Greater than                           | If the value of the left-side operand is greater than  the value of the right - side operand ,then condition is true, otherwise ,it is False                                                                                                                                             | x > y                  |
| <      | Less Than                           | If the value of the left-side operand is less than  the value of the right - side operand ,then condition is true, otherwise ,it is False                                                                                                                                             | x < y                  |
|   >=  |    Greater than  or equal to | If the value of the left -side operand is less than  the value of the right-side operand, then condition is true, otherwise, it is False    If the value of the left-hand operand is greater than or equal to value of right-hand operator,then condition is true, otherwise it is False | x >= y |
| <=       | Less than or equals to                 | If the value of the left-hand operant is less than or equal to  value of right -hand operator ,then condition is true, otherwise it is False                                                                                                                                             | x <= y                   |

### **Example Of Relational Operator**

```Python
# Initialize Value 
 >>> a = 13
 >>> b = 33

# a > b is False 
 >>> print(a > b) 

# a < b is True 
 >>> print(a < b) 

# a == b is False 
 >>> print(a == b) 

# a != b is True 
 >>> print(a != b) 

# a >= b is False 
 >>> print(a >= b) 

# a <= b is True 
 >>> print(a <= b)
```

### **Output**

```Python
     False
     True
     False
     True
     False
     True
```



## **Assignment Operators**

Assignment operator assigns or changes the value of
the variable on its left.

<table>
<thead>
<tr>
<th style="text-align:center">Operator</th>
<th style="text-align:center">Description</th>
<th style="text-align:center">Syntax</th>
<th style="text-align:center">Same As</th>
</tr>
</thead>
<tbody>
<tr>
<td style="text-align:center">=</td>
<td style="text-align:center">Assign value of right side of expression to left side operand</td>
<td style="text-align:center">x = y + z</td>
<td style="text-align:center"></td>
</tr>
<tr>
<td style="text-align:center">+=</td>
<td style="text-align:center">Add AND: Add right side operand with left side operand and then assign to left operand</td>
<td style="text-align:center">a+=b</td>
<td style="text-align:center">a=a+b</td>
</tr>
<tr>
<td style="text-align:center">-=</td>
<td style="text-align:center">Subtract AND: Subtract right operand from left operand and then assign to left operand</td>
<td style="text-align:center">a-=b</td>
<td style="text-align:center">a=a-b</td>
</tr>
<tr>
<td style="text-align:center">*=</td>
<td style="text-align:center">Multiply AND: Multiply right operand with left operand and then assign to left operand</td>
<td style="text-align:center">a*=b</td>
<td style="text-align:center">a=a*b</td>
</tr>
<tr>
<td style="text-align:center">/=</td>
<td style="text-align:center">Divide AND: Divide left operand with right operand and then assign to left operand</td>
<td style="text-align:center">a/=b</td>
<td style="text-align:center">a=a/b</td>
</tr>
<tr>
<td style="text-align:center">%=</td>
<td style="text-align:center">Modulus AND: Takes modulus using left and right operands and assign result to left operand</td>
<td style="text-align:center">a%=b</td>
<td style="text-align:center">a=a%b</td>
</tr>
<tr>
<td style="text-align:center">//=</td>
<td style="text-align:center">Divide(floor) AND: Divide left operand with right operand and then assign the value(floor) to left operand</td>
<td style="text-align:center">a//=b</td>
<td style="text-align:center">a=a//b</td>
</tr>
<tr>
<td style="text-align:center">**=</td>
<td style="text-align:center">Exponent AND: Calculate exponent(raise power) value using operands and assign value to left operand</td>
<td style="text-align:center">a**=b</td>
<td style="text-align:center">a=a**b</td>
</tr>
<tr>
<td style="text-align:center">&amp;=</td>
<td style="text-align:center">Performs Bitwise AND on operands and assign value to left operand</td>
<td style="text-align:center">a&amp;=b</td>
<td style="text-align:center">a=a&amp;b</td>
</tr>
<tr>
<td style="text-align:center">|=</td>
<td style="text-align:center">Performs Bitwise OR on operands and assign value to left operand</td>
<td style="text-align:center">a=| b</td>
<td style="text-align:center">a=a | b</td>
</tr>
<tr>
<td style="text-align:center">^=</td>
<td style="text-align:center">Performs Bitwise xOR on operands and assign value to left operand</td>
<td style="text-align:center">a^=b</td>
<td style="text-align:center">a=a^b</td>
</tr>
<tr>
<td style="text-align:center">&gt;&gt;=</td>
<td style="text-align:center">Performs Bitwise right shift on operands and assign value to left operand</td>
<td style="text-align:center">a&gt;&gt;=b</td>
<td style="text-align:center">a=a&gt;&gt;b</td>
</tr>
<tr>
<td style="text-align:center">&lt;&lt;=</td>
<td style="text-align:center">Performs Bitwise Left shift on operands and assign value to left operand</td>
<td style="text-align:center">a&lt;&lt;=b</td>
<td style="text-align:center">a=a&lt;&lt;b</td>
</tr>
</tbody>
</table>







## **Logical Operators**

There are three logical operators supported by Python.
These operators **(and, or, not)** are to be written in
lower case only. <br>The logical operator evaluates to either
True or False based on the logical operands on either
side. Every value is logically either True or False. 
<br>
By default, all values are True except None, False, 0
(zero), empty collections "", (), [], {}, and few other special
values.

| Operator    | Operations | Description | Example |
| :--------: | :---: |:---: | :---: |
| and | Logical AND  | If both the operands are True, then condition becomes True | x < 5 and x < 10 |
| or | Logical OR | If any of the two operands are True, then condition becomes True | x < 5 or x < 4 |
| not |  Logical NOT|  Used to reverse the logicalstate of its operand | not(x < 5 and x < 10) |

### **Example Of Logical Operator**

```Python
     # Examples of Logical Operator 
     >>> a = True
     >>> b = False

     # Print a and b is False 
     >>> print(a and b) 

     # Print a or b is True 
     >>> print(a or b) 

     # Print not a is False 
     >>> print(not a) 


```

### **Output**

```Python
     False
     True
     False

```


## **Membership Operators**

Membership operators are used to check if a value is a
member of the given sequence or not.

| Operator | Description                                                                                   | Example                                                                 |
|----------|-----------------------------------------------------------------------------------------------|:------------------------------------------------------------------------:|
| in       | Returns true if the variable/value is found in the specified sequence and False otherwise     | x in y |
| not in   | Returns True if the variable/value is not found in the specified sequence and False otherwise | x not in y                  |

### **Example Of Membership Operator**

```Python
  # Examples of Membership operator 
  >>> x = 'hello guys'
  >>> y = {3:'a',4:'b'} 


  >>> print('h' in x) 

  >>> print('Hello' not in x) 

  >>> print('hello' not in x) 

  >>> print(3 in y) 
```

### **Output**

```Python
  True
  True
  False
  True
```

## **Bitwise Operators**

Bitwise operators treat operands as sequences of binary digits and operate on them bit by bit.<br> The following operators are supported:

<table>
<thead>
<tr>
<th style="text-align:center">Methods</th>
<th style="text-align:center">Description</th>
<th style="text-align:center">Example</th>
</tr>
</thead>
<tbody>
<tr>
<td style="text-align:center">&amp;</td>
<td style="text-align:center">AND</td>
<td style="text-align:center">Sets each bit to 1 if both bits are 1</td>
</tr>
<tr>
<td style="text-align:center">|</td>
<td style="text-align:center">OR</td>
<td style="text-align:center">Sets each bit to 1 if one of two bits is 1</td>
</tr>
<tr>
<td style="text-align:center">^</td>
<td style="text-align:center">XOR</td>
<td style="text-align:center">Sets each bit to 1 if only one of two bits is 1</td>
</tr>
<tr>
<td style="text-align:center">~</td>
<td style="text-align:center">NOT</td>
<td style="text-align:center">Inverts all the bits</td>
</tr>
<tr>
<td style="text-align:center">«</td>
<td style="text-align:center">Zero fill left shift</td>
<td style="text-align:center">Shift left by pushing zeros in from the right and let the leftmost bits fall off</td>
</tr>
<tr>
<td style="text-align:center">»</td>
<td style="text-align:center">Signed right shift</td>
<td style="text-align:center">Shift right by pushing copies of the leftmost bit in from the left, and let the rightmost bits fall off</td>
</tr>
</tbody>
</table>



### **Example Of Bitwise Operator**

```Python
 # Initialize Value
 >>> a = 10
 >>> b = 4

 # Print bitwise AND operation   
 >>> print(a & b) 

 # Print bitwise OR operation 
 >>> print(a | b) 

 # Print bitwise NOT operation  
 >>> print(~a) 

 # print bitwise XOR operation  
 >>> print(a ^ b) 

 # print bitwise right shift operation  
 >>> print(a >> 2) 

 # print bitwise left shift operation  
 >>> print(a << 2) 
```

### **Output**

```Python
    0
   14
  -11
   14
   2
   40
```






## **Identity Operators**

Identity operators are used to determine whether the
value of a variable is of a certain type or not. Identity
operators can also be used to determine whether two variables are referring to the same object or not. There
are two identity operators.

  | Operator |                                                                                          Description                                                                                          | Example                                                                                                                    |
|----------|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------:|----------------------------------------------------------------------------------------------------------------------------|
| is | Evaluates True if the variables on either side of the operator point towards the same memory location and False otherwise. var1 is var2 results to True  if id(var1)is  equal to id(var2)     | x is y |
| is not   | Evaluates to False if the variables on   either side  of the operator point to same memory location and True otherwise. var1 is not var2 results to True if id(var1) is not equal to id(var2)| x is not y <br>                                                                                             |                           

### **Example Of Identity Operator**

```Python
 # Initializing Value 
 >>> a1 = 3
 >>> b1 = 3
 >>> a2 = 'hello'
 >>> b2 = 'hello'
 >>> a3 = [1,2,3] 
 >>> b3 = [1,2,3] 
 >>> print(a1 is not b1) 


 >>> print(a2 is b2) 

# Output is False, since lists are mutable. 
 >>> print(a3 is b3) 
```

### **Output**

```Python
     False
     True
     False
```



    
## **Precedence of Operators**


Evaluation of the expression is based on precedence of
operators. When an expression contains different kinds
of operators, precedence determines which operator
should be applied first. <br>***Higher precedence operator is
evaluated before the lower precedence operator.*** Most
of the operators studied till now are binary operators.
Binary operators are operators with two operands.
The unary operators need only one operand, and they
have a higher precedence than the binary operators.
The minus (-) as well as + (plus) operators can act as
both unary and binary operators, but not is a unary
logical operator.<br>
```Python
# Depth is using - (minus) as unary operator
Value = -Depth
# not is a unary operator, negates True
print(not(True))
```
The following table lists precedence of all operators
from highest  to  lowest  :- <br>


| Order of precedence | Operators              | Description                               |
|---------------------|------------------------|-------------------------------------------|
| 1                   | **                     | Exponentiation(raised to the power        |
| 2                   | -,+,-                  | Complement, unary plus and unary minus    |
| 3                   | *,/,%,//               | Multiply,divide,modulo and floor division |
| 4                   | +,-                    | Addition and Subtraction                  |
| 5                   | <=,<,>,>=              | Relational Operators                      |
| 6                   | ==,!=                  | Equality operators                        |
| 7                   | =,%=,/=,//=,-=, *=,+*= | Assignment operators                      |
| 8                   | is, is not             | Identity operators                        |
| 9                   | in,not in              | Membership operators                      |
| 10                  | not,or,and             | Logical operators                         |

**Note :-**
*  Parenthesis can be used to override the precedence of
operators. The expression within () is evaluated first.<br>
*  For operators with equal precedence, the expression is
evaluated from left to right.<br>    


##  **How will Python evaluate the following expression?**


**20 + 30 * 40** <br>
 >> Solution:<br>
  = 20 + (30 * 40) #Step 1<br>
precedence of * is more than that of + <br>
 = 20 + 1200 #Step 2<br>
 = 1220 #Step 3<br>


##  How will the following expression be evaluated in Python?
 **15.0 / 4 + (8 + 3.0)**
 >>Solution:<br>
 = 15.0 / 4 + (8.0 + 3.0) #Step 1<br>
 = 15.0 / 4.0 + 11.0 #Step 2<br>
 = 3.75 + 11.0 #Step 3<br>
 = 14.75 #Step 4<br>



## **Any All in Python**

Any and All are two built ins provided in python used for successive And/Or.
Let Us Discuss It One By One :-

### __*Any*__

Returns true if any of the items is True. It returns False if empty or all are false. Any can be thought of as a sequence of OR operations on the provided iterables. It short circuit the execution i.e. stop the execution as soon as the result is known.

### *Syntax :-*

```Python
 any(list of iterables)
```

### *Example*

```Python
 # Since all are false, false is returned 
 >>> print (any([False, False, False, False])) 

 # Here the method will short-circuit at the 
 # second item (True) and will return True. 
 >>> print (any([False, True, False, False])) 

 # Here the method will short-circuit at the 
 # first (True) and will return True. 
 >>> print (any([True, False, False, False])) 

```

### *Output*

```Python

 False
 True
 True

```


### __*All*__

Returns true if all of the items are True *(or if the iterable is empty)*. All can be thought of as a sequence of AND operations on the provided iterables. It also short circuit the execution i.e. stop the execution as soon as the result is known.

### *Syntax :-*

```Python
 all(list of iterables)

```

### *Example*

```Python
# Here all the iterables are True so all 
# will return True and the same will be printed 
 >>> print (all([True, True, True, True])) 

# Here the method will short-circuit at the  
# first item (False) and will return False. 
 >>> print (all([False, True, True, False])) 

# This statement will return False, as no 
# True is found in the iterables 
 >>> print (all([False, False, False])) 


```

### *Output*

```Python

 True
 False
 False


```




 ## **Conclusion**

 In this, you learned about the diverse operators that Python supports to combine objects into expressions.