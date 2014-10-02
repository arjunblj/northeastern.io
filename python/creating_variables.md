# Creating Variables and Using Basic Operations

It's time to write your first bit of Python.

Type ```x = 5``` and hit return.

This statement *assigns* the value ```5``` to the variable ```x```. Try typing ```print x``` and hitting return. It will print out the value associated with x (```5```).

You can redefine x to be anything you want. Try repeating the steps above with ```x = 8```.

Now, let's try doing some basic math.
```python
>>> x = 2 + 2
```
This statement will evaluate the expression ```2 + 2``` and store the result in x. Print the value of x once again using ```print x``` and you should see 4.

Try some different operations like subtraction (```-```), multiplication (```*```), and division (```/```). Bonus points for checking out modulo (```%```), as well.

Another important idea to understand with variables, is that they can be used to assign *themselves* in Python. What the heck does that mean?

```python
>>> x = 1
>>> print x
1
>>> x = x + 1
>>> print x
2
```
The easy way to deal with this is remembering that the ```=``` operator does not mean both sides are mathematically equal, but rather that the value on the right is being assigned to the one on the left.

We promised this wouldn't just work with numbers, though.

```python
>>> friend = "Bob"
>>> print friend
"Bob"
```
We can do some operations on these as well, such as
```python
>>> greeting = "Hi, " + friend
>>> print greeting
"Hi, Bob"
```

We're getting ahead of ourselves though. Let's get a better idea of how we can store different types of information in variables, first, and then return to these ideas.
