# PYTHON RECAP

 Python has no command for declaring a variable.

x = 5
y = "John"
print(x)
print(y)

## Casting

If you want to specify the data type of a variable, this can be done with casting.

x = str(3)    # x will be '3'
y = int(3)    # y will be 3
z = float(3)  # z will be 3.0

## Get the Type

x = 5
y = "John"
print(type(x)) # <type 'int'>
 
print(type(y)) # <type 'str'>

## global variable 
If you create a variable with the same name inside a function, this variable will be local, and can only be used inside the function. The global variable with the same name will remain as it was, global and with the original value.

## Data types

 *Text Type:	str # eg 'hello'
 *Numeric Types:	int, float, complex  
 *Sequence Types:	list, tuple, range
 *Mapping Type:	dict
 *Set Types:	set, frozenset
 *Boolean Type:	bool
 *Binary Types:	bytes, bytearray, memoryview
 *None Type:	NoneType

### Getting the Data Type

x = 5 

print (type(x))

### setting the Data type 
 *x = "Hello World"-------str	
 *x = 20	----------------int	
 *x = 20.5	------------float	
 *x = 1j----------------	complex	
 *x = ["apple", "banana", "cherry"]-------------	list	
 *x = ("apple", "banana", "cherry")-------------	tuple	
 *x = range(6)------------	range	
 *x = {"name" : "John", "age" : 36}--------------	dict	
 *x = {"apple", "banana", "cherry"}--------------	set	
 *x = frozenset({"apple", "banana", "cherry"})----------------	frozenset	
 *x = True-------------	bool	
 *x = b"Hello"----------------------	bytes	
 *x = bytearray(5)------------bytearray	
 *x = memoryview(bytes(5))--------	memoryview	
 *x = None

### setting the specific Data type 

 *x = str("Hello World")------------------	str	
 *x = int(20)	----------------int	
 *x = float(20.5)---------------	float	
 *x = complex(1j)	----------------complex	
 *x = list(("apple", "banana", "cherry"))-----------------	list	
 *x = tuple(("apple", "banana", "cherry"))----------------	tuple	
*x = range(6)----------------	range	
 *x = dict(name="John", age=36)------------	dict	
 *x = set(("apple", "banana", "cherry"))-------------	set	
 *x = frozenset(("apple", "banana", "cherry"))------------	frozenset	
 *x = bool(5)--------------	bool	
 *x = bytes(5)----------	bytes	
 *x = bytearray(5)----------	bytearray	
 *x = memoryview(bytes(5))-----------	memoryview	

## Type conversion

x = 16.0
y = 2
z = 7
print (int(x)) ----16
print (float(y)) ---2.0
print (complex(z))---(7+0j)

## Random Number
Python does not have a random() function to make a random number, but Python has a built-in module called random that can be used to make random numbers:

import random

print(random.randrange(1, 10))

## python casting 

x = int(7.0)
print(x) ----- ans 7

## Strings 

python strings have either single or double quotation marks 

### Multiline Strings
Multiline Strings
a = """Lorem ipsum dolor sit amet,
consectetur adipiscing elit,
sed do eiusmod tempor incididunt
ut labore et dolore magna aliqua."""
print(a)

### Looping Through a String
Since strings are arrays, we can loop through the characters in a string, with a for loop.

for x in 'Kariuki':
    print(x)

    ans 
K
a
r
i
u
k
i

###  String Length
To get the length of a string, use the len() function.

###  Check String
To check if a certain phrase or character is present in a string, we can use the keyword in.

## upper case 

x = "hello"
print (a.upper())

## lower case 
a = HELLO
print (a.lower())

## Remove Whitespace
Whitespace is the space before and/or after the actual text, and very often you want to remove this space.

a = "hello  world"
print (a.strip())
 ## additional 
 replace 
 The replace() method replaces a string with another string


 ### Python String split()

The split() method breaks up a string at the specified separator and returns a list of strings.

text = 'Python is a fun programming language'

# split the text from space
print(text.split(' '))

 Output: ['Python', 'is', 'a', 'fun', 'programming', 'language']

## String Concatenation
To concatenate, or combine, two strings you can use the + operator.

a = "Hello"
b = "World"
c = a + b
print(c)

output Hello World 
## string format

quantity = 3
itemno = 567
price = 49.95
myorder = "I want {} pieces of item {} for {} dollars."
print(myorder.format(quantity, itemno, price))


Mathematical operators

 *+	Addition	x + y	
 *-	Subtraction	x - y	
 **	Multiplication	x * y	
 */	Division	x / y	
 *%	Modulus	x % y	
 ***	Exponentiation	x ** y	
 *//	Floor division	x // y   15//2 output 7 


Operator	Example	Same As	Try it
 *=	x = 5	x = 5	
 *+=	x += 3	x = x + 3	
 *-=	x -= 3	x = x - 3	
 **=	x *= 3	x = x * 3	
 */=	x /= 3	x = x / 3	
 *%=	x %= 3	x = x % 3	
 *//=	x //= 3	x = x // 3	
 ***=	x **= 3	x = x ** 3	
 *&=	x &= 3	x = x & 3	
 *|=	x |= 3	x = x | 3	
 *^=	x ^= 3	x = x ^ 3	
 *>>=	x >>= 3	x = x >> 3	
 *<<=	x <<= 3	x = x << 3


## List 
## append 

To add an item to the end of the list, use the append() method:

## Extend List
To append elements from another list to the current list, use the extend() method.

thislist = ["apple", "banana", "cherry"]
tropical = ["mango", "pineapple", "papaya"]
thislist.extend(tropical)
print(thislist)

The extend() method does not have to append lists, you can add any iterable object (tuples, sets, dictionaries etc.).

## Remove Specified Item
The remove() method removes the specified item.

### Loop Through the Index Numbers
You can also loop through the list items by referring to their index number.
### string methods
Use the range() and len() functions to create a suitable iterable.

 *capitalize()	Converts the first character to upper case
 *casefold()	Converts string into lower case
 *center()	Returns a centered string
 *count()	Returns the number of times a specified value occurs in a string
 *encode()	Returns an encoded version of the string
 *endswith()	Returns true if the string ends with the specified value
 *expandtabs()	Sets the tab size of the string
 *find()	Searches the string for a specified value and returns the position of where it was found
 *format()	Formats specified values in a string
 *format_map()	Formats specified values in a string
 *index()	Searches the string for a specified value and returns the position of where it was found
 *isalnum()	Returns True if all characters in the string are alphanumeric
 *isalpha()	Returns True if all characters in the string are in the alphabet
 *isdecimal()	Returns True if all characters in the string are decimals
 *isdigit()	Returns True if all characters in the string are digits
 *isidentifier()	Returns True if the string is an identifier
 *islower()	Returns True if all characters in the string are lower case
 *isnumeric()	Returns True if all characters in the string are numeric
 *isprintable()	Returns True if all characters in the string are printable
 *isspace()	Returns True if all characters in the string are whitespaces
 *istitle()	Returns True if the string follows the rules of a title
 *isupper()	Returns True if all characters in the string are upper case
 *join()	Joins the elements of an iterable to the end of the string
 *ljust()	Returns a left justified version of the string
 *lower()	Converts a string into lower case
 *lstrip()	Returns a left trim version of the string
 *maketrans()	Returns a translation table to be used in translations
 *partition()	Returns a tuple where the string is parted into three parts
 *replace()	Returns a string where a specified value is replaced with a specified value
 *rfind()	Searches the string for a specified value and returns the last position of where it was found
 *rindex()	Searches the string for a specified value and returns the last position of where it was found
 *rjust()	Returns a right justified version of the string
 *rpartition()	Returns a tuple where the string is parted into three parts
 *rsplit()	Splits the string at the specified separator, and returns a list
 *rstrip()	Returns a right trim version of the string
 *split()	Splits the string at the specified separator, and returns a list
 *splitlines()	Splits the string at line breaks and returns a list
 *startswith()	Returns true if the string starts with the specified value
 *strip()	Returns a trimmed version of the string
 *swapcase()	Swaps cases, lower case becomes upper case and vice versa
 *title()	Converts the first character of each word to upper case
 *translate()	Returns a translated string
 *upper()	Converts a string into upper case
 *zfill()	Fills the string with a specified number of 0 values at the beginning

## list

Check if Item Exists
To determine if a specified item is present in a list use the in keyword:

thislist = ["apple", "banana", "cherry"]
if "apple" in thislist:
  print("Yes, 'apple' is in the fruits list")

  output: Yes, 'apple' is in the fruits list

  ## Remove Specified Item
The remove() method removes the specified item.

thislist = ["apple", "banana", "cherry"]
thislist.remove("banana")
print(thislist)

## Remove Specified Index
The pop() method removes the specified index.

thislist = ["apple", "banana", "cherry"]
thislist.pop(1)
print(thislist)


### Using a While Loop
You can loop through the list items by using a while loop.

Use the len() function to determine the length of the list, then start at 0 and loop your way through the list items by refering to their indexes.

Remember to increase the index by 1 after each iteration.

## list comprehension

people = "diana", "anne ", "carol", "Jne ", "kriuki"
newlist = []

for x in people:
    if "a" in x:
       newlist.append(x)
       
       print (newlist)

       output : diana , anne , carol


## sort

Sort List Alphanumerically
List objects have a sort() method that will sort the list alphanumerically, ascending, by default:

thislist = ["orange", "mango", "kiwi", "pineapple", "banana"]
thislist.sort()
print(thislist)

## List Methods
Python has a set of built-in methods that you can use on lists.

Method	Description
 *append()	Adds an element at the end of the list
 *clear()	Removes all the elements from the list
 *copy()	Returns a copy of the list
 *count()	Returns the number of elements with the specified value
 *extend()	Add the elements of a list (or any iterable), to the end of the current list
 *index()	Returns the index of the first element with the specified value
 *insert()	Adds an element at the specified position
 *pop()	Removes the element at the specified position
 *remove()	Removes the item with the specified value
 *reverse()	Reverses the order of the list
 *sort()	Sorts the list

## Tuple Methods
Python has two built-in methods that you can use on tuples.

Method	Description
count()	Returns the number of times a specified value occurs in a tuple
index()	Searches the tuple for a specified value and returns the position of where it was found

## Python If ... Else

Python supports the usual logical conditions from mathematics:

 *Equals: a == b
 *Not Equals: a != b
 *Less than: a < b
 *Less than or equal to: a <= b
 *Greater than: a > b
 *Greater than or equal to: a >= b

These conditions can be used in several ways, most commonly in "if statements" and loops.

An "if statement" is written by using the if keyword.

Indentation

Python relies on indentation (whitespace at the beginning of a line) to define scope in the code. Other programming languages often use curly-brackets for this purpose.

### Elif
The elif keyword is pythons way of saying "if the previous conditions were not true, then try this condition".

a = 33
b = 33
if b > a:
  print("b is greater than a")
elif a == b:
  print("a and b are equal")

### Else
The else keyword catches anything which isn't caught by the preceding conditions.

a = 200
b = 33
if b > a:
  print("b is greater than a")
elif a == b:
  print("a and b are equal")
else:
  print("a is greater than b")
 
## Python While Loops

Python has two primitive loop commands:

while loops
for loops
The while Loop
With the while loop we can execute a set of statements as long as a condition is true.

i = 1
while i < 6:
  print(i)
  i += 1


 ### The break Statement
With the break statement we can stop the loop even if the while condition is true:

Example
Exit the loop when i is 3:

i = 1
while i < 6:
  print(i)
  if i == 3:
    break
  i += 1 
  output:
  1
  2
  3

## Python For Loops

A for loop is used for iterating over a sequence (that is either a list, a tuple, a dictionary, a set, or a string).

With the for loop we can execute a set of statements, once for each item in a list, tuple, set etc.

## Python Functions

A function is a block of code which only runs when it is called.

You can pass data, known as parameters, into a function.

A function can return data as a result.

#### Creating a Function
In Python a function is defined using the def keyword:

def my_function():
  print("Hello from a function")

#### Calling a Function
To call a function, use the function name followed by parenthesis

def my_function():
  print("Hello from a function")

my_function()

## Arguments
Information can be passed into functions as arguments.

Arguments are specified after the function name, inside the parentheses. You can add as many arguments as you want, just separate them with a comma.

The following example has a function with one argument (fname). When the function is called, we pass along a first name, which is used inside the function to print the full name:

Example
def my_function(fname):
  print(fname + " Refsnes")

my_function("Emil")
my_function("Tobias")
my_function("Linus")


output:
Emil Refsnes
Tobias Refsnes
Linus Refsnes

## 
Arbitrary Arguments, *args
If you do not know how many arguments that will be passed into your function, add a * before the parameter name in the function definition.

This way the function will receive a tuple of arguments, and can access the items accordingly:

Example
If the number of arguments is unknown, add a * before the parameter name:

def my_function(*kids):
  print("The youngest child is " + kids[2])

my_function("Emil", "Tobias", "Linus")

output: The youngest child is linus

## Arbitrary Keyword Arguments, **kwargs
If you do not know how many keyword arguments that will be passed into your function, add two asterisk: ** before the parameter name in the function definition.

This way the function will receive a dictionary of arguments, and can access the items accordingly:

Example
If the number of keyword arguments is unknown, add a double ** before the parameter name:

def my_function(**kid):
  print("His last name is " + kid["lname"])

my_function(fname = "Tobias", lname = "Refsnes")

output: His last name is Refnes

### Python Classes and Objects

Python is an object oriented programming language.

Almost everything in Python is an object, with its properties and methods.

A Class is like an object constructor, or a "blueprint" for creating objects.

### Create a Class
To create a class, use the keyword class:

Create Object
Now we can use the class named MyClass to create objects:

Example
Create an object named p1, and print the value of x:

p1 = MyClass()
print(p1.x)


The __init__() Function


The examples above are classes and objects in their simplest form, and are not really useful in real life applications.

To understand the meaning of classes we have to understand the built-in __init__() function.

All classes have a function called __init__(), which is always executed when the class is being initiated.

Use the __init__() function to assign values to object properties, or other operations that are necessary to do when the object is being created:

Create a class named Person, use the __init__() function to assign values for name and age:

class Person:
  def __init__(self, name, age):
    self.name = name
    self.age = age

p1 = Person("John", 36)

print(p1.name)
print(p1.age)

Note: The __init__() function is called automatically every time the class is being used to create a new object.
 The self parameter is a reference to the current instance of the class, and is used to access variables that belong to the class.

### The self Parameter
The self parameter is a reference to the current instance of the class, and is used to access variables that belongs to the class.

It does not have to be named self , you can call it whatever you like, but it has to be the first parameter of any function in the class:

Example
Use the words mysillyobject and abc instead of self:

class Person:
  def __init__(mysillyobject, name, age):
    mysillyobject.name = name
    mysillyobject.age = age

  def myfunc(abc):
    print("Hello my name is " + abc.name)

p1 = Person("John", 36)
p1.myfunc()

## Python Inheritance

Inheritance allows us to define a class that inherits all the methods and properties from another class.

Parent class is the class being inherited from, also called base class.

Child class is the class that inherits from another class, also called derived class.

Create a Parent Class
Any class can be a parent class, so the syntax is the same as creating any other class:

Example
Create a class named Person, with firstname and lastname properties, and a printname method:

class Person:
  def __init__(self, fname, lname):
    self.firstname = fname
    self.lastname = lname

  def printname(self):
    print(self.firstname, self.lastname)

#Use the Person class to create an object, and then execute the printname method:

x = Person("John", "Doe")
x.printname()


### Python Iterators
Python Iterators
An iterator is an object that contains a countable number of values.

An iterator is an object that can be iterated upon, meaning that you can traverse through all the values.

Technically, in Python, an iterator is an object which implements the iterator protocol, which consist of the methods __iter__() and __next__().

## Python Dates
A date in Python is not a data type of its own, but we can import a module named datetime to work with dates as date objects.

Example
Import the datetime module and display the current date:

import datetime

x = datetime.datetime.now()
print(x)


### Return the year and name of weekday:

import datetime

x = datetime.datetime.now()

print(x.year)
print(x.strftime("%A"))


###  The strftime() Method
The datetime object has a method for formatting date objects into readable strings.

The method is called strftime(), and takes one parameter, format, to specify the format of the returned string:

Example
Display the name of the month:

import datetime

x = datetime.datetime(2018, 6, 1)

print(x.strftime("%B"))

 *%a	Weekday, short version	Wed	
 *%A	Weekday, full version	Wednesday	
 *%w	Weekday as a number 0-6, 0 is Sunday	3	
 *%d	Day of month 01-31	31	
 *%b	Month name, short version	Dec	
*%B	Month name, full version	December	
*%m	Month as a number 01-12	12	
*%y	Year, short version, without century	18	
*%Y	Year, full version	2018	
*%H	Hour 00-23	17	
*%I	Hour 00-12	05	
*%p	AM/PM	PM	
*%M	Minute 00-59	41	
*%S	Second 00-59	08	
*%f	Microsecond 000000-999999	548513	
*%z	UTC offset	+0100	
*%Z	Timezone	CST	
*%j	Day number of year 001-366	365	
*%U	Week number of year, Sunday as the first day of week, 00-53	52	
*%W	Week number of year, Monday as the first day of week, 00-53	52	
*%c	Local version of date and time	Mon Dec 31 17:41:00 2018	
*%C	Century	20	
*%x	Local version of date	12/31/18	
*%X	Local version of time	17:41:00	
*%%	A % character	%	
*%G	ISO 8601 year	2018	
*%u	ISO 8601 weekday (1-7)	1	
*%V	ISO 8601 weeknumber (01-53)	01	

### Built-in Math Functions
The min() and max() functions can be used to find the lowest or highest value in an iterable:

Example
x = min(5, 10, 25)
y = max(5, 10, 25)

print(x)
print(y)
The abs() function returns the absolute (positive) value of the specified number:

Example
x = abs(-7.25)

print(x)
The pow(x, y) function returns the value of x to the power of y (xy).

Example
Return the value of 4 to the power of 3 (same as 4 * 4 * 4):

x = pow(4, 3)

print(x)


# DJANGO FRAME WORK 

Django is a Python framework that makes it easier to create web sites using Python.

Django takes care of the difficult stuff so that you can concentrate on building your web applications.

Django emphasizes reusability of components, also refereed to as DRY (Don't Repeat Yourself), and comes with ready-to-use features like login system, database connection and CRUD operations (Create Read Update Delete).

Django is especially helpful for database driven websites.

## How does Django Work?
Django follows the MVT design pattern (Model View Template).

Model - The data you want to present, usually data from a database.
View - A request handler that returns the relevant template and content - based on the request from the user.
Template - A text file (like an HTML file) containing the layout of the web page, with logic on how to display the data.


## Model
The model provides data from the database.

In Django, the data is delivered as an Object Relational Mapping (ORM), which is a technique designed to make it easier to work with databases.

The most common way to extract data from a database is SQL. One problem with SQL is that you have to have a pretty good understanding of the database structure to be able to work with it.

Django, with ORM, makes it easier to communicate with the database, without having to write complex SQL statements.

The models are usually located in a file called models.py.

## View
A view is a function or method that takes http requests as arguments, imports the relevant model(s), and finds out what data to send to the template, and returns the final result.

The views are usually located in a file called views.py.

## Template
A template is a file where you describe how the result should be represented.

Templates are often .html files, with HTML code describing the layout of a web page, but it can also be in other file formats to present other results, but we will concentrate on .html files.

Django uses standard HTML to describe the layout, but uses Django tags to add logic:

<h1>My Homepage</h1>

<p>My name is {{ firstname }}.</p>
The templates of an application is located in a folder named templates.

## URLs
Django also provide a way to navigate around the different pages in a website.

When a user requests a URL, Django decides which view it will send it to.

This is done in a file called urls.py.


### 
When you have installed Django and created you first Django web application, and the browser requests the URL, this is basically what happens:

*Django receives the URL, checks the urls.py file, and calls the view that matches the URL.
*The view, located in views.py, checks for relevant models.
*The models are imported from the models.py file.
*The view then sends the data to a specified template in the template folder.
*The template contains HTML and Django tags, and with the data it returns finished HTML content back to the browser.
