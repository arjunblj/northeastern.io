 # Input and Output
## Output

We output information in Python using the **print** statement, which you've already seen a bit.

```python
>>> x = 11
>>> print x
11
```
There's more to print than just outputing simple variables, though.

### Formatting
Let's say we wanted to provide more information about what is being printed.

```python
>>> print "The value in x is %d" % x
The value in x is 11
```

This is called **string formatting**. That *%d* is a placeholder for where we want our value to go. The *d* in *%d * stands for "decimal" and is used to let Python know that we want the value after the *%* at the end of the line to be output as a standard decimal number. We could have just as easily printed this value in another format, like hexidecimal.

```python
>>> print "The value in x is %x" % x
The value in x is b
```

While I can't imagine you'll be printing out hexidecimal values very often, you will using this formatting to work with the two types we discussed in the last section: integers and strings.

We've already learned how to output integers using %d. The idea is the same for strings, only they use %s instead.

```python
>>> y = "dog"
>>> print "I have a pet %s" % y
I have a pet dog
```
String formatting can be used to print multiple values as well.

```python
>>> print "I have a pet %s and he is %d." % (y, x)
I have a pet dog and he is 11.
```

We group the variables we want to print in the order in which they appear, using parentheses, and separated by commas.

As you might have guessed, string formatting isn't just for print. We can store formatted values in strings.

```python
>>> sentence = "I have a pet %s and he is %d" % (y, x)
>>> print sentence
I have a pet dog and he is 11.
```

For additional info on string formatting, the [Python String Format Cookbook](http://mkaz.com/2012/10/10/python-string-format/) is a great resource.

### Special characters

Even with all of this formatting, sometimes all of the alphanumerical characters aren't enough to convey an idea you have in text. Python has a bunch of **special characters** to store and print concepts you can't place between two quotes.

For example, ```\n``` produces a return, or **n**ewline, where it is inserted.
```python
>>> print "This is on one line.\nThis is on another."
This is on one line.
This is on another.
```
Similarly, ```\t``` produces a tab.

```python
>>> print "I am here\tAnd I am over here"
I am here	And I am over here
```
For a more comprehensive list of special characters, check out [this page](https://docs.python.org/2.0/ref/strings.html) of the python documentation.

## Input

Printing out information is nice, but it's only polite for us to give the user a voice as well. To prompt for input in Python, use the ```raw_input``` function. Here's a simple program to ask for a user's name and print out a greeting:

```python
# greeting.py

name = raw_input("What is your name? ")
print "Hello, %s!" % name
```
Running this program should produce the following. Try it for yourself!
```
$ python greeting.py
What is your name? Luke
Hello, Luke!
```

