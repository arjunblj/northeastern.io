# Inline Styles

Now that you know what CSS is used for, we're going to go ahead and cover *how it's implemented* and the different dimensions you can style given HTML code.

There are three ways that you can implement styling using CSS for a given HTML page:

1. Inline styles

2. Internal style sheets

3. External style sheets

While the third option is overwhelmingly preferred by most web developers in the world (you'll realize why soon enough), we'll briefly cover the uses of inline styles and internal style sheets, using them as stepping stones to using external style sheets.

Inline styles are the most basic way of styling a given HTML page. A brief example, a slightly styled version of the first page you built:

```html
<html>
    <head>
        <title>
            My Website
        </title>
    </head>
    <body>
        <h1 style="color:red; margin-left:30px;">This is a heading.</h1>
    </body>
</html>
```

The output should look like this:

![](https://www.dropbox.com/s/97d6kemq67reuon/Screenshot%202014-09-17%2023.32.59.png?dl=1)

What just happened?

With a little pattern matching, you should have identified that the big difference is an *attribute* (vocab word!) in the `h1` element called `style` which has two *properties*, `color` and `margin-left` with the values you see above.

Styling a HTML page works on a very elemental level. As a simplified, high-level explanation: when a browser interprets the coded version of your page, it's going throug and rendering each tag (in order) and also checking to see if there is any associated styling attached to a specific tag (which it also does in order, as we'll see later).

In this case, when the browser hit the `h1` tag, it also caught the `style` attribute, which needed to be rendered (in the same way the browser would render the heading as a link given an `a` attribute). It then renders the associated styles, of which two were specified.

Here are a few other examples — play around with different properties of the specified styles. Some "gimme" dimensions to experiment with: color (look up hexadecimal colors), margins, etc.

```html
<p style="background:blue; color:white;">A new background and font color with inline CSS</p>
```

```html
<div style="width:20px; height:20px; background-color:#ffcc00;"></div>
```

Play around with styling your page with inline styles, though you'll soon realize the inefficiency of doing so. ;-)
