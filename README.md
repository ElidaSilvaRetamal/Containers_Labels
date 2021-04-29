# Containers_Labels
Test Hypotheses - Are Variables Containers? Or Are They Labels?

# 1 - Integer (int)
 
# Creating the int
x = 25  # x is a label and 25 is a object / variables are labels which can be attached to objects in memory.
​
# Creating a second variable int equal to the first
y = x  # y is a label and x is a object and so object and label are value.
​
# Printing
print(x, y)
print(id(x))
print(id(y))
print( "x and y are actually referring to the same object 25 \n")
​
# Changing the second int variable
x = [10, 20, 30]  # here we are building a new object for x
​
print(f'value of x: {x} ID of x: {id(x)}')
print(f'value of x[0]: {x[0]} ID of x: {id(x[0])}')
print(f'value of x[1]: {x[1]} ID of x: {id(x[1])}')
print(f'value of x[2]: {x[2]} ID of x: {id(x[2])}')
print("x is referring to the different object ")
25 25
140707926573344
140707926573344
x and y are actually referring to the same object 25 

value of x: [10, 20, 30] ID of x: 1653950142792
value of x[0]: 10 ID of x: 140707926572864
value of x[1]: 20 ID of x: 140707926573184
value of x[2]: 30 ID of x: 140707926573504
x is referring to the different object 
# 2 - Float
x = 25.25
y = x
​
print(id(x))
print(id(y))
​
x = [10.2 , 20.3 , 30.25]
print(f'value of x: {x} ID of x: {id(x)}') 
1653949927664
1653949927664
value of x: [10.2, 20.3, 30.25] ID of x: 1653950142792
# 3 - String
a = "name"
b = a
​
print(id(a))
print(id(b))
​
b = ["Mary"," Paty", "Ale"]
print(f' value of b: {b} ID of b: {id(b)}')
1653877697144
1653877697144
 value of b: ['Mary', ' Paty', 'Ale'] ID of b: 1653950107208
# 4 - List
# Printing
print(f"Value of List1: {List1} ID of List1: {id(List1)}")
print(f"Value of List2: {List2} ID of List2: {id(List2)}")
print(f"Value of List2[1]: {List2[1]} ID of List2[1]: {id(List2[1])}")
​
# Creating the List
List1 =  [1, 5.2, 9, 12, 24, 33]
​
# Creating a second variable List equal to the first
List2 = List1 
​
# Printing
print(id(List1))
print(id(List2))
​
# Changing the second List variable
List2 = [1968,"car","model" ]
​
# Printing
print(f"Value of List1: {List1} ID of List1: {id(List1)}")
print(f"Value of List2: {List2} ID of List2: {id(List2)}")
print(f"Value of List2[1]: {List2[1]} ID of List2[1]: {id(List2[1])}")
1653950141320
1653950141320
Value of List1: [1, 5.2, 9, 12, 24, 33] ID of List1: 1653950141320
Value of List2: [1968, 'car', 'model'] ID of List2: 1653950104392
Value of List2[1]: car ID of List2[1]: 1653951023680
# 5 - Tuple
# Creating a variable tuple
tuple1 = (57, "birthday", 1964, "weight",[1965, 1964, 1963])
​
# Creating a second variable tuple equal to the first
tuple2 = tuple1
​
# printing
print(id(tuple1))
print(id(tuple2))
​
print ('Tuple is immutable variable')
​
# 1.3) Changing the second variable
tuple2[3] = 89
1653950826544
1653950826544
Tuple is immutable variable
---------------------------------------------------------------------------
TypeError                                 Traceback (most recent call last)
<ipython-input-13-9e37bd2c5e07> in <module>
     12 
     13 # 1.3) Changing the second variable
---> 14 tuple2[3] = 89

TypeError: 'tuple' object does not support item assignment

tuple
# Creating a variable tuple
tuple1 = (57, "birthday", 1964, "weight",[1965, 1964, 1963])
​
# Creating a second variable tuple equal to the first
tuple2 = tuple1
​
# printing
print(id(tuple1))
print(id(tuple2))
​
print ('Tuple is immutable variable')
​
# 1.3) Changing the second variable
tuple2 = (2.0, "name", "whatever")
print(f"Value of tupl2[1]: {tuple2[1]} ID of tuple2[1]: {id(tuple2[1])}")
1653950826544
1653950826544
Tuple is immutable variable
Value of tupl2[1]: name ID of tuple2[1]: 1653877697144

# 6 - Dictionary
# Creating the dictionary
Dict1 = {"key1": 1, "key2": "2", "key3": [3, 3, 3], "key4": "quatro"}

# Creating a second variable dictionay equal to the first
Dict2 = Dict1

# Printing
print(id(Dict1))
print(id(Dict2))

# Changing the second dictionay variable
Dict2["key1"] = "new value" # here we are building a new object. Append value with key into dictionary

print(f'Value of Dict2["key1"]: {Dict2["key1"]} ID of Dict2["key1"]: {id(Dict2["key1"])}')
# Creating the dictionary
Dict1 = {"key1": 1, "key2": "2", "key3": [3, 3, 3], "key4": "quatro"}
​
# Creating a second variable dictionay equal to the first
Dict2 = Dict1
​
# Printing
print(id(Dict1))
print(id(Dict2))
​
# Changing the second dictionay variable
Dict2["key1"] = "new value" # here we are building a new object. Append value with key into dictionary
​
print(f'Value of Dict2["key1"]: {Dict2["key1"]} ID of Dict2["key1"]: {id(Dict2["key1"])}')
1653951833936
1653951833936
Value of Dict2["key1"]: new value ID of Dict2["key1"]: 1653951031344
Conclusion:
Python is a programming language that supports OOP. The variables are labels which can be attached to objects in memory, wherever they are.

​
