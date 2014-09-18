# Selectors and Internal Style Sheets

We can achieve sensible styling nirvana by using a simple (but powerful) tool known as a *selector* (pay attention to this one — it's the tool at the heart of your CSS toolset).

Selectors work using one of the three specifications (or a combination there of): *elements*, *classes*, and *id's* (where the latter two are from attributes specified in `div` or `span` tags).

That was a mouthful! It'll be more obvious with an example, so here's one:

```html
<html>
    <head>
        <title>My Website</title>
        <style>
            h1 {color: red;}
        </style>
    </head>
    <body>
        <h1>This is a heading.</h1>
        <h1>This is a second heading.</h1>
    </body>
</html>
```

The result should look like this:

![](https://www.dropbox.com/s/4t124xlce5rmbon/Screenshot%202014-09-18%2000.46.33.png?dl=1)

Wow! All the `h1` tags are the color red! How did this happen?

In the `head` (which if you remember, stores the *metadata* for the site, which in this case, includes the definitions for styling of the page), there's a `style` tag which has a property for the `h1` element, where it's being styled as the color red.

There are three parts to defining a element's style:

```css
element-name {property_name: value;}
```

Different elements have different properties associated with them, but generally, styling follows that general format.

Let's add a third heading, this time in black. How would we do that?

One was is to put it in a `div` with a class name like "black", and define styles for that class. We're able to select a class much in the same way that we select elements, but class selectors are preceded with a '.' (and names are developer-defined.

They generally work in the form:

```css
.class-name {property_name: value;}
```

An example:

```html
<html>
    <head>
        <title>My Website</title>
        <style>
            h1 {color: red;}
            .black h1 {color: black;}
        </style>
    </head>
    <body>
        <h1>This is a heading.</h1>
        <h1>This is a second heading.</h1>
        <div class="black">
            <h1>This is a black heading.</h1>
        </div>
    </body>
</html>
```

You'll notice that the line defining styles for the third heading specifies multiple selectors. One way to visualize this is the following: "In the 'black' class, all `h1` elements follow the prescribed style.".

However, if making the third heading black was a one-off solution, we can actually write it even more cleanly. Think about it... think about it...

This is it:

```html
...
    .black {color: black;}
...
    <h1 class="black>This is a black heading.</h1>
...
```

However, because black is already the pre-defined default, perhaps it makes more sense to rewrite your file as so:

```html
<html>
    <head>
        <title>My Website</title>
        <style>
            .red {color: red;}
        </style>
    </head>
    <body>
        <div class="red">
            <h1>This is a heading.</h1>
            <h1>This is a second heading.</h1>
        </div>
        <h1>This is a black heading.</h1>
    </body>
</html>
```

That seems to make more logical sense and resolves to the same thing. You'll often find that this is the case. There are typically multiple non-obvious ways of achieving the same visual effect with CSS. You'll want to optimize for this using a couple of general guidelines:

1. Is this an intuitive solution? Will this make sense to other future developerd

2. DRY — where am I repeating/rewriting code where I can optimize it/structure it better?

If something feels like a poor way of doing something, it probably is. If it doesn't, it *may* be a good solution.

Go forth and take the previously written inline styles for your personal site and make it all-around more awesome, powerful, reusable and better.
