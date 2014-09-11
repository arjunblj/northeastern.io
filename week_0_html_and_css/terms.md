# Terms

So what did that code actually do? Visibly, the "title" of the page (visible in the browser tab) was set to "My Website" and there was text on the page that appeared.

In order to fully understand there's a few (only a few, I promise) terms you're going to have to know so that we can have a common language when discussing the technical concepts we'll cover this semester.

## Elements

>Elements are designators that define the structure and content of objects within a page. Some of the more frequently used elements include multiple levels of headings (identified as `h1` through `h6` elements) and paragraphs (identified as the `p` element); the list goes on to include the `a`, `div`, `span`, `strong`, and `em` elements, and many more.

>Elements are identified by the use of less-than and greater-than angle brackets, < >, surrounding the element name. Thus, an element will look like the following: `a`.

What are some elements on the page we created? One example of an element is the `h1` element. Play around with that — try replacing it with some HTML elements to see what they do (and try to guess before testing it!). Some common ones are: `b` and `i`.

The great part about web development is that a lot of learning comes out of just being curious and replacing text, saving it and trying it out! Don't be afraid to try new things. Worst case, CMD + Z is your best friend (or CTRL + Z for you silly Windows users).

## Tags

Your experimentation may have been futile because you didn't correctly structure your HTML elements. With very few exceptions, virtually every element is compost of these *tags*.

>The use of less-than and greater-than angle brackets surrounding an element creates what is known as a tag. Tags most commonly occur in pairs of opening and closing tags.

>An opening tag marks the beginning of an element. It consists of a less-than sign followed by an element’s name, and then ends with a greater-than sign; for example, `<div>`.

>A closing tag marks the end of an element. It consists of a less-than sign followed by a forward slash and the element’s name, and then ends with a greater-than sign; for example, `</div>`.

>The content that falls between the opening and closing tags is the content of that element. An anchor link, for example, will have an opening tag of `<a>` and a closing tag of `</a>`. What falls between these two tags will be the content of the anchor link.

>So, anchor tags will look a bit like this: `<a>...</a>`.

Some sets of tags we have on our "Hello World!" page: `<h1>...</h1>`, `<body>...</body>`, `<head>...</head>`, etc.

You'll notice all of our tags follow a sort of nested structure to them. Learn it. Love it.

While HTML isn't particularly sensitive to whitespace, it's generally good practice to structure your HTML in a cool, nested style. It's more readable and won't cause others to want to rip their eyeballs out. Don't do this:

```html
<html>
                            <head>
  <title>My


  Website</title>
</head>
  <body>
 <h1>Hello, World!
 </h1>
</body>
    </html>
```

While it's *functionally* the same, a cute bunny dies somewhere in the world every time you do that. You don't hate bunnies, *do you*????

Every HTML document is wrapped with a set of `html` tags. You can see this in virtually every site online, whether it's the small "Hello World!" page we rendered above or the Facebook's homepage (Don't go to Facebook to check! Stay focused!).

HTML files follow a structure that looks roughly like this:

```html
<html>
    <head>
        ... various head elements ...
    </head>
    <body>
        ... various body elements ...
    </body>
</html>
```

Let's go ahead and rebuild the page from scratch. Try along with me and compare your result (Don't peek, it won't help at all!).

First, we'll start with wrapping the page in `html` tags and adding some `head` elements.

The `head` contains *metadata* for the HTML file, which is data about the file that may or may not be visible right in the web page.

Right now, the only element we've learned about that goes in the head is the `title` element. Go ahead and add some title tags to the page and title your page!

If you're using Sublime, it might be tempting to allow it to auto-complete some of the tags you start, but trust me, there's so much more to be gained from the hard work of typing tags yourself.

Try running it! If it works, great! If not, take a stab at figuring it out before youcheck out the solution. Identifying mistakes yourself helps reinforce what the "correct" solution is.

You should have something that resembles this:

```html
<html>
    <head>
        <title>Han Shot First: You Know It Too</title>
    </head>
</html>
```

If you're there, congrats! Let's add some content to this currently bland site.

Try adding a variety of tags. Go ahead and add a variety of headings, ranging from `h1` to `h6` and some paragraphs of text.

Here's a quick example of this and the resulting page:

```html
<html>
    <head>
        <title>My Website</title>
    </head>
    <body>
        <h1>This is h1 text.</h1>
        <h2>This is h2 text.</h2>
        <h3>This is h3 text.</h3>
        <h4>This is h4 text.</h4>
        <h5>This is h5 text.</h5>
        <h6>This is h6 text.</h6>

        <p>Selfies quinoa locavore, farm-to-table meh fashion axe Marfa tattooed mixtape stumptown chillwave banh mi iPhone street art. Helvetica Godard typewriter pug. Blog cred Cosby sweater paleo, lomo Marfa Shoreditch iPhone. Paleo roof party pour-over, slow-carb retro direct trade photo booth flannel. Next level raw denim twee, organic hella vinyl cred dreamcatcher gentrify mustache occupy fashion axe banjo tofu.</p>

        <p>3 wolf moon you probably haven't heard of them crucifix post-ironic, butcher polaroid Brooklyn art party mixtape Banksy pug irony hashtag. Swag deep v Pinterest crucifix. Jean shorts High Life bespoke, ethical slow-carb paleo quinoa DIY kitsch cred photo booth Pinterest fap.</p>

        <p>This is a <b>bold</b> word. <i>Italics</i> is fun too, though.</p>
    </body>
</html>
```

![](https://www.dropbox.com/s/ez07qgc6qw1354h/Screenshot%202014-09-10%2023.24.59.png?dl=1)

Excellent, you should now have a page which uses a variety of different tags. Good work!

Go back and take a look at that measly "Hello world!" example you created earlier and how incredibly simple it was in comparison. YOU DONE GOOD, SON!


## Attributes

Congrats on making it to the third (and last) HTML-related term you'll have to learn!

Attributes are where the magic happens.

>Attributes are properties used to provide additional information about an element. The most common attributes include the id attribute, which identifies an element; the class attribute, which classifies an element; the src attribute, which specifies a source for embeddable content; and the href attribute, which provides a hyperlink reference to a linked resource.

>Attributes are defined within the opening tag, after an element’s name. Generally attributes include a name and a value. The format for these attributes consists of the attribute name followed by an equals sign and then a quoted attribute value.

For example, an `a` element including an href attribute would look like the following:

`<a href="http://northeastern.io/">yoloswag</a>`

which would create a link that looked like this: [yoloswag](http://northeastern.io/).

