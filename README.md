# 30 Python Scripts for Beginners

### **01. Hello World:**

---------------------------------------


```python
# The following python script will print the text "Hello World!" as output.

print("Hello World!")
```
----------------------------------------
### **02. Join two strings:**

---------------------------------------


```python
# Two words "Programming" and "Languages" are joined and "ProgrammingLanguages" is printed as output.


x = "Programming"
y = "Languages"
z = x + y
print(z)
```
----------------------------------------
### **03. Format floating point in the string:**

---------------------------------------


```python
# Use of String Formatting
x = 462.75897
print("{:5.2f}".format(x))

# Use of String Interpolation
y = 462.75897
print("%5.2f" % y)
```
----------------------------------------

### **04. Raise a number to a power:**

---------------------------------------


```python
import math
# Assign values to a and n
a = 4
n = 3

# Method 1
b = a ** n
print("%d to the power %d is %d" % (a,n,b))

# Method 2
b = pow(a,n)
print("%d to the power %d is %d" % (a,n,b))

# Method 3
b = math.pow(a,n)
print("%d to the power %d is %5.2f" % (a,n,b))
```
----------------------------------------
### **05. Working with Boolean types:**

---------------------------------------


```python
# Boolean value
x = True
print(x)

# Number to Boolean
x = 10
print(bool(x))

x = -5
print(bool(x))

x = 0
print(bool(x))

# Boolean from comparison operator
x = 6
y = 3
print(x < y)
```
----------------------------------------
### **06. If else statement:**

---------------------------------------


```python
# Assign a numeric value
x = 35

# Check the is more than 35 or not
if (x >= 35):
    print("You have passed")
else:
    print("You have not passed")
```
----------------------------------------
### **07. Using AND and OR operators:**

---------------------------------------


```python
# Take practical marks
x = float(input("Enter the Practical marks: "))
# Take theory marks
y = float(input("Enter the Theory marks: "))

# Check the passing condition using AND and OR operator
if (x >= 25 and y >= 45) or (x + y) >=70:
    print("\nYou have passed")
else:
    print("\nYou have failed")
```
----------------------------------------
### **08. Switch case statement:**

---------------------------------------


```python
# Switcher for implementing switch case options
def employee_details(ID):
    switcher = {
        "5006": "Employee Name: John",
        "5008": "Employee Name: Ram",  
        "5010": "Employee Name: Mohamend",
    }
    '''The first argument will be returned if the match found and
        employee ID does not exist will be returned if no match found'''
    return switcher.get(ID, "employee ID does not exist")

# Take the employee ID
ID = input("Enter the employee ID: ")
# Print the output
print(employee_details(ID))
```
----------------------------------------
### **09. While Loop:**

---------------------------------------


```python
# Initialize counter
counter = 1
# Iterate the loop 9 times
while counter < 10:
    # Print the counter value
    print ("%d" % counter)
    # Increment the counter
    counter = counter + 1
```
----------------------------------------
### **11. Use of command-line argument:**

---------------------------------------


```python
# Import sys module
import sys

# Total number of arguments
print('Total arguments:', len(sys.argv))

print("Argument values are:")
# Iterate command-line arguments using for loop
for i in sys.argv:
  print(i)
```
----------------------------------------
### **12. Run one Python script from another:**

---------------------------------------
```python
#  Hello.py

print("Hello World!")
```

```python
#  Executes the hello.py file in the interpreter

import os
os.system('hello.py')
```
----------------------------------------
### **13. Use of regex:**

---------------------------------------


```python
# Import re module
import re

# Take any string data
string = input("Enter a string value: ")
# Define the searching pattern
pattern = '^[A-Z]'

# match the pattern with input value
found = re.match(pattern, string)

# Print message based on the return value
if found:
  print("The input value is started with the capital letter")
else:
  print("You have to type string start with the capital letter")
```
----------------------------------------
### **14. Use of getpass:**

---------------------------------------


```python
# import getpass module
import getpass

# Take password from the user
passwd = getpass.getpass('Password:')

# Check the password
if passwd == "python":
    print("You are verified")
else:
    print("You are not verified")
```
----------------------------------------
### **15. Use of date format:**

---------------------------------------


```python
from datetime import date

# Read the current date
current_date = date.today()

# Print the formatted date
print("Today is :%d-%d-%d" % (current_date.day,current_date.month,current_date.year))

# Set the custom date
custom_date = date(2026, 12, 26)
print("The date is:",custom_date)
```
----------------------------------------
### **16. Add and remove the item from a list:**

---------------------------------------


```python
# Declare a fruit list
fruits = ["Mango","Orange","Guava","Banana"]

# Insert an item in the 2nd position
fruits.insert(1, "Apple")

# Displaying list after inserting
print("The fruit list after insert:")
print(fruits)
 
# Remove an item
fruits.remove("Banana")

# Print the list after delete
print("The fruit list after delete:")
print(fruits)
```
----------------------------------------
### **17. List comprehension:**

---------------------------------------


```python

# Create a list of characters using list comprehension
char_list = [ char for char in "Python" ]
print(char_list)

# Define a tuple of websites
websites = ("google.com","yahoo.com", "history.com", "quora.com")

# Create a list from tuple using list comprehension
site_list = [ site for site in websites ]
print(site_list)
```
----------------------------------------
### **18. Slice data:**

---------------------------------------


```python

# Assign string value
text = "Python Programming Language"

# Slice using one parameter
sliceObj = slice(5)
print(text[sliceObj])  

# Slice using two parameter
sliceObj = slice(6,12)
print(text[sliceObj])  

# Slice using three parameter
sliceObj = slice(6,25,5)
print(text[sliceObj])

```
----------------------------------------
### **19. Add and search data in the dictionary:**

---------------------------------------


```python

# Define a dictionary
customers = {'05453':'Ram','04457':'Krishna',
'02834':'Vishnu','01655':'Shiva', '07559':'David'}

# Append a new data
customers['06934'] = 'Salomon'

print("The customer names are:")
# Print the values of the dictionary
for customer in customers:
    print(customers[customer])

# Take customer ID as input to search
name = input("Enter customer ID:")

# Search the ID in the dictionary
for customer in customers:
    if customer == name:
        print(customers[customer])
        break



```
----------------------------------------
### **20. Add and search data in the set:**

---------------------------------------


```python


# Define the number set
numbers = {13, 10, 56, 18, 12, 44, 87}
 
# Add a new data
numbers.add(63)
# Print the set values
print(numbers)

message = "Number is not found"

# Take a number value for search
search_number = int(input("Enter a number:"))
# Search the number in the set
for val in numbers:
    if val == search_number:
        message = "Number is found"
        break

print(message)



```
----------------------------------------
### **21. Count items in the list:**

---------------------------------------


```python


# Define the string
string = 'Python Go JavaScript HTML CSS MYSQL Python'
# Define the search string
search = 'Python'
# Store the count value
count = string.count(search)
# Print the formatted output
print("%s appears %d times" % (search, count))



```
----------------------------------------
### **22. Define and call a function:**

---------------------------------------


```python

# Define addition function
def addition(number1, number2):
    result = number1 + number2
    print("Addition result:",result)

# Define area function with return statement
def area(radius):
    result = 3.14 * radius * radius
    return result  

# Call addition function
addition(5, 3)
# Call area function
print("Area of the circle is",area(2))



```
----------------------------------------
### **23. Use of throw and catch exception:**

---------------------------------------


```python


# Try block
try:
    # Take a number
    number = int(input("Enter a number: "))
    if number % 2 == 0:
        print("Number is even")
    else:
        print("Number is odd")

# Exception block    
except (ValueError):
  # Print error message
  print("Enter a numeric value")


```
----------------------------------------
### **24. Read and Write File:**

---------------------------------------


```python

#Assign the filename
filename = "names.txt"
# Open file for writing
fileHandler = open(filename, "w")

# Add some text
fileHandler.write("Ram\n")
fileHandler.write("John\n")
fileHandler.write("David\n")

# Close the file
fileHandler.close()

# Open file for reading
fileHandler = open(filename, "r")

# Read a file line by line
for line in fileHandler:
  print(line)
 
# Close the file
fileHandler.close()

```
----------------------------------------
### **25. List files in a directory:**

---------------------------------------


```python

# Import os module to read directory
import os

# Set the directory path
path = '/Users/Manju/'

# Read the content of the file
files = os.listdir(path)

# Print the content of the directory
for file in files:
    print(file)

```
----------------------------------------
### **26. Read and write using pickle:**

---------------------------------------


```python


# Import pickle module
import pickle

# Declare the object to store data
dataObject = []
# Iterate the for loop for 5 times
for num in range(10,15):
   dataObject.append(num)

# Open a file for writing data
file_handler = open('numbers', 'wb')
# Dump the data of the object into the file
pickle.dump(dataObject, file_handler)
# close the file handler
file_handler.close()

# Open a file for reading the file
file_handler = open('numbers', 'rb')
# Load the data from the file after deserialization
dataObject = pickle.load(file_handler)
# Iterate the loop to print the data
for val in dataObject:
  print(val)
# close the file handler
file_handler.close()


```
----------------------------------------
### **27. Define class and method:**

---------------------------------------


```python


# Define the class
class Employee:
    name = "Johnson"
    # Define the method
    def details(self):
        print("Post: Associate")
        print("Department: QC")
        print("Salary: $6000")

# Create the employee object    
emp = Employee()
# Print the class variable
print("Name:",emp.name)
# Call the class method
emp.details()

```
----------------------------------------
### **28. Use of range function:**

---------------------------------------


```python

# range() with one parameter
for val in range(7):
    print(val, end='  ')
print('\n')

# range() with two parameter
for val in range(7,16):
    print(val, end='  ')
print('\n')

# range() with three parameter
for val in range(0,4,1):
    print(val, end='  ')


```
----------------------------------------
### **29. Use of map function:**

---------------------------------------


```python

# Define the function to calculate power
def cal_power(n):    
    return x ** n

# Take the value of x
x = int(input("Enter the value of x:"))
# Define a tuple of numbers
numbers = [2, 6, 3]

# Calculate the x to the power n using map()
result = map(cal_power, numbers)
print(list(result))

```
----------------------------------------
