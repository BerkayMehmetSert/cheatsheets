<h1 align="center" style="font-family: Roboto">
CSS CHEAT SHEET
</h1>

<h3 style="font-family: Roboto"><code>align-content</code></h3>

<p style="font-family: Roboto">
Defines how each line is aligned within a flexbox/grid container. It only applies if <code>flex-wrap:</code> is present, and if there are multiple lines of flexbox/grid items.
</p>

```css
/* default */
align-content: stretch; 
```

<p style="font-family: Roboto">
Each line will stretch to fill the remaining space.
</p>

```css
align-content: flex-start;
```

<p style="font-family: Roboto">
Each line will only fill the space it needs. They will all move towards the <b>start</b> of the flexbox/grid container's cross axis.
</p>

```css
align-content: flex-end;
```

<p style="font-family: Roboto">
Each line will only fill the space it needs. They will all move towards the <b>end</b> of the flexbox/grid container's cross axis.
</p>

```css
align-content: center;
```

<p style="font-family: Roboto">
Each line will only fill the space it needs. They will all move towards the <b>center</b> of the flexbox/grid container's cross axis. 
</p>

```css
align-content: space-between;
```

<p style="font-family: Roboto">
Each line will only fill the space it needs. The remaining space will appear <b>between</b> the lines. 
</p>

```css
align-content: space-around;
```

<p style="font-family: Roboto">
Each line will only fill the space it needs. The remaining space will be distributed equally <b>around</b> the lines: before the first line, between the two, and after the last one.
</p>

<h3 style="font-family: Roboto"><code> align-items</code></h3>

<p style="font-family: Roboto">
Defines how flexbox items are aligned according to the <b>cross</b> axis, within a line of a flexbox container.
</p>

```css
align-items: flex-start;
```

<p style="font-family: Roboto">
The flexbox items are aligned at the <b>start</b> of the cross axis. 

By default, the cross axis is vertical. This means the flexbox items will be aligned vertically at the <i>top</i>.
</p>

```css
align-items: flex-end;
```

<p style="font-family: Roboto">
The flexbox items are aligned at the <b>end</b> of the cross axis.

By default, the cross axis is vertical. This means the flexbox items will be aligned vertically at the <i>bottom</i>.
</p>

```css
align-items: center;
```

<p style="font-family: Roboto">
The flexbox items are aligned at the <b>center</b> of the cross axis.

By default, the cross axis is vertical. This means the flexbox items will be <i>centered</i> vertically.
</p>

```css
align-items: baseline;
```

<p style="font-family: Roboto">
The flexbox items are aligned at the <b>baseline</b> of the cross axis.

By default, the cross axis is vertical. This means the flexbox items will align themselves in order to have the <i>baseline</i> of their text align along a horizontal line.
</p> 

```css
align-items: stretch;
```

<p style="font-family: Roboto">
The flexbox items will <b>stretch</b> across the whole cross axis.

By default, the cross axis is vertical. This means the flexbox items will fill up the whole <i>vertical space</i>.
</p>

<h3 style="font-family: Roboto"><code>align-self</code></h3>

<p style="font-family: Roboto">
Works like <code>align-items</code>, but applies only to a <b>single</b> flexbox item, instead of all of them. 
</p>

```css
/* default */
align-self: auto;
```

<p style="font-family: Roboto">
The target will use the value of <code>align-items</code>.
</p>

```css
align-self: flex-start;
```

<p style="font-family: Roboto">
If the container has <code>align-items: center</code> and the <b>target</b> has <code>align-self: flex-start</code>, only the target will be at the start of the cross axis.

By default, this means it will be aligned vertically at the <i>top</i>.
</p>

```css
align-self: flex-end;
```

<p style="font-family: Roboto">
If the container has <code>align-items: center</code> and the <b>target</b> has <code>align-self: flex-end</code>, only the target will be at the end of the cross axis.

By default, this means it will be aligned vertically at the <i>bottom</i>.
</p>

```css
align-self: center;
```

<p style="font-family: Roboto">
If the container has <code>align-items: flex-start</code> and the <b>target</b> has <code>align-self: center</code>, only the target will be at the center of the cross axis. 

By default, this means it will be vertically <i>centered</i>.
</p>

```css
align-self: baseline;
```

<p style="font-family: Roboto">
If the container has <code>align-items: center</code> and the <b>target</b> has <code>align-self: baseline</code>, only the target will be at the baseline of the cross axis.
</p>

```css
align-self: stretch;
```

<p style="font-family: Roboto">
If the container has <code>align-items: center</code> and the <b>target</b> has <code>align-self: stretch</code>, only the target will stretch along the whole cross axis.
</p>

<h3 style="font-family: Roboto"><code>animation-delay</code></h3>

<p style="font-family: Roboto">
Defines how long the animation has to wait before <b>starting</b>. The animation will only be delayed on its first iteration. 
</p>

```css
/* default */
animation-delay: 0s;
```

<p style="font-family: Roboto">
The animation will wait zero seconds, and thus start right away.
</p>

```css
animation-delay: 1.2s;
```

<p style="font-family: Roboto">
You can use decimal values in seconds with the keyword <code>s</code>.
</p>

```css
animation-delay: 2400ms;
```

<p style="font-family: Roboto">
You can use milliseconds instead of seconds, with the keyword <code>ms</code>.
</p>

```css
animation-delay: -500ms;
```

<p style="font-family: Roboto">
You can use negative values: the animation will start as if it had already been playing for <code>500ms</code>.
</p>

<h3 style="font-family: Roboto"><code>animation-direction</code></h3>

<p style="font-family: Roboto">
Defines in which direction the animation is played. 
</p>

```css
/* default */
animation-direction: normal;
```

<p style="font-family: Roboto">
The animation is played forwards. When it reaches the end, it starts over at the first keyframe.
</p>

```css
animation-direction: reverse;
```

<p style="font-family: Roboto">
The animation is played backwards: begins at the last keyframe, finishes at the first keyframe.
</p>

```css
animation-direction: alternate;
```

<p style="font-family: Roboto">
The animation is played forwards first, then backwards:
</p>
<li>starts at the first keyframe</li> 
<li>stops at the last keyframe</li>
<li>starts again, but at the last keyframe</li>
<li>stops at the first keyframe</li>

```css
animation-direction: alternate-reverse;
```

<p style="font-family: Roboto">
The animation is played backwards first, then forwards:
</p>
<li>starts at the last keyframe</li>
<li>stops at the first keyframe</li>
<li>starts again, but at the first keyframe</li>
<li>stops at the last keyframe</li>

<h3 style="font-family: Roboto"><code>animation-duration</code></h3>

<p style="font-family: Roboto">
Defines how long the animation lasts. 
</p>

```css
/* default */
animation-duration: 0s;
```

<p style="font-family: Roboto">
The default value is zero seconds: the animation will simply not play. 
</p>

```css
animation-duration: 1.2s;
```

<p style="font-family: Roboto">
You can use decimal values in seconds with the keyword <code>s</code>. 
</p>

```css
animation-duration: 2400ms;
```

<p style="font-family: Roboto">
You can use milliseconds instead of seconds, with the keyword <code>ms</code>. 
</p>

<h3 style="font-family: Roboto"><code>animation-fill-mode</code></h3>

<p style="font-family: Roboto">
Defines what happens before an animation starts and after it ends. The fill mode allows to tell the browser if the animation’s styles should also be applied <i>outside</i> of the animation. 
</p>

```css
/* default */
animation-fill-mode: none;
```

<p style="font-family: Roboto">
The animation styles do not affect the <i>default</i> style: the element is set to its default state before the animation starts, and returns to that default state after the animation ends. 
</p>

```css
animation-fill-mode: forwards;
```

<p style="font-family: Roboto">
The last styles applied at the end of the animation are retained afterwards. 
</p>

```css
animation-fill-mode: backwards;
```

<p style="font-family: Roboto">
The animation's styles will already be applied before the animation actually starts. 
</p>

```css
animation-fill-mode: both;
```

<p style="font-family: Roboto">
The styles are applied before and after the animation plays. 
</p>

<h3 style="font-family: Roboto"><code>animation-iteration-count</code></h3>

<p style="font-family: Roboto">
Defines how many times the animation is played. 
</p>

```css
/* default */
animation-iteration-count: 1;
```

<p style="font-family: Roboto">
The animation will only play once. 
</p>

```css  
animation-iteration-count: 2;
```

<p style="font-family: Roboto">
You can use integer values to define a specific amount of times the animation will play.
</p>

```css
animation-iteration-count: infinite;
```

<p style="font-family: Roboto">
By using the keyword <code>infinite</code>, the animation will play indefinitely. 
</p>

<h3 style="font-family: Roboto"><code>animation-name</code></h3>

<p style="font-family: Roboto">
Defines which animation keyframes to use. 
</p>

```css
/* default */
animation-name: none;
```

<p style="font-family: Roboto">
If no animation name is specified, no animation is played. 
</p>

```css
animation-name: fadeIn;
```

<p style="font-family: Roboto">
If a name is specified, the keyframes matching that name will be used. 
</p>

<h3 style="font-family: Roboto"><code>animation-play-state</code></h3>

<p style="font-family: Roboto">
Defines if an animation is playing or not. 
</p>

```css
/* default */
animation-play-state: running;
```

<p style="font-family: Roboto">
If the <code>animation-duration</code> and <code>animation-name</code> are defined, the animation will start playing automatically. 
</p>

```css
animation-play-state: paused;
```

<p style="font-family: Roboto">
The animation is set paused at the first keyframe. 
</p> 

<h3 style="font-family: Roboto"><code>animation-timing-function</code></h3> 

<p style="font-family: Roboto"> 
Defines how the values between the start and the end of the animation are calculated. 
</p>

```css
/* default */
animation-timing-function: ease;
```

<p style="font-family: Roboto">
The animation starts slowly, accelerates in the middle, and slows down at the end. 
</p>

```css
animation-timing-function: ease-in; 
```

<p style="font-family: Roboto">
The animation starts slowly, and accelerates gradually until the end. 
</p>

```css
animation-timing-function: ease-out;
```

<p style="font-family: Roboto">
The animation starts quickly, and decelerates gradually until the end. 
</p>

```css
animation-timing-function: ease-in-out;
```

<p style="font-family: Roboto">
Like <code>ease</code>, but more pronounced.

The animation starts quickly, and decelerates gradually until the end. 
</p>

<h3 style="font-family: Roboto"><code>animation</code></h3>

<p style="font-family: Roboto">
Shorthand property for <code>animation-name</code> <code>animation-duration</code> <code>animation-timing-function</code> <code>animation-delay</code> <code>animation-iteration-count</code> <code>animation-direction</code> <code>animation-fill-mode</code> and <code>animation-play-state</code>.

Only <code>animation-duration</code> and <code>animation-name</code> are required. 
</p>

<h3 style="font-family: Roboto"><code>background-attachment</code></h3>

<p style="font-family: Roboto">
Defines how the background image will behave when scrolling the page. 
</p>

```css
/* default */
background-attachment: scroll;
``` 

<p style="font-family: Roboto">
The background image will scroll with the page. It will also position and resize itself according to the element it's applied to. 
</p>

```css 
background-attachment: fixed;
```

<p style="font-family: Roboto">
The background image will not scroll with the page, and remain positioned according to the viewport. It will also position and resize itself according to the viewport. As a result, the background image will probably only be partially visible. 
</p>

<h3 style="font-family: Roboto"><code>background-clip</code></h3>

<p style="font-family: Roboto">
Defines how far the background should extend within the element. 
</p>

```css
/* default */
background-clip: border-box;
```

<p style="font-family: Roboto">
The background extends completely throughout the element, even under the border. 
</p>

```css
background-clip: padding-box;
```

<p style="font-family: Roboto">
The background only extends to the edge of the border: it includes the padding but not the border. 
</p>

```css
background-clip: content-box;
```

<p style="font-family: Roboto">
The background only extends to the edge of the content: it doesn't include the padding, nor the border. 
</p>

<h3 style="font-family: Roboto"><code>background-color</code></h3>

<p style="font-family: Roboto">
Defines the color of the element's background. 
</p>

```css
/* default */
background-color: transparent;
```

<p style="font-family: Roboto">
By default, the background color is transparent, basically meaning that there is no background color. 
</p>

```css
background-color: red;
```

<p style="font-family: Roboto">
You can use one of the 140+ color names. 
</p>

```css
background-color: #05ffb0;
```

<p style="font-family: Roboto">
You can use hexadecimal color codes. 
</p>

```css
background-color: rgb(50, 115, 220);
```

<p style="font-family: Roboto">
You can use rgb() color codes:
</p>
<li>the first value is for <code>red</code></li>
<li>the second value is for <code>green</code></li>
<li>the third value is for <code>blue</code></li>
<p style="font-family: Roboto">Each of them can have a value between 0 and 255.
</p>

```css
background-color: rgba(50, 115, 220, 0.3);
```

<p style="font-family: Roboto">
You can use rgba() color codes:
</p>
<li>the first 3 values are for <code>rgb</code></li>
<li>the 4th value is for the <code>alpha</code> channel and defines the opacity of the color</li>
<p style="font-family: Roboto">The alpha value can go from zero 0 (transparent) to one 1 (opaque).
</p>

```css
background-color: hsl(14, 100%, 53%);
```

<p style="font-family: Roboto">
You can use hsl() color codes: 
</p>
<li>the first value is for <code>hue</code> and can go from 0 to 359</li>
<li>the second value is for <code>saturation</code> and go from 0% to 100%</li>
<li>the third value is for <code>luminosity</code> and go from 0% to 100%</li>

```css
background-color: hsla(14, 100%, 53%, 0.6);
```

<p style="font-family: Roboto">
You can use hsla() color codes:
</p>
<li>the first 3 values are for <code>hsl</code></li>
<li>the 4th value is for the <code>alpha</code> channel and defines the opacity of the color</li>

<h3 style="font-family: Roboto"><code>background-image</code></h3>

<p style="font-family: Roboto">
Defines an image as the background of the element. 
</p>

```css
/* default */
background-image: none;
```

<p style="font-family: Roboto">
Removes any background image. 
</p>

```css
background-image: url(/images/jt.png);
```

<p style="font-family: Roboto">
Uses the image defined in the url path. This path can either be relative (to the css file) or absolute. 
</p>

```css
background-image: linear-gradient(red, blue);
```

<p style="font-family: Roboto">
You can define a linear gradient as the background image.

You need to define at least two colors. The first one will start at the top, the second one at the bottom.

The default angle is to bottom (or 180deg), which means the gradient is vertical, starting at the top, ending at the bottom of the element.
</p>

```css
background-image: linear-gradient(45deg, red, blue);
```

<p style="font-family: Roboto">
You can specify an angle, either in degrees, or with keywords.

When using degress, you specify the direction of the gradient, or when it ends. So 0deg means the the top of the element, like 12:00 on a clock.

In this example, 45deg means 2:30, or the top right corner. 
</p> 

```css
background-image: radial-gradient(green, purple);
```

<p style="font-family: Roboto">
You can define a radial gradient as the background image.

You need to define at least two colors. The first one will be at the center, the second one at the edges. 
</p>

```css
background-image: radial-gradient(circle, green, purple);
```

<p style="font-family: Roboto">
You can specify the shape of the radial gradient: circle or ellipse (default). 
</p>

<h3 style="font-family: Roboto"><code>background-origin</code></h3>

<p style="font-family: Roboto">
Defines the origin of the background image. 
</p>

```css
/* default */
background-origin: padding-box;
```

<p style="font-family: Roboto">
The background image starts at the edge of the border: within padding but not the border. 
</p>

```css
background-origin: border-box;
```

<p style="font-family: Roboto">
The background image starts under the border. 
</p>

```css
background-origin: content-box; 
```

<p style="font-family: Roboto">
The background image only starts at the edge of the content: it doesn't include the padding, nor the border. 
</p> 

<h3 style="font-family: Roboto"><code>background-position</code></h3>

<p style="font-family: Roboto">
Defines the position of the background image. 
</p>

```css
/* default */
background-position: 0% 0%; 
```

<p style="font-family: Roboto">
The background image will be positioned at 0% on the horizontal axis and 0% on the vertical axis, which means the top left corner of the element. 
</p>

```css
background-position: bottom right; 
```

<p style="font-family: Roboto">
You can use a combination of position keywords: <code>center</code>, <code>top</code>, <code>bottom</code>, <code>left</code> and <code>right</code>. 
</p>

```css
background-position: center center;
```

<p style="font-family: Roboto">
The background image will be positioned in the center of the element. 
</p>

<h3 style="font-family: Roboto"><code>background-repeat</code></h3>

<p style="font-family: Roboto">
Defines how the background image repeats itself across the element's background, starting from the background position. 
</p>

```css
/* default */
background-repeat: repeat;  
```

<p style="font-family: Roboto">
The background image will repeat itself both horizontally and vertically. 
</p>

```css
background-repeat: repeat-x; 
```

<p style="font-family: Roboto">
The background image will only repeat itself horizontally. 
</p>

```css
background-repeat: repeat-y; 
```

<p style="font-family: Roboto">
The background image will only repeat itself vertically. 
</p> 

```css
background-repeat: no-repeat; 
```

<p style="font-family: Roboto">
The background image will only appear once. 
</p> 

<h3 style="font-family: Roboto"><code>background-size</code></h3>

<p style="font-family: Roboto">
Defines the size of the background image. 
</p>

```css
/* default */
background-size: auto auto; 
```

<p style="font-family: Roboto">
The background image will retain its original size. 
</p>

```css
background-size: contain; 
```

<p style="font-family: Roboto">
The keyword <code>contain</code> will resize the background image to make sure it remains fully visible. 
</p>

```css
background-size: cover; 
```

<p style="font-family: Roboto">
The keyword <code>cover</code> will resize the background image to make sure the element is fully covered. 
</p> 

<h3 style="font-family: Roboto"><code>background</code></h3>

<p style="font-family: Roboto">
Shorthand property for <code>background-image</code> <code>background-position</code> <code>background-size</code> <code>background-repeat</code> <code>background-origin</code> <code>background-clip</code> <code>background-attachment</code> and <code>background-color</code>. 
</p>

<h3 style="font-family: Roboto"><code>border-bottom-color</code></h3>

<p style="font-family: Roboto">
Like <code>border-color</code>, but for the bottom border only. 
</p>

```css
border-bottom-color: transparent; 
```

<p style="font-family: Roboto">
Applies a transparent color to the bottom border. The bottom border will still take up the space defined by the <code>border-width</code> value. 
</p>

```css
border-bottom-color: red; 
```

<p style="font-family: Roboto">
You can use one of the 140+ color names. 
</p>

```css
border-bottom-color: #05ffb0;
```

<p style="font-family: Roboto">
You can use hexadecimal color codes, <code>rgb()</code>, <code>rgba()</code>, <code>hsl()</code>, <code>hsla()</code>... 
</p>

<h3 style="font-family: Roboto"><code>border-bottom-left-radius</code></h3>

<p style="font-family: Roboto">
Defines the radius of the bottom left corner. 
</p>

```css
/* default */
border-bottom-left-radius: 0; 
``` 

<p style="font-family: Roboto">
Removes any border radius. 
</p>

```css
border-bottom-left-radius: 20px; 
```

<p style="font-family: Roboto">
You can use pixel values. 
</p>

```css
border-bottom-left-radius: 50%; 
```

<p style="font-family: Roboto">
You can use percentage values. In this example, the radius starts halfway on the bottom border, and ends halfway on the left border. 
</p>

```css
border-bottom-left-radius: 20px 50%; 
```

<p style="font-family: Roboto">
If you set two values, the first one is for the bottom border, the second one for the left border. 
</p>

<h3 style="font-family: Roboto"><code>border-bottom-right-radius</code></h3>

<p style="font-family: Roboto">
Defines the radius of the bottom right corner. 
</p>

```css
/* default */
border-bottom-right-radius: 0; 
``` 

<p style="font-family: Roboto">
Removes any border radius. 
</p>

```css
border-bottom-right-radius: 20px; 
```

<p style="font-family: Roboto">
You can use pixel values. 
</p>

```css
border-bottom-right-radius: 50%; 
```

<p style="font-family: Roboto">
You can use percentage values. In this example, the radius starts halfway on the bottom border, and ends halfway on the right border. 
</p>

```css
border-bottom-right-radius: 20px 50%; 
```

<p style="font-family: Roboto">
If you set two values, the first one is for the bottom border, the second one for the right border. 
</p>

<h3 style="font-family: Roboto"><code>border-bottom-style</code></h3>

<p style="font-family: Roboto">
Like <code>border-style</code>, but for the bottom border only. 
</p>

```css
/* default */
border-bottom-style: none; 
```

<p style="font-family: Roboto">
Removes the bottom border. 
</p>

```css
border-bottom-style: dotted; 
```

<p style="font-family: Roboto">
Turns the bottom border into a sequence of dots. 
</p>

```css
border-bottom-style: dashed; 
```

<p style="font-family: Roboto">
Turns the bottom border into a sequence of dashes. 
</p>

```css
border-bottom-style: solid; 
```

<p style="font-family: Roboto">
Turns the bottom border into a solid line. 
</p>

```css
border-bottom-style: double; 
```

<p style="font-family: Roboto">
Splits the bottom border into two lines. 
</p> 

<h3 style="font-family: Roboto"><code>border-bottom-width</code></h3>

<p style="font-family: Roboto">
Like <code>border-width</code>, but for the bottom border only. 
</p>

```css
/* default */
border-bottom-width: 0; 
```

<p style="font-family: Roboto">
Removes the bottom border. 
</p>

```css
border-bottom-width: 4px; 
```

<p style="font-family: Roboto">
You can use pixel values. 
</p>

<h3 style="font-family: Roboto"><code>border-bottom</code></h3>

<p style="font-family: Roboto">
border-bottom
Shorthand property for <code>border-bottom-width</code> <code>border-bottom-style</code> and <code>border-bottom-color</code>. 
</p>

<h3 style="font-family: Roboto"><code>border-collapse</code></h3>

<p style="font-family: Roboto">
Defines whether table borders should be separated or collapsed. 
</p>

```css 
/* default */
border-collapse: separate; 
```

<p style="font-family: Roboto">
Each table cell will display its own borders. 
</p>

```css
border-collapse: collapse; 
```

<p style="font-family: Roboto">
Adjacent table cells will merge their borders together. 
</p> 

<h3 style="font-family: Roboto"><code>border-color</code></h3>

<p style="font-family: Roboto">
Defines the color of the element's borders. 
</p>

```css
/* default */
border-color: transparent; 
```

<p style="font-family: Roboto">
Applies a transparent color to the borders. The borders will still take up the space defined by the border-width value. 
</p>

```css
border-color: red; 
```

<p style="font-family: Roboto"> 
You can use one of the 140+ color names. 
</p>

```css
border-color: #05ffb0; 
```

<p style="font-family: Roboto">
You can use hexadecimal color codes. 
</p>

```css
border-color: #05ffb0;
```

<p style="font-family: Roboto">
You can use hexadecimal color codes, <code>rgb()</code>, <code>rgba()</code>, <code>hsl()</code>, <code>hsla()</code>... 
</p>

<h3 style="font-family: Roboto"><code>border-left-color</code></h3>

<p style="font-family: Roboto">
Like <code>border-color</code>, but for the left border only. 
</p>

```css
/* default */
border-left-color: transparent;
```

<p style="font-family: Roboto">
Applies a transparent color to the left border. The left border will still take up the space defined by the border-width value. 
</p>

```css
border-left-color: red; 
``` 

<p style="font-family: Roboto">
You can use one of the 140+ color names. 
</p>

```css 
border-left-color: #05ffb0; 
```

<p style="font-family: Roboto">
You can use hexadecimal color codes, <code>rgb()</code>, <code>rgba()</code>, <code>hsl()</code>, <code>hsla()</code>... 
</p>

<h3 style="font-family: Roboto"><code>border-left-style</code></h3>

<p style="font-family: Roboto">
Like <code>border-style</code>, but for the left border only. 
</p>

```css
/* default */
border-left-style: none; 
```

<p style="font-family: Roboto">
Removes the left border. 
</p>

```css 
border-left-style: dotted; 
```

<p style="font-family: Roboto">
Turns the left border into a sequence of dots. 
</p>

```css
border-left-style: dashed; 
```

<p style="font-family: Roboto">
Turns the left border into a sequence of dashes. 
</p>

```css 
border-left-style: solid; 
```

<p style="font-family: Roboto"> 
Turns the left border into a solid line. 
</p>

```css
border-left-style: double; 
``` 

<p style="font-family: Roboto">
Splits the left border into two lines. 
</p>

<h3 style="font-family: Roboto"><code>border-left-width</code></h3> 

<p style="font-family: Roboto">
Like <code>border-width</code>, but for the left border only. 
</p>

```css 
/* default */
border-left-width: 0; 
```

<p style="font-family: Roboto">
Removes the left border.  
</p>

```css 
border-left-width: 4px; 
``` 

<p style="font-family: Roboto">
You can use pixel values. 
</p> 

<h3 style="font-family: Roboto"><code>border-left</code></h3>

<p style="font-family: Roboto">
Shorthand property for <code>border-left-width</code> <code>border-left-style</code> and <code>border-left-color</code>. 
</p> 

<h3 style="font-family: Roboto"><code>border-radius</code></h3>

<p style="font-family: Roboto">
Defines the radius of the element's corners. 
</p>

```css
/* default */
border-radius: 0; 
```

<p style="font-family: Roboto">
Removes any border radius. 
</p>

```css
border-radius: 20px; 
```

<p style="font-family: Roboto">
You can use pixel values. 
</p>

```css
border-radius: 50%; 
```

<p style="font-family: Roboto">
You can use percentage values. In this example, the radius starts halfway through each border. 
</p>

<h3 style="font-family: Roboto"><code>border-right-color</code></h3> 

<p style="font-family: Roboto">
Like <code>border-color</code>, but for the right border only. 
</p>

```css
/* default */ 
border-right-color: transparent; 
```

<p style="font-family: Roboto"> 
Applies a transparent color to the right border. The right border will still take up the space defined by the <code>border-width</code> value. 
</p>

```css
border-right-color: red; 
```

<p style="font-family: Roboto">
You can use one of the 140+ color names. 
</p>

```css
border-right-color: #05ffb0; 
``` 

<p style="font-family: Roboto">
You can use hexadecimal color codes, <code>rgb()</code>, <code>rgba()</code>, <code>hsl()</code>, <code>hsla()</code>... 
</p> 

<h3 style="font-family: Roboto"><code>border-right-style</code></h3> 

<p style="font-family: Roboto"> 
Like <code>border-style</code>, but for the right border only. 
</p>

```css 
/* default */
border-right-style: none; 
```

<p style="font-family: Roboto">
Removes the right border. 
</p>

```css
border-right-style: dotted; 
```

<p style="font-family: Roboto">
Turns the right border into a sequence of dots. 
</p>

```css
border-right-style: dashed; 
``` 

<p style="font-family: Roboto">
Turns the right border into a sequence of dashes. 
</p>

```css 
border-right-style: solid; 
``` 

<p style="font-family: Roboto">
Turns the right border into a solid line. 
</p>

```css
border-right-style: double; 
```

<p style="font-family: Roboto">
Splits the right border into two lines. 
</p>

<h3 style="font-family: Roboto"><code>border-right-width</code></h3> 

<p style="font-family: Roboto">
Like <code>border-width</code>, but for the right border only. 
</p>

```css
/* default */
border-right-width: 0; 
```

<p style="font-family: Roboto"> 
Removes the right border. 
</p>

```css 
border-right-width: 4px; 
```

<p style="font-family: Roboto">
You can use pixel values. 
</p> 

<h3 style="font-family: Roboto"><code>border-right</code></h3> 

<p style="font-family: Roboto">
Shorthand property for <code>border-right-width</code> <code>border-right-style</code> and <code>border-right-color</code>. 
</p> 

<h3 style="font-family: Roboto"><code>border-top-color</code></h3>

<p style="font-family: Roboto"> 
Like <code>border-color</code>, but for the top border only. 
</p>

```css
/* default */
border-top-color: transparent; 
```

<p style="font-family: Roboto"> 
Applies a transparent color to the top border. The top border will still take up the space defined by the <code>border-width</code> value. 
</p>

```css
border-top-color: red; 
```

<p style="font-family: Roboto">
You can use one of the 140+ color names. 
</p>

```css
border-top-color: #05ffb0; 
``` 

<p style="font-family: Roboto"> 
You can use hexadecimal color codes, <code>rgb()</code>, <code>rgba()</code>, <code>hsl()</code>, <code>hsla()</code>... 
</p> 

<h3 style="font-family: Roboto"><code>border-top-style</code></h3> 

<p style="font-family: Roboto">
Like <code>border-style</code>, but for the top border only. 
</p>

```css 
/* default */
border-top-style: none; 
``` 

<p style="font-family: Roboto"> 
Removes the top border. 
</p>

```css 
border-top-style: dotted; 
```

<p style="font-family: Roboto"> 
Turns the top border into a sequence of dots. 
</p>

```css 
border-top-style: dashed; 
```

<p style="font-family: Roboto">
Turns the top border into a sequence of dashes. 
</p>

```css
border-top-style: solid; 
```

<p style="font-family: Roboto">
Turns the top border into a solid line. 
</p>

```css
border-top-style: double; 
```

<p style="font-family: Roboto">
Splits the top border into two lines. 
</p> 

<h3 style="font-family: Roboto"><code>border-top-width</code></h3> 

<p style="font-family: Roboto">
Like <code>border-width</code>, but for the top border only. 
</p>

```css 
/* default */
border-top-width: 0; 
``` 

<p style="font-family: Roboto"> 
Removes the top border. 
</p>

```css 
border-top-width: 4px; 
``` 

<p style="font-family: Roboto"> 
You can use pixel values. 
</p>

<h3 style="font-family: Roboto"><code>border-top</code></h3> 

<p style="font-family: Roboto"> 
Shorthand property for <code>border-top-width</code> <code>border-top-style</code> and <code>border-top-color</code>. 
</p> 

<h3 style="font-family: Roboto"><code>border-width</code></h3> 

<p style="font-family: Roboto"> 
Defines the width of the element's borders. 
</p>

```css
border-width: 1px; 
```

<p style="font-family: Roboto">
Defines the width of all borders to 1px.   
</p>

```css 
border-width: 2px 0; 
```

<p style="font-family: Roboto"> 
Defines the top and bottom borders to 2px, the left and right to 0. 
</p>

<h3 style="font-family: Roboto"><code>border</code></h3>

<p style="font-family: Roboto">
Shorthand property for <code>border-width</code> <code>border-style</code> and <code>border-color</code>. 
</p>

<h3 style="font-family: Roboto"><code>bottom</code></h3>

<p style="font-family: Roboto">
Defines the position of the element according to its bottom edge. 
</p>

```css
/* default */
bottom: auto; 
``` 

<p style="font-family: Roboto">
The element will remain in its natural position.
</p>

```css
bottom: 20px; 
```

<p style="font-family: Roboto">
If the element is in position relative, the element will move upwards by the amount defined by the bottom value. 
</p> 

```css
bottom: 0; 
```

<p style="font-family: Roboto">
If the element is in position absolute, the element will position itself from the bottom of the first positioned ancestor. 
</p> 

<h3 style="font-family: Roboto"><code>box-shadow</code></h3>

<p style="font-family: Roboto">
Defines the shadow of the element. 
</p>

```css
/* default */
box-shadow: none; 
```

<p style="font-family: Roboto">
Removes any box-shadow that was applied to the element. 
</p>

```css
box-shadow: 2px 4px 10px 4px red; 
```

<p style="font-family: Roboto">
The optional fourth value defines the spread of the shadow.

The spread defines how much the shadow should grow: it enhances the shadow. 
</p>

<h3 style="font-family: Roboto"><code>box-sizing</code></h3>

<p style="font-family: Roboto">
Defines how the width and height of the element are calculated: whether they include the padding and borders or not. 
</p>

```css
/* default */
box-sizing: content-box; 
```

<p style="font-family: Roboto">
The width and height of the element only apply to the content of the element. 
</p>

```css
box-sizing: border-box; 
```

<p style="font-family: Roboto">
The width and height of the element apply to all parts of the element: the content, the padding and the borders. 
</p>

<h3 style="font-family: Roboto"><code>color</code></h3>

<p style="font-family: Roboto">
Defines the color of the text. 
</p>

```css
color: transparent; 
```

<p style="font-family: Roboto">
Applies a transparent color to the text. The text will still take up the space it should. 
</p>

```css
color: red; 
```

<p style="font-family: Roboto">
You can use one of the 140+ color names. 
</p>

```css
color: #05ffb0; 
```

<p style="font-family: Roboto">
You can use hexadecimal color codes, <code>rgb()</code>, <code>rgba()</code>, <code>hsl()</code>, <code>hsla()</code>... 
</p>

<h3 style="font-family: Roboto"><code>column-count</code></h3>

<p style="font-family: Roboto">
Defines the number of columns of the element. 
</p>

```css
/* default */
column-count: auto; 
```

<p style="font-family: Roboto">
Removes any columns from the element (unless another <code>column-</code> property was set).
</p>  

```css
column-count: 3; 
```

<p style="font-family: Roboto">
When using an integer value, the element will distribute its child elements across the number of columns defined. 
</p>

<h3 style="font-family: Roboto"><code>column-gap</code></h3>

<p style="font-family: Roboto">
Defines the gap between the columns of the element. 
</p>

```css
/* default */
column-gap: normal; 
```

<p style="font-family: Roboto">
The gap between the columns is set to the browser's default value, which usually is 1em. 
</p>

```css
column-gap: 2px; 
```

<p style="font-family: Roboto">
You can use pixel values for the gap.

Note that the gap only appears <i>between</i> columns, and not on the exterior sides of the edge columns.
</p>

<h3 style="font-family: Roboto"><code>column-width</code></h3>

<p style="font-family: Roboto">
Defines the number of columns of the element. 
</p>

```css
/* default */
column-width: auto; 
```

<p style="font-family: Roboto">
The element will not distribute its child elements into columns, unlesse a <code>column-count</code> value is defined. In that case, the column width will be infered from the column count. 
</p>

```css
column-width: 10px; 
```

<p style="font-family: Roboto">
You can use pixel values for the column width.

The number of columns will be the minimum needed to distribute all the content across the element. 
</p>

<h3 style="font-family: Roboto"><code>content</code></h3>

<p style="font-family: Roboto">
Defines the text content of the <code>:before</code> and <code>:after</code>pseudo-elements. 
</p>

```css
/* default */
content: normal; 
```

<p style="font-family: Roboto">
No content is added to the element. 
</p>

```css
content: "Foo bar"; 
```

<p style="font-family: Roboto">
The text content will be prepended to the element's content.

Notice how the end result combines text from the HTML and text from the CSS. 
</p>

```css
content: url(/images/jt.png); 
```

<p style="font-family: Roboto">
You can insert images by using the <code>url()</code> function. 
</p>

<h3 style="font-family: Roboto"><code>cursor</code></h3>

<p style="font-family: Roboto">
Sets the mouse cursor when hovering the element. 
</p>

```css
cursor: default; 
```

<p style="font-family: Roboto">
Sets the cursor to the element's default value. For a link, it would be a pointer. For text it would be a selection cursor. 
</p>

```css
cursor: auto; 
cursor: pointer;
cursor: move;
cursor: crosshair;
cursor: text;
cursor: wait;
cursor: help-resize;
cursor: ne-resize;
cursor: nw-resize;
cursor: n-resize;
cursor: se-resize;
cursor: sw-resize;
cursor: s-resize;
cursor: w-resize; 
```

<p style="font-family: Roboto">
Auto, pointer, move, crosshair, text, wait, help-resize, ne-resize, nw-resize, n-resize, se-resize, sw-resize, s-resize, w-resize. 
</p>

<h3 style="font-family: Roboto"><code>display</code></h3>

<p style="font-family: Roboto">
Sets the display behavior of the element. 
</p>

```css
display: none; 
```

<p style="font-family: Roboto">
The element is completely removed, as if it wasn't in the HTML code in the first place. 
</p>

```css
display: inline; 
```

<p style="font-family: Roboto">
The element is turned into an inline element: it behaves like simple text.

Any <code>height</code> and <code>width</code> applied will have no effect.
</p>

```css
display: block; 
```

<p style="font-family: Roboto">
The element is turned into a block element: it starts on a new line, and takes up the whole width. 
</p>

```css
display: inline-block; 
```

<p style="font-family: Roboto">
Inline because the element behaves like simple text, and inserts itself in a block of text. 

Block because you can apply height and width values.
</p>

```css
display: flex; 
```

<p style="font-family: Roboto">
The element is turned into an flexbox container. On its own, it behaves like a block element.

Its child elements will be turned into flexbox items. 
</p>

```css
display: inline-flex; 
``` 

<p style="font-family: Roboto">
Inline because the element behaves like simple text, and inserts itself in a block of text. 

Flexbox because its child element will be turned into flexbox items. 
</p> 

```css
display: grid; 
``` 

<p style="font-family: Roboto">
The element is turned into an grid container. On its own, it behaves like a block element.

Its child elements will be turned into grid items. 
</p>

```css
display: inline-grid; 
``` 

<p style="font-family: Roboto">
Inline because the element behaves like simple text, and inserts itself in a block of text.
Grid because its child element will be turned into flexbox items. 
</p>

<h3 style="font-family: Roboto"><code>flex-basis</code></h3>

<p style="font-family: Roboto">
Defines the initial size of a flexbox item. 
</p>

```css
/* default */
flex-basis: auto; 
```

<p style="font-family: Roboto">
The element will be automatically sized based on its content, or on any <code>height</code> or <code>width</code> value if they are defined. 
</p>

```css
flex-basis: 80px; 
```

<p style="font-family: Roboto">
You can define pixel or (r)em values. The element will wrap its content to avoid any overflow. 
</p>

<h3 style="font-family: Roboto"><code>flex-direction</code></h3>

<p style="font-family: Roboto">
Defines how flexbox items are ordered within a flexbox container. 
</p>

```css
/* default */
flex-direction: row; 
```

<p style="font-family: Roboto">
The flexbox items are ordered the same way as the text direction, along the main axis. 
</p>

```css
flex-direction: row-reverse; 
```

<p style="font-family: Roboto">
The flexbox items are ordered the opposite way as the text direction, along the main axis. 
</p>

```css
flex-direction: column; 
```

<p style="font-family: Roboto">
The flexbox items are ordered the same way as the text direction, along the cross axis.   
</p>

```css
flex-direction: column-reverse; 
```

<p style="font-family: Roboto">
The flexbox items are ordered the opposite way as the text direction, along the cross axis. 
</p>

<h3 style="font-family: Roboto"><code>flex-grow</code></h3>

<p style="font-family: Roboto">
Defines how much a flexbox item should grow if there's space available. 
</p>

```css
/* default */
flex-grow: 0; 
``` 

<p style="font-family: Roboto">
The element will not grow if there's space available. It will only use the space it needs. 
</p>

```css
flex-grow: 1; 
``` 

<p style="font-family: Roboto">
The element will grow by a factor of 1. It will fill up the remaining space if no other flexbox item has a <code>flex-grow</code> value. 
</p>

<h3 style="font-family: Roboto"><code>flex-shrink</code></h3>

<p style="font-family: Roboto">
Defines how much a flexbox item should shrink if there's not enough space available. 
</p>

```css
/* default */
flex-shrink: 1; 
```

<p style="font-family: Roboto">
If there's not enough space available in the container's main axis, the element will shrink by a factor of 1, and will wrap its content. 
</p>

```css
flex-shrink: 0;
```

<p style="font-family: Roboto">
The element will not shrink: it will retain the width it needs, and not wrap its content. Its siblings will shrink to give space to the target element.

Because the target element will not wrap its content, there is a chance for the flexbox container's content to overflow. 
</p> 

<h3 style="font-family: Roboto"><code>flex-wrap</code></h3>

<p style="font-family: Roboto">
Defines if flexbox items appear on a single line or on multiple lines within a flexbox container. 
</p>

```css
/* default */
flex-wrap: nowrap; 
```

<p style="font-family: Roboto">
The flexbox items will remain on a single line, no matter what, and will eventually overflow if needed. 
</p>

```css
flex-wrap: wrap; 
```

<p style="font-family: Roboto">
The flexbox items will be distributed among multiple lines if needed. 
</p>

```css
flex-wrap: wrap-reverse; 
```

<p style="font-family: Roboto">
The flexbox items will be distributed among multiple lines if needed. Any additional line will appear before the previous one. 
</p>

<h3 style="font-family: Roboto"><code>float</code></h3>

<p style="font-family: Roboto">
Pushes the element to either the left or right side. The following siblings will wrap around the floating element. 
</p>

```css
/* default */
float: none; 
```

<p style="font-family: Roboto">
Removes any previously defined float value. The element will remain in the natural flow of the page. 
</p>

```css
float: left; 
```

<p style="font-family: Roboto">
Moves the element to the left side of its container. The following elements will wrap around it and fill the space remaining on the right. 
</p>

```css
float: right; 
```

<p style="font-family: Roboto">
Moves the element to the right side of its container. The following elements will wrap around it and fill the space remaining on the left. 
</p>

<h3 style="font-family: Roboto"><code>font-famly</code></h3>

```css
font-family: "Source Sans Pro", "Arial", sans-serif; 
```

<p style="font-family: Roboto">
When using multiple values, the font-family list of font families defines the priority in which the browser should choose the font family.

The browser will look for each family on the user's computer and in any `@font-face` resource.

The list is prioritized from left to right: it will use the first value if it's available, or go to the next one, until the end of the list is reached. The default font family is defined by the browser preferences.

In this example, the browser will try to use Source Sans Pro if it's available. If it can't find it, it will try to use Arial. If it's not available either, it will use the browser's sans-serif font. 
</p>

```css
font-family: serif; 
```

<p style="font-family: Roboto">
The browser will use a serif font family: all characters have stroke endings. 
</p>

```css
font-family: sans-serif; 
```

<p style="font-family: Roboto">
The browser will use a sans-serif font family: no character has stroke endings. 
</p>

```css
font-family: monospace; 
```

<p style="font-family: Roboto">
The browser will use a monospace font family: all characters have the same width. 
</p> 

```css
font-family: cursive; 
```

<p style="font-family: Roboto">
The browser will use a cursive font family. 
</p>

```css
font-family: fantasy; 
```

<p style="font-family: Roboto">
The browser will use a fantasy font family. 
</p>

<h3 style="font-family: Roboto"><code>font-size</code></h3>

<p style="font-family: Roboto">
Defines the size of the text. 
</p>

```css
/* default */
font-size: medium; 
```

<p style="font-family: Roboto">
The text will use the browser's default medium size. 
</p>

```css
font-size: 20px; 
```

<p style="font-family: Roboto">
You can use pixel values. 
</p>

```css
font-size: 1.2em; 
```

<p style="font-family: Roboto">
You can use em values.

The value is relative to the parent's font-size.
As a result, the value will cascade if used on child elements. 
</p>

<h3 style="font-family: Roboto"><code>font-style</code></h3>

<p style="font-family: Roboto">
Defines how much the text is slanted. 
</p>

```css
/* default */
font-style: normal; 
```

<p style="font-family: Roboto">
The text is not slanted. 
</p>

```css
font-style: italic; 
```

<p style="font-family: Roboto">
Use the italic version of the font: the letters are slightly slanted. 
</p>

```css
font-style: oblique; 
```

<p style="font-family: Roboto">
Use the oblique version of the font: the letters are more slanted than italic. 
</p>

<h3 style="font-family: Roboto"><code>font-weight</code></h3>

<p style="font-family: Roboto">
Defines the weight of the text. 
</p>

```css
/* default */
font-weight: normal; 
```

<p style="font-family: Roboto">
The text is in normal weight. 
</p>

```css
font-weight: bold; 
```

<p style="font-family: Roboto">
The text becomes bold. 
</p>

```css
font-weight: 600; 
```

<p style="font-family: Roboto">
100 to 900 are valid values. 
</p>

<h3 style="font-family: Roboto"><code>font-variant</code></h3>

<p style="font-family: Roboto">
Defines which glyph to use for each letter. 
</p>

```css
/* default */
font-variant: normal; 
```

<p style="font-family: Roboto">
Each letter uses its normal glyph. 
</p>

```css
font-variant: small-caps; 
```

<p style="font-family: Roboto">
Each letter uses its small capitalized version. 
</p>

<h3 style="font-family: Roboto"><code>font</code></h3>

<p style="font-family: Roboto">
Shorthand property for <code>font-style</code>, <code>font-variant</code>, <code>font-weight</code>, <code>font-size</code>, <code>line-height</code>, and <code>font-family</code>. 
</p>

<h3 style="font-family: Roboto"><code>grid-area</code></h3>

<p style="font-family: Roboto">
Shorthand property for <code>grid-row-start</code>, <code>grid-column-start</code>, <code>grid-row-end</code>, <code>grid-column-end</code>. 
</p>

```css
/* default */
grid-area: auto; 
```

<p style="font-family: Roboto">
The grid item's column and row starts and ends are automatically set. 
</p>

```css
grid-area: main; 
```

<p style="font-family: Roboto">
You can use an area name. 
</p>


<h3 style="font-family: Roboto"><code>grid-auto-column</code></h3>

<p style="font-family: Roboto">
Defines the size of grid columns that were created implicitly: it means that <code>grid-auto-columns</code> targets the columns that were not defined with <code>grid-template-columns</code> or <code>grid-template-areas</code>. 
</p>

```css
/* default */
grid-auto-columns: auto; 
```

<p style="font-family: Roboto">
The implicity-created columns have an auto size. 
</p>

```css
grid-auto-columns: 100px; 
```

<p style="font-family: Roboto">
Here we combine grid-template-areas: "header header header" "sidebar main main" with grid-template-columns: 50px 200px.

In this situation, the grid-template-areas defines 3 columns, while the grid-template-columns only defines 2 column widths.

As a result, the third column width takes its value from the grid-auto-columns property: 100px. 
</p>

<h3 style="font-family: Roboto"><code>grid-auto-flow</code></h3>

<p style="font-family: Roboto">
Defines the position of auto-generated grid items. 
</p>

```css
/* default */
grid-auto-flow: row; 
```

<p style="font-family: Roboto">
In this two-columns setup, the second grid item is two-columns wide, the third item is four-rows tall.

The other grid items are placed on additional rows. 
</p>

```css
grid-auto-flow: column; 
```

<p style="font-family: Roboto">
The other grid items are placed on additional columns. 
</p> 

<h3 style="font-family: Roboto"><code>grid-auto-rows</code></h3>

<p style="font-family: Roboto">
Defines the size of grid rows that were created implicitly: it means that <code>grid-auto-rows</code> targets the rows that were not defined with <code>grid-template-rows</code> or <code>grid-template-areas</code>. 
</p>

```css
/* default */
grid-auto-rows: auto; 
```

<p style="font-family: Roboto">
The implicity-created rows have an auto size. 
</p>

```css
grid-auto-rows: 100px; 
```

<p style="font-family: Roboto">
Here we combine grid-template-areas: "header header header" "sidebar main main" "footer footer footer" with grid-template-rows: 50px 200px.

In this situation, the grid-template-areas defines 3 rows, while the grid-template-rows only defines 2 row heights.

As a result, the third row height (the footer) takes its value from the grid-auto-rows property: 100px. 
</p>

<h3 style="font-family: Roboto"><code>grid-column-end</code></h3>

<p style="font-family: Roboto">
Defines the column end position of a grid item. 
</p>

```css
/* default */
grid-column-end: auto; 
```

<p style="font-family: Roboto">
In this 3-column setup, the grid item is automatically placed. 
</p>

```css
grid-column-end: 2; 
``` 

<p style="font-family: Roboto">
The target grid item ends just before the second column. 
</p>

<h3 style="font-family: Roboto"><code>grid-column-gap</code></h3>

<p style="font-family: Roboto">
Defines the gutter between the columns of a grid container. 
</p>

```css
/* default */
grid-column-gap: 0; 
```

<p style="font-family: Roboto">
Removes the gap. 
</p>

```css
grid-column-gap: 10px; 
```

<p style="font-family: Roboto">
You can use pixel values. 
</p>

<h3 style="font-family: Roboto"><code>grid-column-start</code></h3>

<p style="font-family: Roboto">
Defines the column start position of a grid item. 
</p>

```css
/* default */
grid-column-start: auto; 
```

<p style="font-family: Roboto">
In this 3-column setup, the grid item is automatically placed. 
</p>

```css
grid-column-start: 2; 
```

<p style="font-family: Roboto">
The target grid item is placed on the second column. 
</p>

<h3 style="font-family: Roboto"><code>grid-column</code></h3>

<p style="font-family: Roboto">
Shorthand property for <code>grid-column-start</code> and <code>grid-column-end</code>. 
</p>

```css
grid-column: 1 / 3; 
```

<p style="font-family: Roboto">
The grid item starts before the first column and ends just before the third one. 
</p>

<h3 style="font-family: Roboto"><code>grid-row-end</code></h3>

<p style="font-family: Roboto">
Defines the row end position of a grid item. 
</p>

```css
/* default */
grid-row-end: auto; 
```

<p style="font-family: Roboto">
In this 3-column setup, the grid item is automatically placed. 
</p>

```css
grid-row-end: 3; 
```

<p style="font-family: Roboto">
The target grid item ends just before the third row. 
</p>

<h3 style="font-family: Roboto"><code>grid-row-gap</code></h3>

<p style="font-family: Roboto">
Defines the gutter between the rows of a grid container. 
</p>

```css
/* default */
grid-row-gap: 0; 
```

<p style="font-family: Roboto">
Removes the gap. 
</p>

```css
grid-row-gap: 10px; 
```

<p style="font-family: Roboto">
You can use pixel values. 
</p>

<h3 style="font-family: Roboto"><code>grid-row-start</code></h3>

<p style="font-family: Roboto">
Defines the row start position of a grid item. 
</p>

```css
/* default */
grid-row-start: auto; 
```

<p style="font-family: Roboto">
In this 3-column setup, the grid item is automatically placed on the first row. 
</p>

```css
grid-row-start: 2; 
```

<p style="font-family: Roboto">
The target grid item is placed on the second row. 
</p>

<h3 style="font-family: Roboto"><code>grid-row</code></h3>

<p style="font-family: Roboto">
Shorthand property for <code>grid-row-start</code> and <code>grid-row-end</code>. 
</p>

```css
grid-row: 1 / 3; 
```

<p style="font-family: Roboto">
The grid item starts before the first row and ends just before the third one. 
</p>

<h3 style="font-family: Roboto"><code>grid-template-areas</code></h3>

<p style="font-family: Roboto">
Defines areas within a grid container. These areas can then be referenced when placing a grid item. 
</p>

```css
/* default */
grid-template-areas: none; 
```

<p style="font-family: Roboto">
No area is defined. 
</p>

```css
grid-template-areas: "header header header" "sidebar main main"; 
```

<p style="font-family: Roboto">
You can use area names to specify which cells each grid item should occupy. 
</p>

<h3 style="font-family: Roboto"><code>grid-template-columns</code></h3> 

<p style="font-family: Roboto">
Defines the columns of a grid container. You can specify the width of a column by using a keyword (like auto) or a length (like 10px). The number of columns is determined by the number of values defined in the space-separated list. 
</p>

```css
/* default */
grid-template-columns: none; 
``` 

<p style="font-family: Roboto">
No columns are defined, so you only have one. 
</p>

```css
grid-template-columns: auto auto auto; 
```

<p style="font-family: Roboto">
You can use the keyword auto so that each column resizes itself automatically. 
</p>

```css
grid-template-columns: 40px 1fr 2fr; 
```

<p style="font-family: Roboto">
You can use the fr flex unit to distribute the remaining space across all flex columns. 
</p>

<h3 style="font-family: Roboto"><code>grid-template-rows</code></h3>

<p style="font-family: Roboto">
Defines the rows of a grid container. You can specify the width of a row by using a keyword (like auto) or a length (like 10px). The number of rows is determined by the number of values defined in the space-separated list. 
</p>

```css
/* default */
grid-template-rows: none; 
```

<p style="font-family: Roboto">
No rows are defined. 
</p>

```css
grid-template-rows: 120px auto 3rem; 
```

<p style="font-family: Roboto">
You can mix the units. 
</p>

```css
grid-template-rows: 20px 1fr 2fr; 
```

<p style="font-family: Roboto">
You can use the fr flex unit to distribute the remaining space across all flex rows. 
</p>

<h3 style="font-family: Roboto"><code>grid-template</code></h3>

<p style="font-family: Roboto">
Shorthand property for <code>grid-template-columns</code> and <code>grid-template-rows</code>. 
</p>

<h3 style="font-family: Roboto"><code>grid</code></h3>

<p style="font-family: Roboto">
Shorthand property for <code>grid-template-rows</code> <code>grid-template-columns</code> <code>grid-template-areas</code> <code>grid-auto-rows</code> <code>grid-auto-columns</code> and <code>grid-auto-flow</code>. 
</p>

<h3 style="font-family: Roboto"><code>height</code></h3>

<p style="font-family: Roboto">
Defines the height of the element. 
</p>

```css
/* default */
height: auto; 
```

<p style="font-family: Roboto">
The element will automatically adjust its height to allow its content to be displayed correctly. 
</p>

```css
height: 100px; 
```

<p style="font-family: Roboto">
You can use numeric values like pixels, (r)em, percentages...

If the content does not fit within the specified height, it will overflow. How the container will handle this overflowing content is defined by the overflow property. 
</p>

<h3 style="font-family: Roboto"><code>justify-content</code></h3>

<p style="font-family: Roboto">
Defines how flexbox/grid items are aligned according to the main axis, within a flexbox/grid container. 
</p>

```css
/* default */
justify-content: flex-start; 
```

<p style="font-family: Roboto">
The flexbox/grid items are pushed towards the start of the container's main axis. 
</p>

```css
justify-content: flex-end; 
```

<p style="font-family: Roboto">
The flexbox/grid items are pushed towards the end of the container's main axis. 
</p>

```css
justify-content: center; 
```

<p style="font-family: Roboto">
The flexbox/grid items are centered along the container's main axis.
</p>

```css
justify-content: space-between; 
```

<p style="font-family: Roboto">
The remaining space is distributed between the flexbox/grid items. 
</p>

```css
justify-content: space-around; 
```

<p style="font-family: Roboto">
The remaining space is distributed around the flexbox/grid items: this adds space before the first item and after the last one. 
</p>

<h3 style="font-family: Roboto"><code>left</code></h3>

<p style="font-family: Roboto">
Defines the position of the element according to its left edge. 
</p>

```css
/* default */
left: auto; 
```

<p style="font-family: Roboto">
The element will remain in its natural position. 
</p>

```css
left: 80px; 
```

<p style="font-family: Roboto">
If the element is in position relative, the element will move left by the amount defined by the left value. 
</p>

<h3 style="font-family: Roboto"><code>letter-spacing</code></h3>

<p style="font-family: Roboto">
Defines the spacing between the characters of a block of text. 
</p>

```css
/* default */
letter-spacing: normal; 
```

<p style="font-family: Roboto">
The spacing between the characters is normal. 
</p>

```css
letter-spacing: 2px; 
```

<p style="font-family: Roboto">
You can use pixel values. 
</p>

<h3 style="font-family: Roboto"><code>line-height</code></h3>

<p style="font-family: Roboto">
Defines the height of a single line of text. 
</p>

```css
/* default */
line-height: normal; 
```

<p style="font-family: Roboto">
Reverts to the default value of the browser. 
</p>

```css
/* recommended */
line-height: 1.6; 
```

<p style="font-family: Roboto">
You can use unitless values: the line height will be relative to the font size. 
</p>

<h3 style="font-family: Roboto"><code>list-style-type</code></h3>

<p style="font-family: Roboto">
Defines the type of a list item's bullet point. 
</p>

```css
/* default */
list-style-type: disc; 
```

<p style="font-family: Roboto">
The list items will use a disc as their bullet point. 
</p>

```css
list-style-type: circle;
list-style-type: square; 
list-style-type: decimal;
list-style-type: none; 
```

<p style="font-family: Roboto">
You can use the following values: <code>disc</code>, <code>circle</code>, <code>square</code>, <code>decimal</code> and <code>none</code>.
</p>

<h3 style="font-family: Roboto"><code>margin-bottom</code></h3>

<p style="font-family: Roboto">
Defines the space outside the element, on the bottom side. 
</p>

```css
/* default */
margin-bottom: 0; 
```

<p style="font-family: Roboto">
Removes any margin at the bottom. 
</p>

```css
margin-bottom: 30px; 
```

<p style="font-family: Roboto">
You can use pixel values. 
</p>

<h3 style="font-family: Roboto"><code>margin-left</code></h3>

<p style="font-family: Roboto">
Defines the space outside the element, on the left side. 
</p>

```css
/* default */
margin-left: 0; 
```

<p style="font-family: Roboto">
Removes any margin on the left. 
</p>

```css
margin-left: 30px; 
```

<p style="font-family: Roboto">
You can use pixel values. 
</p>

<h3 style="font-family: Roboto"><code>margin-right</code></h3>

<p style="font-family: Roboto">
Defines the space outside the element, on the right side. 
</p>

```css
/* default */
margin-right: 0; 
```

<p style="font-family: Roboto"> 
Removes any margin on the right. 
</p>

```css
margin-right: 30px; 
```

<p style="font-family: Roboto">
You can use pixel values. 
</p>

<h3 style="font-family: Roboto"><code>margin-top</code></h3>

<p style="font-family: Roboto">
Defines the space outside the element, on the top side. 
</p>

```css
/* default */
margin-top: 0; 
```

<p style="font-family: Roboto">
Removes any margin on the top. 
</p>

```css
margin-top: 30px; 
``` 

<p style="font-family: Roboto">
You can use pixel values. 
</p>

<h3 style="font-family: Roboto"><code>margin</code></h3>

<p style="font-family: Roboto">
Shorthand property for the <code>margin-top</code>, <code>margin-right</code>, <code>margin-bottom</code> and <code>margin-left</code> properties. 
</p>

<h3 style="font-family: Roboto"><code>max-height</code></h3>

<p style="font-family: Roboto">
Defines the maximum height the element can be. 
</p>

```css
/* default */
max-height: none; 
```

<p style="font-family: Roboto">
The element has no limit in terms of height. 
</p>

```css
max-height: 100px; 
```

<p style="font-family: Roboto">
You can use numeric values like pixels, (r)em, percentages...

If the maximum height is larger than the element's actual height, the max height has no effect. 
</p>

<h3 style="font-family: Roboto"><code>max-width</code></h3>

<p style="font-family: Roboto">
Defines the maximum width the element can be. 
</p>

```css
/* default */
max-width: none; 
```

<p style="font-family: Roboto">
The element has no limit in terms of width. 
</p>

```css
max-width: 100px; 
```

<p style="font-family: Roboto">
You can use numeric values like pixels, (r)em, percentages... 
</p> 

<h3 style="font-family: Roboto"><code>min-height</code></h3> 

<p style="font-family: Roboto">
Defines the minimum height of the element. 
</p>

```css
/* default */
min-height: 0; 
```

<p style="font-family: Roboto">
The element has no minimum height. 
</p>

```css
min-height: 100px; 
```

<p style="font-family: Roboto">
You can use numeric values like pixels, (r)em, percentages... 
</p>

<h3 style="font-family: Roboto"><code>min-width</code></h3> 

<p style="font-family: Roboto">
Defines the minimum width of the element. 
</p>

```css
/* default */
min-width: 0; 
```

<p style="font-family: Roboto">
The element has no minimum width. 
</p>

```css
min-width: 100px; 
``` 

<p style="font-family: Roboto">
You can use numeric values like pixels, (r)em, percentages... 
</p>

<h3 style="font-family: Roboto"><code>opacity</code></h3>

<p style="font-family: Roboto">
Defines how opaque the element is. 
</p>

```css
/* default */
opacity: 1; 
```

<p style="font-family: Roboto">
The element is fully opaque. 
</p>

```css
opacity: 0.5; 
```

<p style="font-family: Roboto">
Any value between 0 (zero) and 1 (one) will make the element semi transparent. 
</p>

<h3 style="font-family: Roboto"><code>outline-color</code></h3>

<p style="font-family: Roboto">
Defines the color of the element's outlines. 
</p>

```css
/* default */
outline-color: transparent; 
```

<p style="font-family: Roboto"> 
Applies a transparent color to the outlines. The outlines will still take up the space defined by the outline-width value. 
</p>

```css
outline-color: red; 
``` 

<p style="font-family: Roboto">
You can use one of the 140+ color names. 
</p>

<h3 style="font-family: Roboto"><code>outline-style</code></h3>

<p style="font-family: Roboto">
Defines the style of the element's outlines. 
</p>

```css
/* default */
outline-style: none; 
```

<p style="font-family: Roboto">
Removes the element's outlines. 
</p>

```css
outline-style: dotted; 
```

<p style="font-family: Roboto">
Turns the outline into a sequence of dots. 
</p>

```css
outline-style: solid; 
```

<p style="font-family: Roboto">
Turns the outline into a solid line. 
</p>

```css
outline-style: dashed; 
```

<p style="font-family: Roboto">
Turns the outline into a sequence of dashes. 
</p>

<h3 style="font-family: Roboto"><code>outline-width</code></h3>

<p style="font-family: Roboto">
Defines the width of the element's outlines. 
</p>

```css
/* default */
outline-width: medium; 
```

<p style="font-family: Roboto">
Defines the width of all outlines to medium. 
</p>

```css
outline-width: 1px; 
```

<p style="font-family: Roboto">
Defines the width of all outlines to 1px. 
</p>

<h3 style="font-family: Roboto"><code>outline</code></h3>

<p style="font-family: Roboto">
Shorthand property for the <code>outline-color</code>, <code>outline-style</code> and <code>outline-width</code> properties. 
</p>

<h3 style="font-family: Roboto"><code>overflow-wrap</code></h3>

<p style="font-family: Roboto">
Defines if words should break when reaching the end of a line. 
</p>

```css
/* default */
overflow-wrap: normal; 
``` 

<p style="font-family: Roboto">
Words with no space will not break. Sequences of uninterrupted characters will be displayed on a single line. 
</p>

```css
overflow-wrap: break-word; 
``` 

<p style="font-family: Roboto">
Words with no space will break as soon as they reach the end of a line. 
</p>

<h3 style="font-family: Roboto"><code>overflow-x</code></h3>

<p style="font-family: Roboto">
Defines how overflowing content on the horizontal axis is displayed. 
</p>

```css
/* default */
overflow-x: visible; 
```

<p style="font-family: Roboto">
The overflowing content is visible, while the element itself stays at the specified width. 
</p>

```css
overflow-x: hidden; 
```

<p style="font-family: Roboto">
The overflowing content is hidden and can not be accessed. 
</p>

```css
overflow-x: scroll; 
```

<p style="font-family: Roboto">
The overflowing content is accessible thanks to a horizontal scrollbar. 
</p>

```css
overflow-x: auto; 
```

<p style="font-family: Roboto">
The browser decides whether to display a horizontal scrollbar or not. 
</p>

<h3 style="font-family: Roboto"><code>overflow-y</code></h3>

<p style="font-family: Roboto">
Defines how overflowing content on the vertical axis is displayed. 
</p>

```css
/* default */
overflow-y: visible; 
```

<p style="font-family: Roboto">
The overflowing content is visible, while the element itself stays at the specified height. 
</p>

```css
overflow-y: hidden; 
```

<p style="font-family: Roboto">
The overflowing content is hidden and can not be accessed. 
</p>

```css
overflow-y: scroll; 
```

<p style="font-family: Roboto">
The overflowing content is accessible thanks to a vertical scrollbar. 
</p>

```css
overflow-y: auto; 
```

<p style="font-family: Roboto">
The browser decides whether to display a vertical scrollbar or not. 
</p>

<h3 style="font-family: Roboto"><code>overflow</code></h3>

<p style="font-family: Roboto">
Shorthand property for the <code>overflow-x</code> and <code>overflow-y</code> properties. 
</p> 

<h3 style="font-family: Roboto"><code>padding-bottom</code></h3>

<p style="font-family: Roboto">
Defines the space inside the element, on the bottom side. 
</p>

```css
/* default */
padding-bottom: 0; 
```

<p style="font-family: Roboto">
Removes any padding on the bottom. 
</p>

```css
padding-bottom: 50px; 
```

<p style="font-family: Roboto">
You can use pixels values. 
</p>

<h3 style="font-family: Roboto"><code>padding-left</code></h3>

<p style="font-family: Roboto">
Defines the space inside the element, on the left side. 
</p>

```css
/* default */
padding-left: 0; 
```

<p style="font-family: Roboto">
Removes any padding on the left. 
</p>

```css
padding-left: 50px; 
```

<p style="font-family: Roboto">
You can use pixels values. 
</p>

<h3 style="font-family: Roboto"><code>padding-right</code></h3>

<p style="font-family: Roboto">
Defines the space inside the element, on the right side. 
</p>

```css
/* default */
padding-right: 0; 
```

<p style="font-family: Roboto">
Removes any padding on the right. 
</p>

```css
padding-right: 50px; 
```

<p style="font-family: Roboto">
You can use pixels values. 
</p>

<h3 style="font-family: Roboto"><code>padding-top</code></h3>

<p style="font-family: Roboto"> 
Defines the space inside the element, on the top side. 
</p>

```css
/* default */ 
padding-top: 0; 
```

<p style="font-family: Roboto">
Removes any padding on the top. 
</p>

```css
padding-top: 50px; 
```

<p style="font-family: Roboto"> 
You can use pixels values. 
</p>

<h3 style="font-family: Roboto"><code>padding</code></h3>

<p style="font-family: Roboto">
Shortcut property for the <code>padding-top</code>, <code>padding-right</code>, <code>padding-bottom</code> and <code>padding-left</code> properties. 
</p>

<h3 style="font-family: Roboto"><code>right</code></h3>

<p style="font-family: Roboto">
Defines the position of the element according to its right edge. 
</p>

```css
/* default */
right: auto; 
```

<p style="font-family: Roboto">
The element will remain in its natural position. 
</p>

```css
right: 50px; 
```

<p style="font-family: Roboto">
If the element is in position relative, the element will move right by the amount defined by the right value. 
</p>

<h3 style="font-family: Roboto"><code>text-align</code></h3>

<p style="font-family: Roboto">
Defines how the text content of the element is horizontally aligned. 
</p>

```css
text-align: left; 
```

<p style="font-family: Roboto">
The text content is aligned to the left. 
</p>

```css
text-align: right; 
``` 

<p style="font-family: Roboto">
The text content is aligned to the right. 
</p>

```css
text-align: center; 
```

<p style="font-family: Roboto">
The text content is centered. 
</p>

```css
text-align: justify; 
```

<p style="font-family: Roboto">
The text content is justified. 
</p>

<h3 style="font-family: Roboto"><code>text-decoration</code></h3>

<p style="font-family: Roboto">
Defines how the text content of the element is decorated. 
</p>

```css
/* default */
text-decoration: none; 
```

<p style="font-family: Roboto">
Removes any text decoration. 
</p>

```css
text-decoration: underline; 
```

<p style="font-family: Roboto">
Underlines the text content. 
</p>


<h3 style="font-family: Roboto"><code>text-indent</code></h3>

<p style="font-family: Roboto">
Defines the indentation of the element's first line of text. 
</p>

```css
/* default */
text-indent: 0; 
```

<p style="font-family: Roboto">
The text is not indented. 
</p>

```css
text-indent: 50px; 
```

<p style="font-family: Roboto">
You can use numeric values like pixels, (r)em, percentages... 
</p>

<h3 style="font-family: Roboto"><code>text-transform</code></h3>

<p style="font-family: Roboto">
Defines how the text content should be transformed. 
</p>

```css
/* default */
text-transform: none; 
```

<p style="font-family: Roboto">
Removes any text transformation: the text will appear the same as in the HTML code. 
</p>

```css
text-transform: capitalize;
text-transform: uppercase;
text-transform: lowercase;
```

<p style="font-family: Roboto">
<code>capitalize</code>, <code>uppercase</code> and <code>lowercase</code> transform the text content to the specified case. 
</p>

<h3 style="font-family: Roboto"><code>top</code></h3>

<p style="font-family: Roboto">
Defines the position of the element according to its top edge. 
</p>

```css
/* default */
top: auto; 
```

<p style="font-family: Roboto">
The element will remain in its natural position. 
</p>

```css
top: 50px; 
```

<p style="font-family: Roboto">
If the element is in position relative, the element will move downwards by the amount defined by the top value. 
</p>

<h3 style="font-family: Roboto"><code>vertical-align</code></h3>

<p style="font-family: Roboto">
Defines how an inline or table-cell element aligns vertically. 
</p>

```css
vertical-align: baseline; 
```

<p style="font-family: Roboto">
The element is aligned with the baseline of the parent. 
</p>

```css
vertical-align: sub; 
```

<p style="font-family: Roboto">
The element is aligned with the subscript baseline of the parent. 
</p>

<h3 style="font-family: Roboto"><code>width</code></h3>

<p style="font-family: Roboto">
Defines the width of the element. 
</p>

```css
/* default */
width: auto; 
```

<p style="font-family: Roboto">
The element will automatically adjust its width to allow its content to be displayed correctly. 
</p>

```css
width: 50px; 
```

<p style="font-family: Roboto">
You can use numeric values like pixels, (r)em, percentages... 
</p>

<h3 style="font-family: Roboto"><code>z-index</code></h3>

<p style="font-family: Roboto">
Defines the order of the elements on the z-axis. It only works on positioned elements (anything apart from static). 
</p>

```css
/* default */
z-index: auto; 
```

<p style="font-family: Roboto">
The order is defined by the order in the HTML code:
</p>
<li>first in the code = behind</li>
<li>last in the code = in front</li>

```css
z-index: 1; 
```

<p style="font-family: Roboto">
The z-index value is relative to the other ones. The target element is move in front of its siblings. 
</p>