
<p align="center">
   <img src="https://miro.medium.com/max/1200/1*PPIp7twJJUknfohZqtL8pQ.png" alt="Python Programming"
        width="500" height="150">
   <br />
   <b> PYTHON - TURTLE LIBRARY </b>
   <br />
   <b> This mark down file helps understand Turtle library in Python. </b>
   <br />
</p>

---

### 📋 Turtle Library in Python

<p align="justify">
   Turtle is a pre-installed Python library that enables users to create pictures and shapes by providing them with a virtual canvas. The onscreen pen used for drawing is called the turtle and this is what gives the library its name. In short, the Python turtle library helps new programmers get a feel for what programming with Python is like in a fun and interactive way. Turtle is mainly used to introduce children to the world of computers. It’s a straightforward yet versatile way to understand the concepts of Python. This makes it a great avenue for kids to take their first steps in Python programming. That being said, the Python turtle library is not restricted to little ones alone! It’s also proved extremely useful for adults who are trying their hands at Python, which makes it great for Python beginners.
</p>
</ br>

<b> Python Compatible Environment and Version for Turtle </b>
<p align="justify">
   Python Environment can be any of the applications among IDLE, Jupyter Notebooks. Python version has to be version-3 as Turtle is within the version-3 of Python. The good thing about turtle is that it’s a built-in library, so there's no need to install any new packages. The library can be put into use with just one line of code. Before beginning with libraries in  Python, let's understand what it is. In the non-computer world, a library is a place where different types of books are stored. These books can be accessed at any time, take whatever information is needed from them, and return them back to the same place. In the computer world, a library works similarly. By definition, a library is a set of important functions and methods that can be accessed to make programming easier. The Python turtle library contains all the methods and functions that one need to create own set of images. To access a Python library, just import it into the Python environment like this,
</p>

```
>>> import turtle
```
</br>

<b>Turtle Specific Methods</b>
<table class="table table-bordered">
<tr>
<th style="text-align:center;">Method</th>
<th style="text-align:center;">Parameters</th>
<th style="text-align:center;">Description</th>
</tr>
<tr>
<td>Turtle()</td>
<td>None</td>
<td>It creates and returns a new turtle object</td>
</tr>
<tr>
<td>forward()</td>
<td>Amount</td>
<td>It moves the turtle forward by the specified amount</td>
</tr>
<tr>
<td>backward()</td>
<td>Amount</td>
<td>It moves the turtle backward by the specified amount</td>
</tr>
<tr>
<td>right()</td>
<td>Angle</td>
<td>It turns the turtle clockwise</td>
</tr>
<tr>
<td>left()</td>
<td>Angle</td>
<td>It turns the turtle counter clockwise</td>
</tr>
<tr>
<td>penup()</td>
<td>None</td>
<td>It picks up the turtle’s Pen</td>
</tr>
<tr>
<td>pendown()</td>
<td>None</td>
<td>It puts down the turtle’s Pen</td>
</tr>
<tr>
<td>up()</td>
<td>None</td>
<td>It picks up the turtle’s Pen</td>
</tr>
<tr>
<td>down()</td>
<td>None</td>
<td>It puts down the turtle’s Pen</td>
</tr>
<tr>
<td>color()</td>
<td>Color Name</td>
<td>It changes the color of the turtle’s pen</td>
 </tr>
<tr>
<td>fillcolor()</td>
<td>Color Name</td>
<td>It changes the color of the turtle will use to fill a polygon</td>
</tr>
<tr>
<td>heading()</td>
<td>None</td>
<td>It returns the current heading</td>
</tr>
<tr>
<td>position()</td>
<td>None</td>
<td>It returns the current position</td>
</tr>
<tr>
<td>goto()</td>
<td>x, y</td>
<td>It moves the turtle to position x,y</td>
</tr>
<tr>
<td>begin_fill()</td>
<td>None</td>
<td>It remembers the starting point for a filled polygon</td>
</tr>
<tr>
<td>end_fill()</td>
<td>None</td>
<td>It closes the polygon and fills with the current fill color</td>
</tr>
<tr>
<td>dot()</td>
<td>None</td>
<td>It leaves the dot at the current position</td>
</tr>
<tr>
<td>stamp()</td>
<td>None</td>
<td>It leaves an impression of a turtle shape at the current location</td>
</tr>
<tr>
<td>shape()</td>
<td>Shape Name</td>
<td>It should be ‘arrow’, ‘classic’, ‘turtle’ or ‘circle’</td>
</tr>
</table>
</br>

<b> Steps for Executing Turtle Program in Python </b>
<p align="justify">
   
   - Import the Turtle module
   - Creating a seperate window
   - Creating a Turtle to control the flow
   - Graphic creation using the Turtle methods listed prior
</p>
</br>

<b> Program to Demonstrate the Turtle Library </b>
</br>
<p align="justify">
   A turtle screen has to be opened first, and a variable has to be initialized for it in the following way. It makes up a window called the screen, where the ouptut for the code can be viewed. The litte black triangular shape in the middle of the screen as shown in the figure is called the turtle. 
</p>

```
>>> dev = turtle.getscreen()
```

<p align="center">
   <img src="https://files.realpython.com/media/Screenshot_2019-12-10_at_7.40.34_AM.86e4071c3bb4.png" alt="Turtle Intro"
        width="400" height="300">
</p>
</br>

<p align="justify">
   Next, it is necessary to initialize the variable, which can then be used throughout the program to refer to the turtle. Just like for the screen, this also has to be given a name. The screen acts as a canvas, while the turtle acts like a pen. The turtle can be programmed to move around the screen. The turtle has certain changeable characteristics, like size, color, and speed. It always points in a specific direction, and will move in that direction until it is changed. When it is up, it means that no line will be drawn when it moves. When it is down, it means that a line will be drawn when it moves. The initialization can be done as follows,
</p>

```
>>> t = turtle.Turtle()
```

<p align="justify">
   There are four directions that a turtle can move in, i.e., forward, backward, left and right. The turtle moves .forward() or .backward() in the direction that it is facing. The direction can be changed by turning it .left() or .right() by a certain degree. The code for movement and direction can be as simple as,
</p>

```
>>> t.right(90) #can also use .rt()
>>> t.forward(100) #can also use .fd()
>>> t.left(90) #can also use .lt()
>>> t.backward(100) #can also use .bk()
```

<p align="justify">
  A line can also be drawn from the current position to any other arbitrary position on the screen. This is done with the help of coordinates. The screen is divided into four quadrants. The point where the turtle is initially positioned at the beginning of the program is (0,0). This is called Home. To move the turtle to any other area on the screen, .goto() function can be used with the coordinates passed as parameters. The first line of code draws a line from current position to (100,100) point on the screen. To bring back the turtle to its home position the second line of code can be used. Alternatively, third line of code can also be used to send the turtle back home, but the second one is quicker.
</p>

```
>>> t.goto(100,100) #goto (100,100)
>>> t.home() #goto home
>>> t.goto(0,0) #alternatively go to home
```

<b> Program to Draw a Polygon </b>

```
>>> import turtle
>>> polygon_ = turtle.Turtle()
>>> for i in range(6):
>>> polygon_.forward(100)
>>> polygon_.right(300)
>>> turtle.done()
```

<p align="center">
   <img src="https://cdn.educba.com/academy/wp-content/uploads/2020/03/Python-Turtle-2.jpg.webp" alt="polygon"
        width="200" height="200">
</p>

<b> Program to Draw a Star </b>

```
>>> import turtle
>>> star = turtle.Turtle()
>>> num_of_sides = 5
>>> length_of_side = 50
>>> each_angle = 720.0 / num_of_sides
>>> for i in range(num_of_sides):
>>> star.forward(length_of_side)
>>> star.right(each_angle)
>>> turtle.done()
```

<p align="center">
   <img src="https://cdn.educba.com/academy/wp-content/uploads/2020/03/Python-Turtle-3.jpg.webp" alt="star"
        width="200" height="200">
</p>

<b> Program to Draw a Colorful Spiral Pattern </b>

```
>>> from turtle import *
>>> colors = ['orange', 'red', 'pink', 'yellow', 'blue', 'green'] for x in range(360):
>>> pencolor(colors[x % 6])
>>> width(x / 5 + 1)
>>> forward(x)
>>> left(20)
```

<p align="center">
   <img src="https://cdn.educba.com/academy/wp-content/uploads/2020/03/Python-Turtle-4.jpg.webp" alt="spiral"
        width="200" height="200">
</p>

<b> Program to Draw a Hang Spiral Pattern </b>

```
>>> from turtle import *
>>> penup()
>>> for a in range(40, -1, -1):
>>> stamp()
>>> left(a)
>>> forward(20)
```

<p align="center">
   <img src="https://cdn.educba.com/academy/wp-content/uploads/2020/03/Python-Turtle-5.jpg.webp" alt="hang"
        width="200" height="200">
</p>

<p align="justify">
  Using basic commands, which are readable and understandable, one can create a window canvas like the "drawing box" to draw whatever they want just by giving the parameters for the turtle to move in the direction of desire. All the functions are the instructions for the Python program to follow. When all the functions listed out are used properly, the reult could be a great lot of visually beautiful designs and patterns. Python Turtle is a great library to encourage kids to acknowledge more about programming, especially Python. Turtle is powerful and it therefore means they do have a lot of functions or attributes. Yes, it is true but it is not possible to cover the functionality of all the defined attributes and therefore this markdown file is limiting down the number of functions. Most important functions under of the library have been explained very clearly. 
</p>


