# External Style Sheets

Finally, we arrive at the *crème de la crème* of styling methods: external style sheets.

Fortunately for you, you've already learned 90% of what you need to know in order to make use of this technique!

External style sheets work almost exactly like internal style sheets — the only difference is that all the styling resides in an external *.css file (i.e.`styles.css`) and is linked to the HTML file from the `head` section with a `link` tag, in the form:

```html
<head>
    <link rel="stylesheet" type="text/css" href="your_css_file_name.css">
</head>
```

In order for this to work, the two files have to be in the same directory, but by specifying the destination, it can reside in a sub-directory. Try it!

If you were to do this for our previous example, this is what it'd look like —

In `index.html`:

```html
<html>
    <head>
        <title>My Website</title>
        <link rel="stylesheet" type="text/css" href="styles.css">
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

In `styles.css`:

```css
.red {color: red;}
```

That's it!

Writing your styles in an external style sheet is greatly beneficial because it adds more structure to your styling.

Moving forward, use this style for the most part. For pages where there is virtually no styling used, it may be tempting to just throw your styling inline, but from an organizational standpoint — this is far cleaner, and your brain will thank you for it.
