# Python Basic Notes

Most people use VSCode now for Python. Eclipse used to be another IDE that programmers used, but VSCode is very much universal.

```

Use the following annotation to define a multiline comment.

'''
This is a multiline
comment or docstring
can be in single or double quotes
'''

```

Variable Rules:

Variable Names are case sensitive (ex: name and NAME are two different variables)
Variables must start with a letter or an underscore
Variables can contain numbers, but cannot begin with one.

No need to write semi colons to end statements.
No need to declare variable type with the variable.

x = 1 is acceptable.

The system will determine and assign the type of variable.

```
Single Assignment

x = 1 (int)
y = 2.5 (float)
name = 'John' (string)
is_cool = True (boolean)

Multiple Assignment

x, y, name, is_cool = (1, 2.5, 'John', True)

Basic Math

a = x + y

print(x, y, name, is_cool, a) (a would be 3.5)

type(x) would return int.

Casting

Changing the Types of variables can be done as follows.

x = str(x)

print(type(x)) would return string.

```

# Strings

```
Strings in Python are surrounded by either single or double quotation marks.

name = 'Brad'
age = 37

# Concatenate

print('Hello, my name is ' + name + ' and I am ' + str(age) + ' years old')

# String Formatting

# Arguments by position

print('My name is {name} and I am {age}'.format(name = name, age = age))

# F Strings (Python Version 3.6+)

print(f'Hello, my name is {name} and I am {age}')

# String Methods

s = 'hello world'

# Capitalize Strings

print(s.capitalize())

print(s.upper()) #UpperCases String
print(s.lower()) #LowerCases String
print(s.swapcase()) #SwapCases String
print(len(s)) # Prints Length of String
print(s.replace('world', 'everyone'))

```

# Lists

Lists are very similar in concept to Arrays from JavaScript and other programming languages.

A List is a collection which is ordered and changeable that allows duplicate members.

```
# Create List

numbers = [1,2,3,4,5]

# Use a Constructor

numbers2 = list((1,2,3,4,5))

print(numbers, numbers2) would yield an equal list twice.

Using a constructor is unnecessary when you can simply declare the list like numbers above.

# Get a Value

Lists are 0-indexed, like arrays, so you can index into a list at a certain index.

numbers[1] would yield 2.

# Get Length

len(numbers) would yield 5

# Append to List

numbers.append(6)

6 would then be appended to the back of the list

# Insert into Position

numbers.insert(2, 3)

The first number represents the index to insert at, and the second argument represents the value to be inserted.

# Remove From List

numbers.remove(2)

# Remove with pop

numbers.pop(2)

# Reverse List

numbers.reverse()

# Sort List

numbers.sort()

# Reverse Sort

numbers.sort(reverse=True)

# Change Value

numbers[0] = '-1'
```

# Tuples

A Tuple is a collection which is ordered and unchangeable. It allows duplicate members.

```
# Create Tuples

fruits = ('Apples', 'Oranges', 'Grapes')
fruits2 = tuple(('Apples', 'Oranges', 'Grapes'))

print(fruits, fruits2) would return the same thing

If you initialize a tuple with one value, that value still needs to be followed by a comma. IE:

fruits = ('Apples',)

# Get Value

fruits[1]

# You cannot change a value at a specific index for tuple

fruits[0] = 'Pears' would throw an error, unable to re-assign items

# Delete Tuples

del fruits2, fruits2 becomes undefined

# Length of a Tuple

print(len(fruits))

```

#Sets

A Set is a collection which is unordered and unindexed. No duplicate members are allowed. Very similar to that of a Set from JavaScript.

```
# Create Set

fruits_set = {'Apples', 'Oranges', 'Mango'}

# Check if in Set

'Apples' in fruits_set will return a boolean, in this case True

# Add to Set

fruits_set.add('Grape')

# Remove from set

fruits_set.remove('Grape')

# Clear Set Entirely

fruits_set.clear()

# Delete Set

del fruits_set leaves fruits_set as undefined

```

# Dictionaries

Dictionaries are very similar to Maps in JavaScript. They correspond to an unordered collection, changeable and indexed. No Duplicate members.

```
# Create Dictionary

person = {
  'first_name': 'John',
  'last_name': 'Doe',
  'age': 30  
}

# Get Value

person['first_name'] OR person.get('first_name') both work

# Adding a Key Value Pair

person['phone'] = '123-456-7890'

This will add the key 'phone' with a corresponding phone number inputted as a string.

# Get Dictionary Keys

person.keys() will return all of the keys in our dictionary

# Get Dictionary Items

person.items() will return all of the values in our dictionary

# Copy Dictionary

person2 = person.copy()

this will make a copy of the person

# Remove Item

del(person['age'])
person.pop('phone')

# Clear

person.clear() yields an empty dictionary

# Get Length

len(person)
```

# Functions

A function is a block of code which only runs when it is called or invoked. In Python, we do not use curly brackets, we use indentation with tabs or spaces.

```
# Create Function

def sayHello(name):
  print(f'Hello {name}')


sayHello('John Doe')

This will return 'Hello John Doe' as expected.

If you want to call on sayHello with no argument, we'll need to set a default value to "name" in the function declaration such as "name = 'sam'" or something of the like.

# Return Values

def getSum(num1, num2):
  total = num1 + num2
  return total

getSum(3,4) returns 7 as expected.

# A lambda function is a small anonymous function

# A lambda function can take any number of arguments, but only have one expression. Very similar to JS arrow functions

getSum = lambda num1,num2 : return num1 + num2

getSum(10,3) returns 13 as expected

```
