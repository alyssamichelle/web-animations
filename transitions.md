# Transitions
CSS transitions provide a way to control animation speed when changing CSS properties. Instead of having property changes take effect immediately, you can cause the changes in a property to take place over a period of time.

    transition-delay: 0s
    transition-duration: 0s
    transition-property: all
    transition-timing-function: ease

## Recipe

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
