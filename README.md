# Northeastern.io HTML and CSS

Hi! Welcome to Northeastern.io. Hopefully over the course of the semester, we (Arjun and Luke) will get you from 0 to *n*, where *n* is a slightly more-technical, more-awesome version of yourself.

Whether you just want to build a simple personal site or want to build more complex web applications, we can help you get there over the course of the semester.

One of the things






## Hello World!

We're going to start by getting you set up with a text editor. While Notepad will do, I highly recommend getting an editor called [Sublime Text](http://www.sublimetext.com/) — while their site may seem intimidating, the editor itself is actually quite simple to use, loaded with several helpful features for beginners.

Most introductory programming resources start with a "Hello world!" example. While what you're about to do may not make sense immediately off the bat, rest assured that in twenty minutes, it'll all click. :)

Start by opening up Sublime and creating a file called `hello.html`.

In it, paste the following:

```html
<html>
    <head>
        <title>
            My Website
        </title>
    </head>
    <body>
        <h1>Hello, World!</h1>
    </body>
</html>
```

After saving it, go ahead and try opening the file in your browser of choice.

It should look something like this:

![](https://www.dropbox.com/s/9vkwl0os2287w43/Screenshot%202014-09-10%2021.41.34.png?dl=1)

If it does, congrats! You just made your very first web page.

We'll break down that code in a few sweet minutes.

## Terms

So what did that code actually do? Visibly, the "title" of the page (visible in the browser tab) was set to "My Website" and there was text on the page that appeared.

In order to fully understand there's a few (only a few, I promise) terms you're going to have to know so that we can have a common language when discussing the technical concepts we'll cover this semester.

### Elements

>Elements are designators that define the structure and content of objects within a page. Some of the more frequently used elements include multiple levels of headings (identified as `h1` through `h6` elements) and paragraphs (identified as the `p` element); the list goes on to include the `a`, `div`, `span`, `strong`, and `em` elements, and many more.

>Elements are identified by the use of less-than and greater-than angle brackets, < >, surrounding the element name. Thus, an element will look like the following: `a`.

What are some elements on the page we created? One example of an element is the `h1` element. Play around with that — try replacing it with some HTML elements to see what they do (and try to guess before testing it!). Some common ones are: `b` and `i`.

The great part about web development is that a lot of learning comes out of just being curious and replacing text, saving it and trying it out! Don't be afraid to try new things. Worst case, CMD + Z is your best friend (or CTRL + Z for you silly Windows users).t
