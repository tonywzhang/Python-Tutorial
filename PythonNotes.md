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



```

#Sets
