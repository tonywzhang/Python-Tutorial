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
