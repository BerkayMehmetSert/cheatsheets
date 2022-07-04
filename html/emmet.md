<h1 style="font-family: Roboto" align="center">
EMMET CHEAT SHEET
</h1>

<h3 style="font-family: Roboto">
Multiplication: * 
</h3>

<h4 style="font-family: Roboto">
<code>ul>li*5</code>
</h4>

```html
<ul>
    <li></li>
    <li></li>
    <li></li>
    <li></li>
    <li></li>
</ul>
```

<h3 style="font-family: Roboto">
Child: >
</h3>

<h4 style="font-family: Roboto">
<code>nav>ul>li</code> 
</h4>

```html
<nav>
    <ul>
        <li></li>
    </ul>
</nav>
```

<h3 style="font-family: Roboto">
Custom attributes 
</h3>

<h4 style="font-family: Roboto">
<code>p[title="Hello world"]</code> 
</h4>

```html
<p title="Hello world"></p>
```

<h4 style="font-family: Roboto">
<code>td[rowspan=2 colspan=3 title]</code>
</h4>

```html
<td rowspan="2" colspan="3" title=""></td>
```

<h4 style="font-family: Roboto">
<code>[a='value1' b="value2"]</code>
</h4>

```html
<div a="value1" b="value2"></div>
```

<h3 style="font-family: Roboto">
Text: {} 
</h3>

<h4 style="font-family: Roboto">
<code>a</code>
</h4>

```html
<a href="">Click me</a>
```

<h4 style="font-family: Roboto">
<code>p>{Click }+a{here}+</code> 
</h4>

```html
<p>Click <a href="">here</a> to continue</p>
```

<h4 style="font-family: Roboto">
<code>p>{Click }+a{here}+</code> 
</h4>

```html
<p>Click <a href="">here</a> to continue</p> 
```

<h3 style="font-family: Roboto">
ID and CLASS attributes 
</h3>

<h4 style="font-family: Roboto">
<code>#header</code> 
</h4>

```html
<div id="header"></div> 
```

<h4 style="font-family: Roboto">
<code>.title</code> 
</h4>

```html
<div class="title"></div> 
```

<h4 style="font-family: Roboto">
<code>form#search.wide</code>
</h4>

```html
<form id="search" class="wide"></form>
```

<h4 style="font-family: Roboto">
<code>p.class1.class2.class3</code>
</h4>

```html
<p class="class1 class2 class3"></p>
```

<h3 style="font-family: Roboto">
Implicit tag names 
</h3>

<h4 style="font-family: Roboto">
<code>.class</code>
</h4>

```html
<div class="class"></div>
```

<h4 style="font-family: Roboto">
em>.class 
</h4>

```html
<em>
	<span class="class"></span>
</em>
```

<h4 style="font-family: Roboto">
<code>ul>.class</code>
</h4>

```html
<ul>
	<li class="class"></li>
</ul>
```

<h4 style="font-family: Roboto">
<code>table>.row>.col</code>
</h4>

```html
<table>
	<tr class="row">
		<td class="col"></td>
	</tr>
</table>
```

<h3 style="font-family: Roboto">
Climb-up: ^
</h3>

<h4 style="font-family: Roboto">
<code>div+div>p>span+em^bq</code>
</h4>

```html
<div></div>
<div>
    <p><span></span><em></em></p>
    <blockquote></blockquote>
</div>
```

<h4 style="font-family: Roboto">
<code>div+div>p>span+em^^bq</code>
</h4>

```html
<div></div>
<div>
    <p><span></span><em></em></p>
</div>
<blockquote></blockquote> 
```

<h3 style="font-family: Roboto">  
Sibling: +
</h3>

<h4 style="font-family: Roboto">
<code>div+p+bq</code>
</h4>

```html
<div></div>
<p></p>
<blockquote></blockquote>
```

<h3 style="font-family: Roboto">
Grouping: ()
</h3>

<h4 style="font-family: Roboto">
<code>div>(header>ul>li*2>a)+footer>p</code>
</h4>

```html
<div>
    <header>
        <ul>
            <li><a href=""></a></li>
            <li><a href=""></a></li>
        </ul>
    </header>
    <footer>
        <p></p>
    </footer>
</div>
```

<h4 style="font-family: Roboto">
<code>(div>dl>(dt+dd)*4)+footer>p</code>
</h4>

```html
<div>
    <dl>
        <dt></dt>
        <dd></dd>
        <dt></dt>
        <dd></dd>
        <dt></dt>
        <dd></dd>
        <dt></dt>
        <dd></dd>
    </dl>
</div>
<footer>
    <p></p>
</footer>
```

<h3 style="font-family: Roboto">
$ 
</h3>

<h4 style="font-family: Roboto">
<code>ul>li.item$*3</code>
</h4>

```html
<ul>
    <li class="item1"></li>
    <li class="item2"></li>
    <li class="item3"></li>
</ul>
```

<h4 style="font-family: Roboto">
<code>h$[title=item$]{Header $}*3</code>
</h4>

```html
<h1 title="item1">Header 1</h1>
<h2 title="item2">Header 2</h2>
<h3 title="item3">Header 3</h3> 
```

<h4 style="font-family: Roboto">
<code>ul>li.item$$$*3</code>
</h4>

```html
<ul>
    <li class="item001"></li>
    <li class="item002"></li>
    <li class="item003"></li>
</ul>
```

<h4 style="font-family: Roboto">
<code>ul>li.item$@-*3</code>
</h4>

```html
<ul>
    <li class="item3"></li>
    <li class="item2"></li>
    <li class="item1"></li>
</ul>
```

<h4 style="font-family: Roboto">
<code>ul>li.item$@2*3</code> 
</h4>

```html
<ul>
    <li class="item2"></li>
    <li class="item3"></li>
    <li class="item4"></li>
</ul>
```