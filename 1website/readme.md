# Workshop 1: Personal Website

This workshop is for someone with 0 knowledge about coding to get a personal website started in less than an hour. 
We will teaching the basics of HTML and CSS, using the compiler Cloud9.



### Step 1: Setting up Cloud9
Before we begin coding, you must set up a Cloud9 account. This is a web based 
compiler where we will be writting all our code. Got to: https://hackclub.com/cloud9_setup. 

Enter your email and create a new account. Now create a new workspace and name it `PersonalWebsite` and 
select `Don't set a team for this workspace`. Make sure `public` and the template `HTML5` are selected. 

Click the green `Create workspace` button at the bottom.



### Step 2: Setting up the HTML File 

Start by creating an HTML file. Rick click the `PersonalWebsite` folder on the left sidebar and select `New File`.
Name the file `index.html`. Now double click on the file and it should open up.

Create the backbone of HTML file by typing the following:

```html
<!DOCTYPE html>
<html>
    <head>
    </head>
    <body>
    </body>
</html>
```

Make sure to save as you go along by clicking `file` and `save` or use the shortcut <kbd>Ctrl+s</kbd>. 

You can preview the page by clicking `Preview` on the top bar and then selecting `Live Preview File`.

#### Side note: Comments
Comments can be made in HTML by using `<!--` and `-->`. Text inside these arrows are not dispalyed in 
the browser, but helps document your HTML code. It is a good habit to always comment your code.

```html
<!-- This is a comment-->
```

#### Side note 2: Live Preview
You can preview the code as you work by opening up Live Preview. To do this, click on the `Preview` button
on the top bar of Cloud9. Then select `Live Preview`.

### Step 3: Adding Text

Now you can add some text to your webpage. HTML uses a variety of elements to automatically format 
and identify text. There are mutlipe heading elements (`<h1>`, `<h2>`, `<h3>`, ..., `<h6>`) that create headers,
and there is also a paragraph element (`<p>`) to create paragraph text. 

Text is written inside the body and must be enclosed by a starting (ex: `<p>`) and ending tag (ex: `</p>`). 
Try this! An example is shown below.

```html
<!DOCTYPE html>
<html>
    <head>
    </head>
    <body>
        <h1>Roslyn Code Club</h1> <!--Heading 1-->
        <h2>by Jeffrey Yu</h2> <!--Heading 2-->
        <p>We are the Roslyn Code Club</p> <!--paragraph-->
    </body>
</html>
```

### Step 4: Adding Photos

You can add a photo by using the `<img>` tag. In this tag, you use attributes to control how the tag behaves. 


The attribute `srs` specifies the source of the image. This can be a URL or a file path. 


The attribute `alt` is used as an alternative if the image can not load for whatever reason, usually named 
whatever the image is suppose to be. 

The attribute `title` is the title of the image and is displayed as a tooltip when you mouse over the image.
This attribute can be used with different elements, too, such as `<p>`.

Try adding an image yourself! Google an image and copy it's sourse URL (done by right clicking and selecting 
`Copy Image Address`) An example is show below:

```html
<!DOCTYPE html>
<html>
    <head>
    </head>
    <body>
        <img src="cody1.PNG" alt="cody" title="Cody the Code Club Code Cub"> <!--Image-->
        <h1>Roslyn Code Club</h1> 
        <h2>by Jeffrey Yu</h2>
        <p>We are the Roslyn Code Club</p> 
    </body>
</html>
```

### Step 5: Adding Lists

Lists are just another text element. There are two types of lists: ordered and unordered.

Lets start with an unordered list. The unordered list  tag is `<ul>`. 
Then each list item must have the tag `<li>`. List items are displayed as bullet points.
Try this yourself! An example is shown below.

```html
<!DOCTYPE html>
<html>
    <head>
    </head>
    <body>
        <img src="cody1.PNG" alt="cody" title="Cody the Code Club Code Cub">
        <h1>Roslyn Code Club</h1>
        <h2>by Jeffrey Yu</h2>
        <p>We are the Roslyn Code Club</p>
        <h3>What we Do</h3>
        <!-- Unordered List-->
        <ul>
          <li>Weekly Meetings</li>
          <li>Bryant Library Workshops</li>
          <li>Computer Science Competitions</li>
        </ul>
    </body>
</html>
```

Ordered lists are another type of list, where list items are numbered. The ordered list tag is `<ol>` and 
follows the same rules as unordered lists. Try this yourself! An example is shown below.

```html
<!DOCTYPE html>
<html>
    <head>
    </head>
    <body>
        <img src="cody1.PNG" alt="cody" title="Cody the Code Club Code Cub">
        <h1>Roslyn Code Club</h1>
        <h2>by Jeffrey Yu</h2>
        <p>We are the Roslyn Code Club</p>
        <h3>What we Do</h3>
        <ul>
          <li>Weekly Meetings</li>
          <li>Bryant Library Workshops</li>
          <li>Computer Science Competitions</li>
        </ul>
        <h3>Workshops</h3>
        <!--Ordered List-->
        <ol>
          <li>Personal Website</li>
          <li>Navigation Bar</li>
          <li>Tags and Embedding</li>
        </ol>
    </body>
</html>
```


### Step 6: HTML Formatting Elements

You can add some style directly into the HTML code using tags, but the options are limited.

The HTML `<b>` element defines <b>bold</b> text, without any extra importance.
<br>The HTML `<strong>` element defines <strong>strong</strong> text, with added semantic "strong" importance.

The HTML `<i>` element defines <i>italic</i> text, without any extra importance.
<br>The HTML `<em>` element defines <em>emphasized</em> text, with added semantic importance.

he HTML `<small>` element defines <small>smaller</small> text.

The HTML `<mark>` element defines <mark>marked</mark> or <mark>highlighted</mark> text.

The HTML `<del>` element defines <del>deleted</del> (removed) text.

These are just a few of the many HTML formatting elements. You can find more online witha simple Google search.
Now you try! An example is below:

```html
<!DOCTYPE html>
<html>
    <head>
    </head>
    <body>
        <img src="cody1.PNG" alt="cody" title="Cody the Code Club Code Cub">
        <h1>Roslyn Code Club</h1>
        <h2>by Jeffrey Yu</h2>
        <p>We are the <u>Roslyn Code Club</u></p>  <!-- Underlined "Roslyn Code Club" -->
        <h3>What we Do</h3>
        <ul>
          <li>Weekly Meetings</li>
          <li>Bryant Library Workshops</li>
          <li>Computer Science Competitions</li>
        </ul>
        <h3>Workshops</h3>
        <ol>
          <li>Personal Website</li>
          <li>Navigation Bar</li>
          <li>Tags and Embedding</li>
        </ol>
    </body>
</html>
```

### Step 7: Setting up CSS

CSS, also known as Cascading Style Sheets, is used to add more style to a webpage.

Start by creating a new file inside your `PersonalWebsite` folder and name it `styles.css`.
You must now link this file to your HTML code. This is done by addings some code to the `<head>` of the HTML code.

The `<link />` element is used. The `rel` attribute is used to define what is being linked and the 
`href` attribute is used to specify where the file can be found. Add this:

```html
<link rel="stylesheet" href="styles.css"/>
```

to the `<head>` of your HTML code.

An example is shown below:

```html
<!DOCTYPE html>
<html>
    <head>
      <link rel="stylesheet" href="styles.css"/> <!--Link the CSS file-->
    </head>
    <body>
      <img src="cody1.PNG" alt="cody" title="Cody the Code Club Code Cub">
        <h1>Roslyn Code Club</h1>
        <h2>by Jeffrey Yu</h2>
        <p>We are the <u>Roslyn Code Club</u></p>
        <h3>What we Do</h3>
        <ul>
          <li>Weekly Meetings</li>
          <li>Bryant Library Workshops</li>
          <li>Computer Science Competitions</li>
        </ul>
        <h3>Workshops</h3>
        <ol>
          <li>Personal Website</li>
          <li>Navigation Bar</li>
          <li>Tags and Embedding</li>
        </ol>
    </body>
</html>
```


### Step 8: Adding Styles to CSS

Now open up the CSS file and lets get styling. CSS works by having a selector, often an element, 
and defining rules for it in `{` `}` brackets.

To resize all images on a webpage, select the element `img` and set the `width` to the desired `px`.
You can also add a `margin` of blank space around it. An example of this is shown:

```css
img {
    width: 500px;
    margin: 8px;
}
```

You can then change the style of the entire webpage by selecting 'body'. You can change the
text alignment, font, text color, and background color. An example of this is shown:

```css
body {
    text-align: center;
    font-family: Helvetica;
    background-color:#809fff;
    color: black;
    margin: 20px;
}
```

### Step 9: Being ~fancy~ with CSS

Now