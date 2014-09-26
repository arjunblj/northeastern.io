# Type

Oddly enough, the many types of data are called **data types**. Each type is suited for holding a different kind of information.

While, Python handles the issue of assigning each variable a type for us, we still have to be aware of a variable's type because it governs how we treat that variable and what that variable can do.

There are hundreds of types, but we'll discuss only two of the most common/useful for now.

## Integer
An integer, or **int**, represents some whole numerical value. ```5``` is an int.```-20``` is an int. ```2.7``` is not an int. When we wrote ```x = 5``` for the first time, we created a variable named ```x```, and based on the value we gave it (```5```), python made ```x``` an integer. We can verify that by running ```type(x)```. This should tell us x is ```<type 'int'>```.

Integers can be added, subtracted, etc, just as you would expect, but, remember, they can only store *whole numbers*. This can cause some trouble if you're not paying attention. For example, running ```x = 5/2``` will assign ```x``` the value ```2```, not ```2.5```.

## String
A **string** represents a set of characters. ```"Bob"``` is a string. ```5``` is not a string. ```"5"``` is a string. Did you notice the subtle different there? The quotes around the information tell python that this variable is a string and should be treated as such. We can append strings together using the ```+``` operator (as you saw on the last page).
```python
>>> animals = "Cats" + " and " + "Dogs"
>>> print animals
"Cats and Dogs"
```
We can verify this type at well
```python
>>> type(animals)
<type 'str'>
```
