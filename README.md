# JS - Rainbow_Rectangles

<p>Concentric rectangles following a specific color specter.</p>
<p>You can see the live preview on: <a href="https://negrut112.github.io/JS-rainbow-squares/">https://negrut112.github.io/JS-rainbow-squares/</a></p>

<img src="https://i.imgur.com/o6T9GMo.jpg">

## HTML
<p>I have used the HTML to define the area where I’m working defining the height, width and the border style:</p>
<p>&lt;canvas id=“myCanvas” height=“310” width=“500” style=“border: 1px solid black”&gt;&lt;/canvas&gt;</p>

## JavaScript
<p>To generate the rectangles I used a for loop where x manipulate the size of the rectangles and their position as well. starting from a width of 450 and 300 heigth the rectangles decrement their size by 20 on x-axis and 17 on y-axis.</p>
<p>For colors I used the same loop decrementing hue parameter by 17 for each rectangle.</p>
<pre><code>for(var x = 0;x&lt;17;x++){<br>
context.fillStyle=‘hsl(’ +(360-(360/17))<em>x+ ‘, 50%, 45%,1)’;<br>
context.fillRect(x</em>10,x<em>9, 450-20</em>x, 300-17*x);<br>
}</pre></code>
