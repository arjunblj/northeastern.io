# Internal and External Style Sheets

If you started styling your personal web page with inline styles, you would have soon started to see the ineffeciency of doing so. Inherently, inline styles don't lend themselves to reusability, violating one of the fundamental principles of writing good, clean code: [DRY](http://en.wikipedia.org/wiki/Don't_repeat_yourself) (Don't repeat yourself.).

In case you didn't have a chance to see that at work, here's a simple example based on the example in *2.1*:

```html
<html>
    <head>
        <title>
            My Website
        </title>
    </head>
    <body>
        <h1 style="color:red; margin-left:30px;">This is a heading.</h1>
        <h1>This is a second heading.</h1>
    </body>
</html>
```

For the lazy, it should look like this:

![](https://www.dropbox.com/s/oxw4yb2lugs78qq/Screenshot%202014-09-18%2000.07.39.png?dl=1)

But Arjun! I want my second heading to be colorful and pretty like my first one!

Unfortunately, the "cleanest" way to do that with inline styles would be to do something like this:

```html
<h1 style="color:red; margin-left:30px;">This is a heading.</h1>
<h1 style="color:red; margin-left:30px;">This is a second heading.</h1>
```

But Arjun! Doesn't that violate DRY?! Why would we write that attrocity?!

Yes, yes it does. It's not just that it's bad because we're repeating code. Imagine you want to change something simple, like the color of all your headings (let's make them blue!). If you had hundreds of headings on the page, you'd have to go through and replace them all. Find + Replace All makes that relatively trivial, but you're better than that.

What if we had a way to style all the `h1` elements together?

Welcome to the magic of style sheets.
