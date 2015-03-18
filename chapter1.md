# CSS3 Animations
- spinning gear icon

- checkboxes use label bc they mark check or uncheck, still have check box but they hide it, style the label like that...

- http://useyourinterface.com/

- https://www.firebase.com/docs/hosting/guide/deploying.html scroll to the bottom of the site, notice how the next section is displayed

- Lends a hand to user interaction, not take away

## Inspiration & Resources
Inspiration: http://tympanus.net/codrops/category/playground/
animate.css: http://daneden.github.io/animate.css/
Val Head Book: https://www.dropbox.com/sh/yf8o1xc5vnduqyk/AADxPo28J7iHeQo-ZyU0dunwa?dl=0
Val Head Video: https://vimeo.com/61477511
Animations MDN: https://developer.mozilla.org/en-US/docs/Web/CSS/animation
Transitions MDN: https://developer.mozilla.org/en-US/docs/Web/Guide/CSS/Using_CSS_transitions
Pluralsight CSS3 in Depth: http://www.pluralsight.com/courses/css3-in-depth
PS CSS3 Michael: http://www.pluralsight.com/courses/css3

## App Ideas
App: http://www.raawmacaw.com/customized-energy-bars
Preview: http://screencast.com/t/0Y6H2QFa

## Code Pen
Animating Dropdown: http://codepen.io/alyssamichelle/pen/JoeeyZ

## Animations

- animation-name: none
- animation-duration: 0s
- animation-timing-function: ease
- animation-delay: 0s
- animation-iteration-count: 1
- animation-direction: normal
- animation-fill-mode: none
- animation-play-state: running

Formal syntax: `<single-animation-name> || <time> || <timing-function> || <time> || <single-animation-iteration-count> || <single-animation-direction> || <single-animation-fill-mode> || <single-animation-play-state>`

There are two parts to keyframe animations:
- creating the animation
- assigning the animation

- **Vendor Prefixes**

### Basic Ingredients to all CSS Animations
 - a name
 - keyframes
 - something to take direction (element)

### 2 Main parts of any CSS animation

1. Defining the animation
2. Assigning it to a specific HTML element


### @keyframes Rule
Used to declare the keyframes:

  ```css
  @keyframes nameOfAnimation {

  }
  ```

### @keyframes Name
Used to refer to the animation later: `nameOfAnimation`


### What is a Keyframe
**Keyframe: A list of what should happen over the course of the animation; which properties should change, how and when.**

### Defining a Keyframe
- @keyframe declarations
  - `from` and `to` keywords
- percentages

### Keyframe declarations
```css
@keyframes nameOfAnimation {
  from {transform: translateX(0);}
  to {transform: translateX(400px);}
}
```

#### -same as-

### Percentages
```css
@keyframes nameOfAnimation {
  0% {transform: translateX(0);}
  100% {transform: translateX(400px);}
}
```

As you can see, `from` is equivalent to `0%` and `to` is equivalent to `100%`.


# Section 2 More Control

```css
 animation-delay: 2s;
 animation-fill-mode: forwards;
```

http://codepen.io/anon/pen/XJxQjQ

### Practical CS Example
A model notification that pops in at the bottom of the page, read more docs?, that is dismissable.

## Animation-fill-mode
The animation-fill-mode CSS property specifies how a CSS animation should apply styles to its target before and after it is executing.

### Animation-fill-mode properties

- none: default
- forwards: The element will stay set by the last keyframe encountered. **Important note: last key frame to execute, not defined.**

- backwards: Causes the first keyframe of an animation to persist before the animation starts. `animation-delay` period

Jameson: can be good for chaining, check out https://vimeo.com/89021288

- both: The animation will follow the rules for both forwards and backwards, thus extending the animation properties in both directions. **I think this means: The element will stay set by the first keyframe encountered during the `animation-delay` period and after animating will be stay set by the last keyframe values.**

    “ The target of your animation will take on the styles of your first keyframe before the animation starts. Then, when the animation completes, it will maintain the styling from the last keyframe to be executed.”

Excerpt From: Val Head. “A Pocket Guide to CSS animations.” iBooks.

---

## A Shorthand

`animation: myAnimation 1s ease-in-out 2s 4;`

animation: `<animation-name> <animation-duration> <animation-timing-function> <animation-delay> <animation-iteration-count>`


### Defining Multiple Animations in one Shorthand
To define multiple animations on one element using the shorthand, you need to separate the values for each animation with a comma. So an element with two animations applied to it would look something like this:

`animation: myAnimation 1s ease-in-out 2s 4, myOtherAnimation 4s ease-out 2s;`


## Transitions
CSS transitions provide a way to control animation speed when changing CSS properties. Instead of having property changes take effect immediately, you can cause the changes in a property to take place over a period of time.

    transition-delay: 0s
    transition-duration: 0s
    transition-property: all
    transition-timing-function: ease

#### Recipe

Formal syntax: `[ none | <single-transition-property> ] || <time> || <timing-function> || <time>`

Shorthand syntax:

`animation: <animation-name> <animation-duration> <animation-timing-function> <animation-delay> <animation-iteration-count>`

Real Example:
`animation: myAnimation 1s ease-in-out 2s 4;`

How to read formal syntax from MDN: https://developer.mozilla.org/en-US/docs/Web/CSS/Value_definition_syntax


The shorthand CSS syntax is written as follows:

```css
div {
    transition: <property> <duration> <timing-function> <delay>;
}
```

#### Simplest Transition over 0 seconds:

```css
a {
  color: red;
}

a:hover {
  color: yellow;
}
```

#### Simplest Transition over 1 second:

```css
a {
  color: red;
  transition: 1s;
}

a:hover {
  color: yellow;
}
```

#### What can be transitioned?
They are working towards all properties being able to transition. For now, if a property can have a middle state, then it can be transitioned. For instance, opacity.
http://www.pluralsight.com/training/player?author=estelle-weyl&name=css3-in-depth-m11&mode=live&clip=0&course=css3-in-depth

```css
code {
  opacity: 1;
}
code:halfway {
  opacity: 0.5;
}
code:hover {
  opacity: 0;
}
```

```css
code {
  display: block;
}
code:halfway {
  display: ???;
}
code:hover {
  display: none;
}
```

### List of transitional properties
https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_animated_properties

---

## Level 3, Section 1: SVG Animations
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
