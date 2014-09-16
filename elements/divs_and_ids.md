# Divs

Now we'll go over an element that is extremely prevalent and important in the HTML universe: `div`.

Divs are used to make separate sections to semantically organize your HTML code. This is extremely helpful later when grouping specific sections to be styled together with CSS.

Without any styling, divs don't serve any specific function but can be used to link to one part of a page from another.

Divs can take two attributes: `class` and `id`. They're both set in the form `<div class="class_name">` or `<div id="id_name">`. They are both to distinguish the name of the `div`.

From a [Stack Overflow answer](http://stackoverflow.com/questions/84378/div-class-vs-id) on the difference between `id` and `class`:

>Use `id` to identify elements that there will only be a single instance of on a page. For instance, if you have a single navigation bar that you are placing in a specific location, use `id="navigation"`.

>Use `class` to group elements that all behave a certain way. For instance, if you want your company name to appear in bold in body text, you might use `<div class='company'>`.

While there is a distinction between the two, I recommend sticking to `class` attributes for now with divs for the sake of consistency.

Here's an example of a small website using divs to check out:

```html
<html>
    <head>
        <title>My Website</title>

    </head>
    <body>
        <div class="header">This is a header</div>
        <div class="menu">
            <a href="homepage.html">Home</a><br>
            <a href="aboutpage.html">About</a><br>
            <a href="contactpage.html">Contact</a><br>
        </div>
        <div class="content">
            "Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum."
        </div>
        <div class="footer"></div>
    </body>
</html>
```

Small project: try using divs to make a sigle small web page. Add a lot of links to different page sections to see how to link them together.
