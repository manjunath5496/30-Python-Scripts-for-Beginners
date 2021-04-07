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
