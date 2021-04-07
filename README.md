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
