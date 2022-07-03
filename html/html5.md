<h1 align="center" style="font-family: Roboto">
Beginner's 
<br/>
HTML CHEAT SHEET
</h1>

```html
<html>...</html>
```

<p style="font-family: Roboto">
The tag shows up at beginning and end of an HTML document(know as the root element). It indicates that the webpage is written in HTML5, and all other page markup comens in between these beginning and ending tags.
</p>

```html
<head>...</head>
```

<p style="font-family: Roboto">
The contains information that specific page, including the
title tags, meta data, and links to scripts and style sheets.
</p>

```html
<title>...</title>
```

<p style="font-family: Roboto">
The title tag is the title for that page, useful for both search
engines (when they scan and index pages) and users
 (showing up up inabrowser's title bar) by explicitly stating
the primary topic of each page.
</p>

```html
<body>...</body>
```

<p style="font-family: Roboto">
Body tags include all content that will be shown to users,
 including everything they'll see & read.
</p>

<h4 style="font-family: Roboto" >Example:</h4>

``` html
<html>
<head>
	<title>HTML5 Cheat Sheet</title>
</head>
<body>
	<h1>Beginner's HTML Cheat Sheet</h1>
</body>
</html>
```

<h3 style="font-family: Roboto" >Document Information:</h4>

```html
<base/>
```

<p style="font-family: Roboto">
The Base URL (for example:www.YourSite.com) is useful
for specifying all relative links inadocument (especially if
you have many internal links).
</p>


```html
<meta/>
```

<p style="font-family: Roboto">
Meta data spells out additional information about the
page, including the page's description, author, published
date, keywords and other typically "hidden" page information.
</p>

```html
<link/>
```

<p style="font-family: Roboto">
Can be used to a create relationships with external pages
or documents, including style sheets.
</p>

```html 
<style></style>
```

<p style="font-family: Roboto">
This element includes document style information, typically defaulting to CSS.
</p>

```html
<script></script>
```

<p style="font-family: Roboto">
This element includes all scripting information, or links to
external scripts. You can also include this element in the
body to dynamically generate content. 
</p>

<h4 style="font-family: Roboto" >Example:</h4>

``` html
<html>
  <head>
   <meta charset="utf-8">
   <base href="http://website.com"target="_blank"/>
   <title>My Beautiful Website</title>
   <link rel="stylesheet"href="/css/style.css">
    <script type="text/javascript">
       var MyVar=0;
    </script>
 </head>
 <body>
 ...
 </body>
</html>
```
<h3 style="font-family: Roboto" >Document Structure:</h4>

```html
<h1>...</h1>
<h2>...</h2>
<h3>...</h3>
<h4>...</h4>
<h5>...</h5>
<h6>...</h6>
```

<p style="font-family: Roboto">
All six levels of Headings, with 1 being the most important
on a page and 6 being the least. These elements are used
to describe content sections on a page.
</p>

```html
<div>...</div>
```

<p style="font-family: Roboto">
A generic container used to denote a page section or
</p>

```html
<span>...</span>
```

<p style="font-family: Roboto">
An inline section or block container, typically used for
grouping styling elements.
</p>

```html
<p>...</p>
```

<p style="font-family: Roboto">
This foundational tag is used to organize paragraphs of
text.
</p>

```html
<br/>
```

<p style="font-family: Roboto">
Creates a line break (or old-school carriage-return), useful
for writing blocks of text that need to be on different lines
(think addresses,etc.)
</p>

```html
<hr/>
```

<p style="font-family: Roboto">
Creates a horizontal rule, a sectional break in an HTML
page. Typically used to denote a change in topic or section
of a page.
</p>

<h4 style="font-family: Roboto" >Example:</h4>

``` html
<div>
 <h1>Ways to make your cat happy</h1>
 <p>You havea <span>mini-lion</span> at
home and you want to make it as happy as pos
sible.</p>
 <h/>
 <h2>Feed your cat well.</h2>
 <p>The right diet is<span>extremely</span>
important for the wellbeing of your cat.<br/>
Obesity isacommon source of problems among
domesticated animals.</p>
</div>
```

<h3 style="font-family: Roboto" >Text:</h3>

```html
<strong>...</strong>
```

<p style="font-family: Roboto">
Exactly like it sounds,indicating STRONG emphasis,displayed bold in most browsers.
</p>

```html
<b>...</b>
```

<p style="font-family: Roboto">
Another way to create bold text,however it's more for
drawing attention as opposed to emphasizing extra emphasis like the previous tag.
</p>

```html
<em>...</em>
```

<p style="font-family: Roboto">
The emphasis tags also are like they sound,emphasizing text or phrases displayed as italics in most browsers.
</p>

```html
<i>...</i>
```

<p style="font-family: Roboto">
Another way to add italics to text,however without the
added emphasis (similar to the bold tags above) and instead used to denote things like thoughts or names. 
</p>

```html
<strike>...</strike>
```

<p style="font-family: Roboto">
This tag creates strike through text (or text with a line
through it). Another older tag not commonly supported.
</p>

```html
<pre>...</pre>
```

<p style="font-family: Roboto">
Pre-formatted, ‘monospace’ text laid out with whitespace inside the element intact.
</p>

```html
<del>...</del>
```

<p style="font-family: Roboto">
Helps denote a previously deleted section of text.
</p> 

```html
<blockquote>...</blockquote>
```

<p style="font-family: Roboto">
Reserved for long paragraphs of quotations, often cited.
</p>

```html
<q>...</q>
```

<p style="font-family: Roboto">
These are used for shorter quotations.
</p>

```html
<address>...</address>
```

<p style="font-family: Roboto">
A helpfully obvious tag that displays the author's contact information.
</p>

```html
<code>...</code>
```

<p style="font-family: Roboto">
Code text displays code snippets (like the one over to the left), typically showing up monospaced.
</p>

```html
<small>...</small>
```

<p style="font-family: Roboto">
Small size text Historically used to simply reduce text size,
in HTML5 it aso refers to information that may no longer be valid, accurate or relevant.
</p>

<h3 style="font-family: Roboto" >Links:</h4>

```html
<a href="http://www.google.com">...</a>
```

<p style="font-family: Roboto">
Anchor text for hyperlink. 
</p>

```html
<a href="mailto:">...</a>
```

<p style="font-family: Roboto">
A link used to pull up an outgoing message to a specific email address.
</p>

```html
<a href="tel:">...</a>
```

<p style="font-family: Roboto">
A link to make phone numbers clickable, especially useful for mobile users.
</p>

```html
<a name="name">...</a>
```

<p style="font-family: Roboto">
An anchor that's useful for bringing users to specific document elements.
</p>

```html
<a href="#name">...</a>
```

<p style="font-family: Roboto">
An anchor link that brings users specifically to a div element.
</p>

<h3 style="font-family: Roboto" >Images:</h4>

```html
<img/>
```

<p style="font-family: Roboto">
An image tag to include and display image files.
</p>

```html
<img src="url" />
```

<p style="font-family: Roboto">
Exactly like it sounds. The URL or file on the image to display.
</p>

```html
<img src="url" alt="text" />
```

<p style="font-family: Roboto">
Alternative text that helps explain the image content to both search engines and users.
</p>

```html
<img src="url" height="100" />
```

<p style="font-family: Roboto">
The ability to specify image height in pixels or percentages.
</p>

```html
<img src="url" width="100" />
```

<p style="font-family: Roboto">
The ability to specify width in pixels or percentages.
</p>

```html
<img src="url" align="" />
```

<p style="font-family: Roboto">
The alignment of the image.
</p>

```html
<img src="url" border="" />
```

<p style="font-family: Roboto">
Explains the border thickness (if any) of the image.
</p>

<h3 style="font-family: Roboto" >Lists:</h4>

```html
<ol>...</ol>
```

<p style="font-family: Roboto">
Create numbered (ordered) lists showing sequential order, preference or priority.
</p>

```html
<ul>...</ul>
```

<p style="font-family: Roboto">
Display a bulleted (unordered) list without any extra emphasis on order of importance.
</p>

```html
<li>...</li>
```

<p style="font-family: Roboto">
Specifies each list items to be bulleted or numbered.
</p>

<h4 style="font-family: Roboto" >Example:</h4>

```html
<ol>
<li>Item 1</li>
<li>Item 2</li>
<li>Item 3</li>
</ol> 

<ul>
<li>Item 1</li>
<li>Item 2</li>
<li>Item 3</li>
</ul>
```

<h3 style="font-family: Roboto" >Forms:</h4>

```html
<form>...</form>
```

<p style="font-family: Roboto">
The form element creates a form, spelling out how the form will operate based on its attributes.
</p>

```html
<form action="">...</form>
```

<p style="font-family: Roboto">
The form action URL specifies where data is to be sent when a site visitor submits the form. 
</p>

```html
<form method="">...</form>
```

<p style="font-family: Roboto">
The method attribute refers to the HTTP method (GET, POST), which dictates how to send the form data.
</p>

```html
<form autocomplete>...</form>
```

<p style="font-family: Roboto">
Dictates whether a form should have autocomplete enabled or off.
</p>

```html
<form novalidate>...</form>
```

<p style="font-family: Roboto">
Dictates whether a form should not be validated when submitted.
</p>

```html
<form target="">...</form>
```

<p style="font-family: Roboto">
Tells where to display the form response after being submitted, generally one of the following: <code>_blank, _self, _parent, _top </code>
</p>

```html
<label>...</label>
```

<p style="font-family: Roboto">
A simple field label, telling the user what to enter in each field.
</p>

```html
<input/>
```

<p style="font-family: Roboto">
The form input attribute defines the type of field information to receive from a user.
</p>

```html
<input type="" />
```

<p style="font-family: Roboto">
Specifies the field input type, typical including <code>text, password, date-time, checkbox</code>
</p>

```html
<input type="" value="" />
```

<p style="font-family: Roboto">
Describes the value or input field information.
</p>

```html
<input type="" size="" />
```

<p style="font-family: Roboto">
Specifies the input element width in characters.
</p>

```html
<input type="" maxlength="" />
```

<p style="font-family: Roboto">
Identifies the maximum input element character numbers allowed. 
</p>

```html
<input type="" required />
```

<p style="font-family: Roboto">
Another helpfully explicit tag, making sure the <code>input</code> element is completely filled out prior to the user submitting the form.
</p>

```html
<input type="" width="" />
```

<p style="font-family: Roboto">
Specifies the width (in pixels) of the <code>input</code> element.
</p>

```html
<input type="" height="" />
```

<p style="font-family: Roboto">
Specifies the height (in pixels) of the <code>input</code> element.
</p>

```html
<input type="" placeholder="" />
```

<p style="font-family: Roboto">
Provides a helpful hint to the user, describing what the <code>input</code> element value should be.
</p>

```html
<input type="" autofocus />
```

<p style="font-family: Roboto">
Says to make sure that the <code>input</code> element comes into focus after the page loads.
</p>

```html
<input type="" disabled />
```

<p style="font-family: Roboto">
Disables <code>input</code> element on the form.
</p>

```html
<textarea>...</textarea>
```

<p style="font-family: Roboto">
Specifies a large text input for longer messages.
</p>

```html
<select>...</select>
```

<p style="font-family: Roboto">
Describes a drop-down box list automatically comes into focus after the page loads.
</p>

```html
<select name="">...</select>
```

<p style="font-family: Roboto">
The name for a drop down combination box.
</p>

```html
<select multiple>...</select>
```

<p style="font-family: Roboto">
Allows for multiple selections to be made at one time.
</p>

```html
<select size="">...</select>
```

<p style="font-family: Roboto">
Specifies the number of available, visible options in a drop-down box. 
</p>

```html
<option>...</option>
```

<p style="font-family: Roboto">
Defines one of the available options in a drop-down list.
</p>

```html
<option value="">...</option>
```

<p style="font-family: Roboto">
Explains the option value available for selection.
</p>

```html
<option value="" selected>...</option>
```

<p style="font-family: Roboto">
Defines the default selected option in a drop-down list.
</p>

```html
<button>...</button>
```

<p style="font-family: Roboto">
Defines the clickable button for users to submit options.
</p>

<h4 style="font-family: Roboto" >Example:</h4>

```html
<form action="action_page.php" method="post">
First name:<br>
<input type="text" name="firstName" value="" placeholder="Enter your first name"><br>
Last name:<br>
<input type="text" name="lastName" value="" placeholder="Enter your last name"><br>
Favorite color:<br>
<select name="color">
	<option value="red">Red</option>
	<option value="green">Green</option>
	<option value="blue">Blue</option>
</select>
<textarea name="comment" placeholder="Enter your comment here"></textarea>
<button type="submit">Submit</button>
</form>
```

<h3 style="font-family: Roboto" >Forms:</h3>

```html
<table>...</table>
```

<p style="font-family: Roboto">
The table tag identifies and contains all table related content.
</p>

```html
<caption>...</caption>
```

<p style="font-family: Roboto">
The caption is a description of what the table is, and what it contains.
</p>

```html
<thead>...</thead>
```

<p style="font-family: Roboto">
The table headers describe the type of information contained in each column underneath.
</p>

```html
<tbody>...</tbody>
```

<p style="font-family: Roboto">
The table body contains the table's data or information.
</p>

```html
<tfoot>...</tfoot>
```

<p style="font-family: Roboto">
Table footers describe all footer content.
</p>

```html
<tr>...</tr>
```

<p style="font-family: Roboto">
Contains the information to be included in a single row of the table.
</p>

```html
<th>...</th>
```

<p style="font-family: Roboto">
Contains the actual information or data in a single header item.
</p>

```html
<td>...</td>
```

<p style="font-family: Roboto">
Contains the actual information or data in a single table cell. 
</p>

```html
<col>...</col>
```

<p style="font-family: Roboto">
Defines a single column of information inside a table.
</p>

```html
<colgroup>...</colgroup>
```

<p style="font-family: Roboto">
Group a single (or multiple) columns for formatting purposes.
</p>

<h4 style="font-family: Roboto" >Example:</h4>

```html
<table>
<colgroup>
	<col span="2" style="background-color: #f00">
	<col style="width:100px">
</colgroup>
<tr>
	<th>First Name</th>
	<th>Last Name</th>
	<th>Age</th>
</tr>
<tr>
	<td>John</td>
	<td>Doe</td>
	<td>35</td>
</tr>
<tr>
	<td>Jane</td>
	<td>Doe</td>
	<td>32</td>
</tr>
</table>
```

<h3 style="font-family: Roboto" >HTML5 New Tags:</h3>

```html
<header>...</header>
```

<p style="font-family: Roboto">
Defines the header block for a document (or individual section).
</p>

```html
<footer>...</footer>
```

<p style="font-family: Roboto">
Identifies the footer block for a document (or an individual section).
</p>

```html
<nav>...</nav>
```

<p style="font-family: Roboto">
Navigation links for the user in a document.
</p>

```html
<main>...</main>
```

<p style="font-family: Roboto">
Describes the main content of a document.
</p>

```html
<article>...</article>
```

<p style="font-family: Roboto">
Identifies an article inside a document.
</p>

```html
<aside>...</aside>
```

<p style="font-family: Roboto">
Specifies content contained in a document sidebar.
</p>

```html
<section>...</section>
```

<p style="font-family: Roboto">
Specifies a section block in the document.
</p>

```html
<details>...</details>
```

<p style="font-family: Roboto">
Describes additional facts or information that the user can view or hide.
</p>

```html
<dialog>...</dialog>
```

<p style="font-family: Roboto">
A dialog box or window. 
</p>

```html
<mark>...</mark>
```

<p style="font-family: Roboto">
Displays a portion of highlighted text within the page content.
</p>

```html
<meter>...</meter>
```

<p style="font-family: Roboto">
Describes the scalar measurement within a know array.
</p>

```html
<progress>...</progress>
```

<p style="font-family: Roboto">
Displays the progress of a task, usually used for progress bar.
</p>

```html
<summary>...</summary>
```

<p style="font-family: Roboto">
Contains a visible heading for a <code>details</code> element.
</p>

```html
<time>...</time>
```

<p style="font-family: Roboto">
Identifies the time and date.
</p>

<h3 style="font-family: Roboto" >Collective Character Objects:</h3>

- Quotation marks: &quot &quot (" ")
- Ampersand: &amp (&)
- Less than sign: &lt (<)
- Greater than sign: &gt (>)
- Non-breaking space: &nbsp ( )
- Copyright: &copy (&copy;)
- @ symbol: &reg  (&reg;)
- Small bullet: &#8226 (&#8226;)
- Trade mark: &#8482 (&#8482;)