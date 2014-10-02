# If Statements

>“It is our choices, Harry, that show what we truly are, far more than our abilities.”
― J.K. Rowling, Harry Potter and the Chamber of Secrets

Now that we've learned how to assign data to variables and perform some basic operations on that data, it's time for us to take this data and make decisions based on it. One of the core pieces of making decisions in python (and most programming languages) is the **if statement**.

```python
if condition:
    statement
```

##Condition
The **condition** of an if statement is the test we're putting on our data. Is some value x greater than 5? Is the given word the same as the word "dog"?

To ask these questions, we use **comparison operators**. Here's a table of some basic comparison operators.

| Operator | Use |
| -- | -- |
| < | less than |
| > | greater than |
| == | is equal to |
| != | is not equal to |
| and | both of these are true |
| or | one of these is true |

Note that we compare the equality of two things using ```==``` not ```=```. The single equals sign is for *assigning* a value to a variable. The double equals sign is for comparing two values (the mathematical understanding of the equals sign).

```python
name = "Bob"
if name == "Bob":
    print "Hi, Bob!"
```

The words ```and``` and ```or``` are used to combine these statements together. You can use parentheses to group comparisons together more cleanly.

```python
birthday = 5
name = "Bob"
if (name == "Bob") and (birthday == 5):
    print "Hi, Bob! Happy 5th birthday!"
```

###One more type

If we're going to talk about comparison we have to talk about one more type, **booleans**. Booleans are super simple because they can only have one of two values: ```True``` or ```False```. Comparing two values will give us back a boolean value.

```python
>>> pet = "dog"
>>> pet == "cat"
False
>>> pet == "dog"
True
```

In if statements, the statements after the condition will run only if the condition is true.

We can get the opposite value of a boolean value with the ```not``` operator.

```python
>>> x = 5
>>> x == 5
True
>>> not (x == 5)
False
```

##What else?

Using only ```if``` to make decisions can get troublesome as decisions become more complex. Most of the time, we'll want to specify not only what happens if something is true, but also if it is not.

We do this using ```elif``` and ```else```.

```python
x = 7

if x == 6:
    print "x is 6"
elif x > 6:
    print "x is greater than 6"
else:
    print "x is less than 6"
```

Take a second to sort out what will get printed here (ans: "x is greater than 6").

An important idea to note is that once one of the conditions is true. The rest don't matter at all.

```python
x = 7

if x == 7:
    print "x is 7"
elif x > 6:
    print "x is greater than 6"
else:
    print "x is something else"
```

This will only print "x is 7" even though the statement after is also true for x.

## Exercises
Having read these first few sections on Python, it's time to test your knowledge a bit.
###1
>Ask the user to input a number, and then print its value. For multiples of three, print “fizz” instead of the number, and for the multiples of five, print “buzz”. For numbers which are multiples of both three and five, print “fizzbuzz”.

Examples:
Entering 5 prints 'buzz'.
Entering 15 prints 'fizzbuzz'.
Entering 4 prints 4.

Hint: Use the modulo operator (%)

###2
>Ask the user to enter numbers for three variables, a, b, and c. Print the greatest value of those three numbers.

Example: If a = 5, b = 6, c = 7, print 7. If a = 4, b = 4, c = 0, print 4.




