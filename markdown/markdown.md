<h1 style="font-family: Roboto" align="center">
MARKDOWN CHEAT SHEET 
</h1>

<h3 style="font-family: Roboto">
Markdown Quick Reference 
</h3>

<h4 style="font-family: Roboto">
<code>Headers (atx style)</code> 
</h4>

```markdown
# h1
## h2
### h3
#### h4
##### h5
###### h6
```

<h4 style="font-family: Roboto">
<code>Headers (setext style)</code>
</h4>

```markdown
Header 1
========
Header 2
--------
```

<h4 style="font-family: Roboto">
<code>Blockquotes</code>
</h4>

```markdown
> This is
> a blockquote
>
> > Nested
> > Blockquote
```

<h4 style="font-family: Roboto">
<code>Unordered List</code>
</h4>

```markdown
* Item 1
* Item 2
    * item 3a
    * item 3b

or

- Item 1
- Item 2

or

+ Item 1
+ Item 2

or

- [ ] Checkbox off
- [X] Checkbox on
```

<h4 style="font-family: Roboto">
<code>Ordered List</code>
</h4>

```markdown
1. Item 1
2. Item 2
    a. item 3a
    b. item 3b
```

<h4 style="font-family: Roboto">
<code>Links</code>
</h4>

```markdown
[link](http://google.com)
[link][google]
[google]: http://google.com
<http://google.com>
```

<h4 style="font-family: Roboto">
<code>Emphasis</code>
</h4>

```markdown
*italic*
_italic_
**bold**
__bold__
`inline code`
~~struck out~~
```

<h4 style="font-family: Roboto">
<code>Horizontal line</code>
</h4>

```markdown
Hyphens

---
Asterisks

***
Underscores

___
```

<h4 style="font-family: Roboto">
<code>Code</code>
</h4>

```markdown

```javascript
console.log("This is a block code")
	```
~~~css
.button { border: none; }
~~~
 4 space indent makes a code block

inline code
`Inline code` has back-ticks around it
```

<h4 style="font-family: Roboto">
<code>Tables</code>
</h4>

```markdown
| Left column | Center column | Right column |
|:------------|:-------------:|-------------:|
| Cell 1      |   Centered    |        $1600 |
| Cell 2      |    Cell 3     |          $12 |
Simple style

Left column | Center column | Right column
:----------:|:-------------:|:-----------:
   Cell 1   |   Centered    |    $1600
   Cell 2   |    Cell 3     |     $12
 
// A markdown table generator: tableconvert.com
```

<h4 style="font-family: Roboto">
<code>Images</code>
</h4>

```markdown
![GitHub Logo](/images/logo.png)

![Alt Text](url)

Image with link
[![GitHub Logo](/images/logo.png)](https://github.com/)

[![Alt Text](image_url)](link_url)

Reference style
![alt text][logo]

[logo]: /images/logo.png "Logo Title"
```

<h4 style="font-family: Roboto">
<code>Backslash escapes</code>
</h4>

| **Characters** | **Escape** | **Description**     |
|----------------|------------|---------------------|
| \              | \\         | backslash           |
| `              | \`         | backtick            |
| *              | \*         | asterisk            |
| _              | \_         | underscore          |
| {}             | \{}        | curly braces        |
| []             | \[]        | square brackets     |
| ()             | \()        | parentheses         |
| #              | \#         | hash mark           |
| +              | \+         | plus sign           |
| -              | \-         | minus sign (hyphen) |
| .              | \.         | dot                 |
| !              | \!         | exclamation mark    |