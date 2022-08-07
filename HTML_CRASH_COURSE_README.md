HTML is a language which you'll use to structure your website.
Think of it as a skeleton, blueprint, framework.
Basic bare bone HTML website looks like this:
```html
<!DOCTYPE html>
<html>
    <head>
        <title>Title on top bar/tab!</title>
    </head>
    <body>
      <!-- This is a comment and it will not be displayed on page --!>
        Main stuff. Your content gets here
    </body>
</html>
```

- 1'st line :  ```<!DOCTYPE html>``` informs us (and browser) what document type to expect. It's just declaration tag.


- 2'nd line: ```<html>``` and it's closing ```</html>``` represents the root of an HTML document.
The ```<html>``` tag is the container for all other HTML elements.


- 3'rd line: The ```<head>``` element is a container for metadata (data about data) and is placed between the ```<html>``` tag and the ```<body>``` tag.
Metadata is data about the HTML document. Metadata is not displayed.
Metadata typically define the document title, character set, styles, scripts, and other meta information.
The following elements can go inside the ```<head>``` element:
    - ```<title>``` - must have in every website
    - ```<link>```
    - ```<script>```


- 4'th line : ```<title>``` as it's name sugest prints out website/ page title


- 6'th line: ```<body>``` tag defines document's body. It is here, where all the other elements of website will go (lists, forms, paragraphs, images and videos)


# Text formatting:

<b>1. Break line with ```<br>```</b>

If you have long block of text and you want to divide it into smaller parts, then by all means use ```<br>``` tag. It'll break a line and split text

I.e

Lorem ipsum dolor sit amet, consectetur adipiscing elit. Cras sollicitudin in enim at rutrum. Nam finibus leo et placerat pretium. Curabitur malesuada volutpat felis, ac malesuada augue tristique quis. Sed massa est, tincidunt sed gravida sit amet, accumsan sit amet ante. Ut fermentum tincidunt magna, et aliquam tellus dignissim ut. Vivamus lorem est, auctor in libero pretium, ullamcorper ultrices dolor. Aenean vulputate arcu sed volutpat vestibulum. Pellentesque sit amet dui in orci egestas ultricies. In at purus sem. Nam lobortis neque in nunc efficitur viverra. Ut convallis eleifend ornare. Aliquam et nisi sed lorem placerat tincidunt a eget nunc. Cras malesuada eget ipsum porttitor bibendum. Ut at ullamcorper augue. Nulla commodo purus eu auctor pellentesque. Ut vel tristique metus, eget interdum dui.

after adding ```<br>```:

Lorem ipsum dolor sit amet, consectetur adipiscing elit. Cras sollicitudin in enim at rutrum.```<br>``` <br> Nam finibus leo et placerat pretium. Curabitur malesuada volutpat felis, ac malesuada augue tristique quis. Sed massa est, tincidunt sed gravida sit amet, accumsan sit amet ante. Ut fermentum tincidunt magna, et aliquam tellus dignissim ut.```<br>``` <br>Vivamus lorem est, auctor in libero pretium, ullamcorper ultrices dolor. Aenean vulputate arcu sed volutpat vestibulum. Pellentesque sit amet dui in orci egestas ultricies. In at purus sem. Nam lobortis neque in nunc efficitur viverra. Ut convallis eleifend ornare. Aliquam et nisi sed lorem placerat tincidunt a eget nunc.```<br>``` <br>Cras malesuada eget ipsum porttitor bibendum. Ut at ullamcorper augue. Nulla commodo purus eu auctor pellentesque. Ut vel tristique metus, eget interdum dui.

*Note that ```<br>``` tag doesn't need a closing ```</>``` tag at all.

 <b>2. Divide with horizontal rule</b>

Also you can divide text with horizontal rule. Just use ```<hr>``` tag.

I.e

Lorem ipsum dolor sit amet, consectetur adipiscing elit. Cras sollicitudin in enim at rutrum. Nam finibus leo et placerat pretium. Curabitur malesuada volutpat felis, ac malesuada augue tristique quis. Sed massa est, tincidunt sed gravida sit amet, accumsan sit amet ante. Ut fermentum tincidunt magna, et aliquam tellus dignissim ut. Vivamus lorem est, auctor in libero pretium, ullamcorper ultrices dolor. Aenean vulputate arcu sed volutpat vestibulum. Pellentesque sit amet dui in orci egestas ultricies. In at purus sem. Nam lobortis neque in nunc efficitur viverra. Ut convallis eleifend ornare. Aliquam et nisi sed lorem placerat tincidunt a eget nunc. Cras malesuada eget ipsum porttitor bibendum. Ut at ullamcorper augue. Nulla commodo purus eu auctor pellentesque. Ut vel tristique metus, eget interdum dui.

After using ```<hr>``` :

Lorem ipsum dolor sit amet, consectetur adipiscing elit. Cras sollicitudin in enim at rutrum. Nam finibus leo et placerat pretium. Curabitur malesuada volutpat felis, ac malesuada augue tristique quis. Sed massa est, tincidunt sed gravida sit amet, accumsan sit amet ante. Ut fermentum tincidunt magna, et aliquam tellus dignissim ut.```<hr>```<hr> Vivamus lorem est, auctor in libero pretium, ullamcorper ultrices dolor. Aenean vulputate arcu sed volutpat vestibulum. Pellentesque sit amet dui in orci egestas ultricies. In at purus sem. Nam lobortis neque in nunc efficitur viverra. Ut convallis eleifend ornare. Aliquam et nisi sed lorem placerat tincidunt a eget nunc. Cras malesuada eget ipsum porttitor bibendum. Ut at ullamcorper augue. Nulla commodo purus eu auctor pellentesque. Ut vel tristique metus, eget interdum dui.

*Also ```<hr>``` tag doesn't require closing tag

<b>3. Heading (very same as in newspaper!)</b>

You can capture readers attention by using headers. Just use pair of ```<h1></h1>``` tag:

```html
<body>
<h1>News Flash! Clark Kent is Superman!</h1>
</body>
```

Which will produce:

# News flash! Clark Kent is Superman!

*Note that in web browser there will be no horizontal rule added to header. It's just github markdown magic going on here.
There are many levels when comes to importance of a header. Starting with ```<h1>``` which is most important (in this case text become larger) up to ```<h6>``` or even ```<h7>``` (being smaller). But general rule of thumb is to use up to ```<h3>``` level for headers.

# Hyperlinks

You can put links inside your website (which will come in handy for your SEO and Google's crawling bot - more on that later)
To do that use ```<a></a>``` tag:

```html
<body>
  <a href ="https://www.google.com"> Google website</a>
</body>
```

Effect:

<a href ="https://www.google.com"> Google website</a>

In addition to that tag you can specify how link will open. In new tab or window.
For new window  add:

```html
<body>
<a href ="https://www.google.com" target ="_blank"> Google website</a>
</body>
```

Effect:

<a href ="https://www.google.com" target ="_blank"> Google website</a>

for the same tab/window use:

```html
<body>
<a href ="https://www.google.com" target ="_self"> Google website</a>
</body>
```
Effect:

<a href ="https://www.google.com" target ="_self"> Google website</a>

There's also other attributes like:
- ```_parent``` - Opens the document in the parent frame
- ```_top``` - Opens the document in the full body of the window

One more thing. You can add text that hint reader what he/she can expect after clicking. It can be very helpful for blind people who are using website readers. Or for previously mentioned Google bot to boost your website in search resaults.

By adding:

```html
<body>
<a href ="https://www.google.com" target ="_self" title= "This link lead you to Google"> Hover over here</a>
</body>
```
Effect:

<a href ="https://www.google.com" target ="_self" title= "This link lead you to Google"> Hover over here</a>

If your website have multiple sub-pages you can link to those same way:

```html
<body>
<a href ="mywebsite/pages/subpage2.html" target ="_self">Kittens photo album</a>
</body>
```
*Note that ```subpage2.html``` file must be a relative path to that file. Again it's up to you how you structurize your files

![This is an image](https://myoctocat.com/assets/images/base-octocat.svg)
