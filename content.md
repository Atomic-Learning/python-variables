In Python, a variable is the name in source code used to refer to a storage location in the computer's memory which contains some form of data. We can create a variable by writing the name of the variable followed by an equals sign (`=`{.python}) and then the value we want to store in the memory location referenced by that variable. If we use the variable name later in our code, Python will use the value in the memory location it references. In the example below, we create a variable called `age`{.python} and assign it the value `25`{.python}. When we place a variable in the parentheses on a call to the `print`{.python} function the value of variable is returned. Here, printing the value of `age`{.python} outputs `25`{.python}.

```py-cell
age = 25
print(age)
```

# Variable Naming Rules

When naming variables in Python, there are a few important rules to follow:

* Variable names can only contain letters (a-z, A-Z), numbers (0-9), and underscores (_).
* Variable names cannot start with a number. For example, `1st_place`{.python} is not a valid variable name.
* Variable names are case-sensitive. This means that `age`{.python}, `Age`{.python}, and `AGE`{.python} are considered different variables.

In addition, variables may not use Python reserved words (keywords), as these have special meanings in the language. These keywords are:

* `and`{.python}
* `as`{.python}
* `assert`{.python}
* `async`{.python}
* `await`{.python}
* `break`{.python}
* `class`{.python}
* `continue`{.python}
* `def`{.python}
* `del`{.python}
* `elif`{.python}
* `else`{.python}
* `except`{.python}
* `False`{.python}
* `finally`{.python}
* `for`{.python}
* `from`{.python}
* `global`{.python}
* `if`{.python}
* `import`{.python}
* `in`{.python}
* `is`{.python}
* `lambda`{.python}
* `None`{.python}
* `nonlocal`{.python}
* `not`{.python}
* `or`{.python}
* `pass`{.python}
* `raise`{.python}
* `return`{.python}
* `True`{.python}
* `try`{.python}
* `while`{.python}
* `with`{.python}
* `yield`{.python}

# Variable Name Clashes

Although the prohibition of reserved words helps avoid some naming conflicts, it is still possible to accidentally overwrite important built-in functions or modules by using the same name for a variable. For example, if we create a variable called `print`{.python}, our variable will hide (or "shadow") the built-in `print`{.python} function, and we will no longer be able to use it until we delete our variable. For example, the code cell below shows what happens when we create a variable called `print`{.python} and then try to use the `print`{.python} function.

```py-cell
print = 5 # This creates a variable called 'print'
print(10) # This will cause an error
```

You should have seen an error message indicating that a `int`{.python} object is not callable. This is because Python is trying to call our variable `print`{.python} (which is an integer) as if it were a function, instead of the built-in `print`{.python} function. In order to fix this, reload the page and then proceed without re-running the code cell above.

To avoid such issues, it is a good practice to choose variable names that are unlikely to clash with built-in names.

# Variables and expressions

If the code on the right-hand side of the assignment operator is an expression, Python will first evaluate the expression and then assign the resulting value to the variable. For example, in the code below, we create a variable called `x`{.python} and assign it the result of the expression `5 + 3`{.python}. Python evaluates the expression to get `8`{.python}, and then assigns that value to `x`{.python}. When we print the value of `x`{.python}, Python outputs `8`{.python}.

```py-cell
x = 5 + 3
print(x)
# If you get an error, reload the page to get rid of the variable named print from the previous cell
```

# Changing Variable Values

We can change the value of a variable by assigning a new value to it. For example, in the code below, we first create a variable called `count`{.python} and assign it the value `10`{.python}. We then change the value of `count`{.python} to `20`{.python} by assigning a new value to it. When we print the value of `count`{.python}, Python outputs `20`{.python}.

```py-cell
count = 10
count = 20
print(count)
```
