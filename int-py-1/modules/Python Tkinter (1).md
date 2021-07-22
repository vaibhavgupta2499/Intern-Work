# ***Python Tkinter***

**GUI (graphical user interface)** is a system of **interactive visual** components for computer software using items such as **icons, menus, windows,** etc

## ***Introduction***

* **Tkinter** is **inbuilt module** that is used for creating the **graphical user interface** for desktop based applications.
* **Tkinter** is most commonly used modules for creating **GUI applications in Python.**
* **Tkinter** provides a powerful **object-oriented interface** to the **Tk GUI toolkit.**

### ***What are widgets ?***

* **Tkinter** provides various **controls, such as buttons, labels and text boxes used in a GUI application.** These controls are commonly called **widgets.**
- The foundational element of a **Tkinter GUI is the window.** 
- Windows are the **containers in which all other GUI elements live.** 
- Widgets are contained **inside of windows.**

## ***Syntax:***

##### import Tkinter
##### top = Tkinter.Tk()
###### #Code to add widgets will go here...
##### top.mainloop()


```python

```

### ***There are currently 19 types of widgets in Tkinter***

1. **Button** - The Button widget is used to **display/add various kinds of buttons in python application.**
2. **Canvas** - The canvas widget is used to **draw the canvas on the window.**
3. **Checkbutton** - The Checkbutton is used to **display the CheckButton on the window.**
4. **Entry** - The entry widget is used to **display the single-line text field to the user.** It is commonly used to accept user values.
5. **Frame** - It can be defined as a **container to which, another widget can be added and organized.**
6. **Label** - A label is a text used to **display some message or information about the other widgets.**
7. **Listbox** - The ListBox widget is used to **display a list of options to the user.**
8. **Menubutton** - The Menubutton is used to **display the menu items to the user.**
9. **Menu** - It is used to **add menu items to the user.**
10. **Message** - The Message widget is used to **display the message-box to the user.**
11. **Radiobutton** - The Radiobutton is different from a **checkbutton.** Here, the user is provided with various options and the user can select only one option among them.
12. **Scale** - It is used to provide the **slider to the user.**
13. **Scrollbar** - It provides the scrollbar to the user so that the user can **scroll the window up and down.**
14. **Text** - It is different from Entry because it provides a **multi-line text field to the user** so that the user can write the **text and edit the text inside it.**
15. **Toplevel** - It is used to create a **separate window container.**
16. **Spinbox** - It is an entry widget used to **select from options of values** or which can be used to **select from a fixed number of values.**
17. **PanedWindow** - It is like a container widget that contains any **number of panes, horizontal or vertical panes.**  
18. **LabelFrame** - A LabelFrame is a simple container widget that acts as a **spacer or container for complex window layouts.**
19. **MessageBox** - This module is used to **display the message-box in applications.**


```python

```

### Tk also provides three geometry managers:
Tkinter widgets have access to specific geometry management methods, which have the purpose of organizing widgets throughout the parent widget area. They are :-
* **place** - which **positions widgets at absolute locations**
* **grid** - which **arranges widgets in a grid**
* **pack** - which **packs widgets into a cavity**

### 1. place() method

The **place()** organizes the widgets to the specific **x and y coordinates.**

**Syntax:- 
widget.place(options)** 

#### List of possible options −

- **Anchor:** It represents the **exact position of the widget within the container.** The **default value (direction)** is **NW (the upper left corner)**
- **bordermode:** The **default value** of the border type is **INSIDE that refers to ignore the parent's inside the border.** The other option is **OUTSIDE.**
- **height, width:** It refers to the **height and width in pixels.**
- **relheight, relwidth:** It is represented as the **float between 0.0 and 1.0** indicating the **fraction of the parent's height and width.**
- **relx, rely:** It is represented as the **float between 0.0 and 1.0** that is the offset in the **horizontal and vertical direction.**
- **x, y:** It refers to the **horizontal and vertical offset in the pixels.**


```python
from tkinter import *  
top = Tk()  
top.geometry("400x250")  
name = Label(top, text = "Name").place(x = 30,y = 50)  
email = Label(top, text = "Userid").place(x = 30, y = 90)  
password = Label(top, text = "Password").place(x = 30, y = 130)  
e1 = Entry(top).place(x = 80, y = 50)  
e2 = Entry(top).place(x = 80, y = 90)  
e3 = Entry(top).place(x = 95, y = 130)  
top.mainloop()  
```

![tkinter1.JPG](attachment:tkinter1.JPG)


```python

```

### 2. grid() method 

*  **grid()** geometry manager **organizes the widgets in the tabular form.**
* We can specify the **rows and columns as the options in the method call.** 
* We can also specify the **column span (width) or rowspan(height) of a widget.**

### **Syntax:** 
**widget.grid(options)**  

#### list of possible options 

* **Column**- The column number in which the **widget is to be placed. The leftmost column is represented by 0.**
* **Columnspan**- The **width** of the widget. It represents the number of columns up to which, the column is expanded.
* **ipadx, ipady**- It represents the **number of pixels** to pad the widget **inside the widget's border.**
* **padx, pady** - It represents the number of pixels to **pad the widget outside the widget's border.**
* **row** - The **row number in which the widget is to be placed.** The **topmost row is represented by 0.**
* **rowspan** - The **height of the widget**, i.e. the number of the **row** up to which the widget is **expanded.**


```python
from tkinter import *  
parent = Tk()  
name = Label(parent,text = "Name").grid(row = 0, column = 0)  
e1 = Entry(parent).grid(row = 0, column = 1)  
password = Label(parent,text = "Password").grid(row = 1, column = 0)  
e2 = Entry(parent).grid(row = 1, column = 1)  
submit = Button(parent, text = "Submit").grid(row = 6, column = 0)  
parent.mainloop()  
```

![tkinter2.JPG](attachment:tkinter2.JPG)

### 3. pack() method

- is used to **organize widget in the block.** 
- The positions widgets added to the python application using the **pack()** method can be controlled by using the various options specified in the **method call.**

**syntax: 
widget.pack(options)**  


#### A list of possible options 

* **expand**: If the expand is set to **true, the widget expands to fill any space.**
* **Fill**: By default, the fill is set to **NONE**. However, we can set it to **X or Y to determine whether the widget contains any extra space.**
* **size**: it represents the side of the **parent to which the widget is to be placed on the window.**


```python
from tkinter import *
root = Tk()
frame = Frame(root)
frame.pack()

bottomframe = Frame(root)
bottomframe.pack( side = BOTTOM )

redbutton = Button(frame, text="Red", fg="red")
redbutton.pack( side = LEFT)

greenbutton = Button(frame, text="green", fg="green")
greenbutton.pack( side = LEFT )

bluebutton = Button(frame, text="Blue", fg="blue")
bluebutton.pack( side = LEFT )

blackbutton = Button(bottomframe, text="Black", fg="black")
blackbutton.pack( side = BOTTOM)

root.mainloop()
```

![tkinter3.JPG](attachment:tkinter3.JPG)

### Advantages
- Tkinter is easy and fast to implement
- provides simple syntax
- very easy to understand
- part of python, nothing extra to download
- kinter’s three geometry managers are powerful and easy to use .

### Disadvantages
- Hard to debug
- very little printing support 
- does not include advanced widgets.
- It is not purely Pythonic.
- It doesn’t have a reliable UI.


```python

```
