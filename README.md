# Pure-CSS-Music-Visualizer
Experience music like never before with this audio-reactive visualizer built entirely with CSS variables and animations. No JS required!
This project uses a fascinating architecture called the CSS Variable Bridge.

Instead of using JavaScript and the <canvas> tag to draw graphics (which is how 99% of visualizers work), JavaScript is only used as a hidden "sensor". It reads the audio frequencies and passes them to HTML as CSS Custom Properties (--vol). 100% of the visuals, scaling, glowing, colors, and reflections are handled purely by CSS.
How to use it:
Open it in your web browser.
Select an MP3 file from your computer (it runs entirely offline, so your files are safe and there are no loading times) and watch the magic!

What makes this code awesome:
The "Wet Floor" Reflection: Notice the -webkit-box-reflect property in the .visualizer-container CSS? It takes a single line of CSS to create a beautiful, dynamic, fading reflection of all the moving bars without duplicating any HTML.
Idle State Animation: Before you put a song on, the visualizer still looks alive. It uses a CSS @keyframes animation combined with calc(var(--i) * -0.1s) to stagger the animation delay automatically, creating a mesmerizing sine wave effect.
No CORS Issues: By allowing the user to select a local file (<input type="file">), this bypasses the strict Cross-Origin Resource Sharing (CORS) security policies browsers enforce on audio, meaning it will run flawlessly on any computer right out of the box!
