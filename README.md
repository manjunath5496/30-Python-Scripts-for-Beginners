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
