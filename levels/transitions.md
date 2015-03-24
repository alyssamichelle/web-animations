# Transitions
CSS transitions provide a way to control animation speed when changing CSS properties. Instead of having property changes take effect immediately, you can cause the changes in a property to take place over a period of time.

    transition-delay: 0s
    transition-duration: 0s
    transition-property: all
    transition-timing-function: ease

## Recipe

Formal syntax: `[ none | <single-transition-property> ] || <time> || <timing-function> || <time>`

Shorthand Syntax:

```css
div {
    transition: <property> <duration> <timing-function> <delay>;
}
```

Note: Order is irrelevant, as long as you have your duration number specified before you delay.

Real Example:
`transition: all 2s ease-in-out 1s;`

Note: technically all that *needs* to be specified is the duration. The rest will have defaults, like all, ease, and 0.

Real Example:
`transition: 2s`

How to read formal syntax from MDN: https://developer.mozilla.org/en-US/docs/Web/CSS/Value_definition_syntax

## Simplest Transition over 0 seconds:

```css
a {
  color: red;
}

a:hover {
  color: yellow;
}
```

## Simplest Transition over 1 second:

```css
a {
  color: red;
  transition: 1s;
}

a:hover {
  color: yellow;
}
```

## What can be transitioned?
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


### Example: transitioning the color state of a button when it is hovered over.
Why: Graceful user feedback

<p data-height="268" data-theme-id="5377" data-slug-hash="zxexVX" data-default-tab="result" data-user="alyssamichelle" class='codepen'>See the Pen <a href='http://codepen.io/alyssamichelle/pen/zxexVX/'>Pure CSS animated menu icon</a> by Alyssa Nicoll (<a href='http://codepen.io/alyssamichelle'>@alyssamichelle</a>) on <a href='http://codepen.io'>CodePen</a>.</p>
<script async src="//assets.codepen.io/assets/embed/ei.js"></script>
