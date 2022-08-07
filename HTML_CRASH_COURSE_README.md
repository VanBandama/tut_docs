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

# Graphics

You can put graphics into your website. It's done via ```<img>``` tag followed by ```src``` attribute:

```html
<body>
<img src="images/base-octocat.svg">
</body>
```

Effect:

![This is an image](https://myoctocat.com/assets/images/base-octocat.svg)

Also you can explicitly tell web browser how it should be viewed. Add height and width attributes. 
```html
<body>
<img src="images/base-octocat.svg" height = "300", width = "200">
</body>
```

You can wrap link ```<a>``` tag around image:

```html
<body>
<a href ="https://github.com/">
<img src="images/base-octocat.svg">
    </a>
</body>
```
Effect:

<a href="https://github.com/"> ![This is an image](https://myoctocat.com/assets/images/base-octocat.svg)</a>

# Audio

In the early 90's when internet where born, everybody wanted to share their hobbies. Show what type of music their listened to. And so HTML can play audio files from within browser. Of course assuming you uploaded audio to server (and you have every copyright to do it legally)

Nevertheless if you wan reader to listen to audio track just add ```<audio src>``` tag to your website:

```html
<body>
 <audio controls src="path/to/audio.mp3">
</body>
```
```<audio controls src>``` will display primitive YT/ vimeo controls to start/stop audio, increase/decrease volume ect.

You can force audio track to play autonomusly, loop or even mute it by adding:

```html
<body>
 <audio controls autoplay loop, muted src="path/to/audio.mp3">
</body>
```
If for some reason web browser can't play mp3 file. You can add alternative file with other extension:

```html
<body>
 <audio controls autoplay loop, muted>
 <source src = "path/to/audio.mp3">
 <source src = "path/to/audio.wav">
</body>
```

# Video

Same goes for video playback option:

```html
<body>
 <video controls src = "path/to/video.mp4">
</body>
```

And you can autoplay video when someone's get into your page. Heck even loop it to troll, and muted if you want:


```html
<body>
 <video controls autoplay loop muted src = "path/to/video.mp4">
</body>
```

Also if for some reason one browser can't play mp4 then you must provide other file extensions:


```html
<body>
 <video controls autoplay loop, muted>
 <source src = "path/to/video.mp4">
 <source src = "path/to/video.WebM">
</body>
```

*Doc Brown here frome the future "Examples of audio and won't work on github but You have to try and play with it yourself. Trust me I'm a doctor"

# Text formatting

Let's back in time to 1955. Actually no. let's get back 10 minutes earlier when we talked about long blocks of text.
You can format text if default viewing option is not for you. Displayed text can be bold, italic, it can be underlined etc.
Here's how:

```html
<body>
    <p>This is normal text</p> <!--- p stands for paragraph --!>
    <p>This is <b>bold</b> text</p> <!-- b is for bold genius --!>
    <p>This is <i>italic</i> text</p> <!-- i stands for italic genius --!>
    <p>This is <big>big</b> text</p> <!-- it'll enlarge a bit section surrounded by that tag --!>
    <p>This is <small>small</small> text</p> <!--pretty obvious einstein--!>
    <p>This is <sub>subscript</sub> text</p>
    <p>This is <sup>superscript</sup> text</p>
    <p>This is <del>deleted</del> text</p> <!-- line put through text --!>
    <p>This is <ins>inserted</ins> text</p> <!-- it's underlined --!>
    <p>This is <mark>marked</mark> text</p> <!-- text is marked --!>
</body>
```

Effect:

<p>This is normal text</p> <!--- p stands for paragraph --!>
    <p>This is <b>bold</b> text</p> <!-- b is for bold genius --!>
    <p>This is <i>italic</i> text</p> <!-- i stands for italic genius --!>
    <p>This is <big>big</b> text</p> <!-- it'll enlarge a bit section surrounded by that tag --!>
    <p>This is <small>small</small> text</p> <!--pretty obvious einstein--!>
    <p>This is <sub>subscript</sub> text</p>
    <p>This is <sup>superscript</sup> text</p>
    <p>This is <del>deleted</del> text</p> <!-- line put through text --!>
    <p>This is <ins>inserted</ins> text</p> <!-- it's underlined --!>
    <p>This is <mark>marked</mark> text</p> <!-- text is marked --!>

*Note that big, small, marked text isn't working (again) on github 'coz it's github.

# Lists

There are 3 types of lists:

 1.Unordered <br>
 2.Ordered<br>
 3.Description<br>

## 1.Unordered List

```html
<body>
<p>Groceries to buy</p>
<ul> <!-- ul stands for unordered list --!>
<li>Tomato</li> <!-- li stands for list item --!>
<li>Cheese</li>
<li>Bread</li>
<li>Ham</li>
</ul>
</body>
```
Effect:

Groceries to buy<br>
-Tomato<br>
-Cheese<br>
-Bread<br>
-Ham<br>

Again you can wrap ```<a>``` tag to make navigation menu for your website:
 
```html
<body>
<p>My menu</p>
<ul> 
<a href:" link/to/subpage1.html"><li>Home</li></a>
<a href:" link/to/subpage2.html"><li>Blog</li></a>
<a href:" link/to/subpage3.html"><li>About</li></a>
<a href:" link/to/subpage4.html"><li>Contact</li></a>
</ul>
</body>
```

## 2.Ordered list

```html
<body>
<p>Groceries to buy</p>
<ol> <!-- ol stands for ordered list --!>
<li>Tomato</ol> 
<li>Cheese</li>
<li>Bread</li>
<li>Ham</li>
</ol>
</body>
```
BTW. you can change viewing of order from numbers to letters:

```html
<body>
<p>Groceries to buy</p>
<ol type = "A"> <!-- ol stands for ordered list --!>
<li>Tomato</ol> 
<li>Cheese</li>
<li>Bread</li>
<li>Ham</li>
</ol>
</body>
```

## 3.Description list

```html
<dl>
<dt>HTML</dt>
<dd>This helps to structurize website</dd>
<dt>CSS</dt>
<dd>This helps to design visually website</dd>
<dt>JavaScript</dt>
<dd>This add interactivity to a website</dd>
</dl>
```

