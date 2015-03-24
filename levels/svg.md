# SVG
This level will answer these questions: What are SVGs; How to get SVGs; When to Use SVGs over raster images; How to animate SVGs with CSS.

## What is SVG?
Just another file type `<img src='horse.svg' alt='horse'>`

- Both HTML & SVG originate from XML
- SMIL
  - An animating syntax built right into SVG
  ```SVG
  <svg viewBox="0 0 127.9 178.4">
    <path d="M37.6,138.8c0 ... ">
      <animate attributeName="fill" dur="5000ms" to="#f06d06" fill="freeze" />  
    </path>
  </svg>
  ```

## Why SVG
[SVG for everybody by Coyier](https://css-tricks.com/video-screencasts/137-svg-is-for-everybody/)

- Scaleable Vector Graphics
- SVG is sharp at any size and small in file size
- SVG and HTML are both XML, a data format

## Getting SVG images to use?

1. Write your own
  - eww, who does that?
2. Save As SVG in an editing program
  - SVG can be made from anything "vector" .eps .pdf .ai
  - Open in [Illustrator](http://www.adobe.com/products/illustrator.html) and save as .svg
  - Or try out a free editing program like Inkscape
3. Find it on the Interwebs (shutterstock yo')

## Animating SVGs
[Three ways to animate SVG by Coyier](https://css-tricks.com/video-screencasts/135-three-ways-animate-svg/)

1. SVG Syntax  (SMIL)
  <image src='https://s3.amazonaws.com/f.cl.ly/items/2O2v2H1H0Z3i2C1x1d3U/Image%202015-03-18%20at%202.23.48%20PM.png'>
2. CSS @keyframes/transitions
3. With Javascript
<p data-height="268" data-theme-id="5377" data-slug-hash="OPaoaO" data-default-tab="result" data-user="alyssamichelle" class='codepen'>See the Pen <a href='http://codepen.io/alyssamichelle/pen/OPaoaO/'>Three Ways to Animate SVG</a> by Alyssa Nicoll (<a href='http://codepen.io/alyssamichelle'>@alyssamichelle</a>) on <a href='http://codepen.io'>CodePen</a>.</p>
<script async src="//assets.codepen.io/assets/embed/ei.js"></script>

### Animating SVGs with CSS
<p data-height="268" data-theme-id="5377" data-slug-hash="dvjhn" data-default-tab="result" data-user="chriscoyier" class='codepen'>See the Pen <a href='http://codepen.io/chriscoyier/pen/dvjhn/'>Wufoo SVG Ad</a> by Chris Coyier (<a href='http://codepen.io/chriscoyier'>@chriscoyier</a>) on <a href='http://codepen.io'>CodePen</a>.</p>
<script async src="//assets.codepen.io/assets/embed/ei.js"></script>
