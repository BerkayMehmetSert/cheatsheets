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