# SVG
This level will answer these questions: What are SVGs; How to get SVGs; When to Use SVGs over raster images; How to animate SVGs with CSS.
- What is SVG?
- Build Tools to create/export as SVG
- Resources to get pre-made SVGs
- Inline SVG <img src='horse.svg' alt='horse'>
- BG image with CSS SVG .horse { background: url(horse.svg);}
- Responsive Icons to achieve Progressive De-hancement
  - CodePen Example by Coyier: http://codepen.io/alyssamichelle/pen/RNqXQG
  - Responsive Icons Site: http://responsiveicons.co.uk/
- Animating SVGs with CSS
  - CodePen Example by Coyier: http://codepen.io/chriscoyier/pen/dvjhn

## Why SVG
https://css-tricks.com/video-screencasts/137-svg-is-for-everybody/

- Scaleable Vector Graphics
- SVG is sharp at any size and small in file size

- SVG and HTML are both XML, a data format

## Getting SVG images to use?

1. Write your own
  - eww, who does that?
2. Save As SVG in an editting program (try inkscape for free)
  - SVG can be made from anything "vector" .eps .pdf .ai .whatever open in illustrator and save as .svg
  - Illustrator 19.99/mo http://www.adobe.com/products/illustrator.html?sdid=KKQMI&kw=semgeneric&skwcid=AL
3. Find it on the Interwebs (shutterstock yo')

## Animating SVGs
Three ways to animate SVG
https://css-tricks.com/video-screencasts/135-three-ways-animate-svg/

1. SVG Syntax <animate> (SMIL)
  - http://cl.nicoll.co/aGIq
2. CSS @keyframes/transitions
  - http://codepen.io/chriscoyier/pen/dvjhn
3. With Javascript


### Addtl Topics

#### Using SVG Images
1. HTML as SVG `<img src='horse.svg' alt='horse'>`
  - Three advantages for using inline svg: http://cl.nicoll.co/aGBI
2. CSS as background-image
```css
.horse {
  background: url(horse.svg);
}
```

- SVG Shape Morphing
  - https://css-tricks.com/svg-shape-morphing-works/
- SVG Viewbox
- SVG Viewport
