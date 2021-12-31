# To learn Telethon You need to learn Basic Python.

## Installation
### [`Install Python`](https://www.python.org/downloads/)

## Python Keywords
Keywords are the reserved words in Python.
We cannot use a keyword as a variable name, function name or any other identifier. They are used to define the syntax and structure of the Python language.

In Python, keywords are case sensitive.

There are 33 keywords in Python 3.7. This number can vary slightly over the course of time.

All the keywords except `True`, `False` and `None` are in lowercase and they must be written as they are. The list of all the keywords is given below.

| First | Second | Third | Fourth | Fifth |
| :---         |     :---:      |     :---:      |     :---:      |          ---: |
| False | await     | else    | import    |pass     |
| None     | break       | except      | in    | raise    |
| True | class     | finally    | is    | return    |
| and     | continue       | for      | lambda    | try    |
| as      | def     | from    | nonlocal   | while    |
| assert     | del       | global      | not   | with    |
| async | elif     | if    | or    | yield    |

## Python Identifiers
An identifier is a name given to entities like class, functions, variables, etc. It helps to differentiate one entity from another.
### Rules for writing identifiers
- Identifiers can be a combination of letters in lowercase (a to z) or uppercase (A to Z) or digits (0 to 9) or an underscore `_`. Names like `myClass`, `var_1` and `print_this_to_screen`, all are valid example.
- An identifier cannot start with a digit. `1variable` is invalid, but `variable1` is a valid name.
- Keywords cannot be used as identifiers. like `global = 1`.
- We cannot use special symbols like `!, @, #, $, %` etc. in our identifier.

## Things to Remember
Python is a case-sensitive language. This means, Variable and variable are not the same.

Always give the identifiers a name that makes sense. While c = 10 is a valid name, writing count = 10 would make more sense, and it would be easier to figure out what it represents when you look at your code after a long gap.

Multiple words can be separated using an underscore, like `this_is_a_long_variable`.

## Python Statement
Instructions that a Python interpreter can execute are called statements. For example, a = 1 is an assignment statement. if statement, for statement, while statement, etc. are other kinds of statements which will be discussed later.

### Multi-line statement
In Python, the end of a statement is marked by a newline character. But we can make a statement extend over multiple lines with the line continuation character (\).
Example

```
a = 1 + 2 + 3 + \
    4 + 5 + 6 + \
    7 + 8 + 9
```
This is an explicit line continuation. In Python, line continuation is implied inside parentheses `( )`, brackets `[ ]`, and braces `{ }`. For instance, we can implement the above multi-line statement as:

```
a = (1 + 2 + 3 +
    4 + 5 + 6 +
    7 + 8 + 9)
```
Here, the surrounding parentheses `( )` do the line continuation implicitly. Same is the case with `[ ]` and `{ }`. For example:

```
colors = ['red',
          'blue',
          'green']
```
We can also put multiple statements in a single line using semicolons, as follows:

```
a = 1; b = 2; c = 3
```

## Python Indentation
Most of the programming languages like C, C++, and Java use braces `{ }` to define a block of code. Python, however, uses indentation.

A code block (body of a function, loop, etc.) starts with indentation and ends with the first unindented line. The amount of indentation is up to you, but it must be consistent throughout that block.

Generally, four whitespaces are used for indentation and are preferred over tabs. Here is an example.
```
for i in range(1,11):
    print(i)
    if i == 5:
        break
```

The enforcement of indentation in Python makes the code look neat and clean. This results in Python programs that look similar and consistent.

Indentation can be ignored in line continuation, but it's always a good idea to indent. It makes the code more readable. For example:

```
if True:
    print('Hello')
    a = 5
```
and
```
if True: print('Hello'); a = 5
```
both are valid and do the same thing, but the former style is clearer.
incorrect indentation will result in `IndentationError`.

## Docstrings in Python
A docstring is short for documentation string.

Python docstrings (documentation strings) are the string literals that appear right after the definition of a function, method, class, or module.

Triple quotes are used while writing docstrings. For example:
```
def double(num):
    """Function to double the value"""
    return 2*num
```
Docstrings appear right after the definition of a function, class, or a module. This separates docstrings from multiline comments using triple quotes.

The docstrings are associated with the object as their __doc__ attribute.

So, we can access the docstrings of the above function with the following lines of code:
```
def double(num):
    """Function to double the value"""
    return 2*num
print(double.__doc__)
```
### Output

```Function to double the value```

## Python Comments
Comments are very important while writing a program. They describe what is going on inside a program, so that a person looking at the source code does not have a hard time figuring it out.

You might forget the key details of the program you just wrote in a month's time. So taking the time to explain these concepts in the form of comments is always fruitful.

In Python, we use the hash (`#`) symbol to start writing a comment.

It extends up to the newline character. Comments are for programmers to better understand a program. Python Interpreter ignores comments.

```#This is a comment
#print out Hello
print('Hello')
Multi-line comments```
We can have comments that extend up to multiple lines. One way is to use the hash(#) symbol at the beginning of each line. For example:

```#This is a long comment
#and it extends
#to multiple lines
Another way of doing this is to use triple quotes, either ''' or """.
```
These triple quotes are generally used for multi-line strings. But they can be used as a multi-line comment as well. Unless they are not docstrings, they do not generate any extra code.
```
"""This is also a
perfect example of
multi-line comments"""
```


