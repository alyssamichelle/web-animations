
# Title
### Transitions
CSS transitions provide a way to control animation speed when changing CSS properties. Instead of having property changes take effect immediately, you can cause the changes in a property to take place over a period of time.


# Problem
### Need a prominent call to action on the product page

Users, like players on game board, must be guided.

We guide Users through, what could be treacherous User Experience waters, to what hopefully is, a beautiful, calming and successful experience.

On the Interwebs, we have things like CSS Animations to help aide us in guiding Users.

For example, on our WYSIT game site, our Users will have multiple goals set out before them — Understanding the game, Purchasing the game, and communicating with other game players.

It is our job as the web designer to distinguish *which* of these goals are most important to our User and create a UI that will guide them to that goal.

Purchasing the Game is top priority. IF the User does not own the game, how can they play it or commun with other players?

We can Use CSS Transitions to make buying the game a prominent call to action on our page

# Solution
### Using Transitions to make the BUY button more prominent

#### Bg-color Transition Lighter over .1 second:

```css
.button {
  background-color: hsl(0, 0%, 75%);
  transition: background-color .1s;
}

.button:hover {
  background-color: hsl(0, 0%, 85%);
}
```
<p data-height="268" data-theme-id="5377" data-slug-hash="WbWaGj" data-default-tab="result" data-user="alyssamichelle" class='codepen'>See the Pen <a href='http://codepen.io/alyssamichelle/pen/WbWaGj/'>WbWaGj</a> by Alyssa Nicoll (<a href='http://codepen.io/alyssamichelle'>@alyssamichelle</a>) on <a href='http://codepen.io'>CodePen</a>.</p>
<script async src="//assets.codepen.io/assets/embed/ei.js"></script>

# Mini Problem
### We want to transition multiple properties on this button, to provide prominence and feedback to the user. Let us both lighten the bg color on hover and the color of the text.

# Mini Solution
### Transitioning Multiple Properties
```css
.button {
  /* Button Color Transition */
  transition: background-color 0.1s ease, color 0.1s ease;
}

.button:hover {
  background-color: hsl(0, 0%, 85%);
  color: hsla(0, 0%, 5%, 0.7);
}
```

<p data-height="268" data-theme-id="5377" data-slug-hash="QwPZjp" data-default-tab="result" data-user="alyssamichelle" class='codepen'>See the Pen <a href='http://codepen.io/alyssamichelle/pen/QwPZjp/'>QwPZjp</a> by Alyssa Nicoll (<a href='http://codepen.io/alyssamichelle'>@alyssamichelle</a>) on <a href='http://codepen.io'>CodePen</a>.</p>
<script async src="//assets.codepen.io/assets/embed/ei.js"></script>

# Problem
### Our button is nice, it gives the User feedback with the current transitions on hover and it also provides Instant Gratification. (The point of the button, and in fact the entire page is short and to the point "BUY GAME") However, it would be nice at this point to also provide more information about the game, like how much it costs.

# Solution
### We can use transitions to animate in the cost on hover!

<p data-height="268" data-theme-id="5377" data-slug-hash="zxXmGa" data-default-tab="result" data-user="alyssamichelle" class='codepen'>See the Pen <a href='http://codepen.io/alyssamichelle/pen/zxXmGa/'>zxXmGa</a> by Alyssa Nicoll (<a href='http://codepen.io/alyssamichelle'>@alyssamichelle</a>) on <a href='http://codepen.io'>CodePen</a>.</p>
<script async src="//assets.codepen.io/assets/embed/ei.js"></script>


# Problem
### The button needs to do *something*... bring out the form!

# Solution
### Use CSS Transitions to bring the purchase form on screen smoothly and with a subtle flair.
<p data-height="268" data-theme-id="5377" data-slug-hash="azxdeR" data-default-tab="result" data-user="alyssamichelle" class='codepen'>See the Pen <a href='http://codepen.io/alyssamichelle/pen/azxdeR/'>azxdeR</a> by Alyssa Nicoll (<a href='http://codepen.io/alyssamichelle'>@alyssamichelle</a>) on <a href='http://codepen.io'>CodePen</a>.</p>
<script async src="//assets.codepen.io/assets/embed/ei.js"></script>

# Recipe Concept
### From here on transitions will follow this pattern, there is also an optional delay property (not often used).

Each property can be specified individually.

Long Syntax:

```css
div {
  transition-delay: 0s
  transition-duration: 0s
  transition-property: all
  transition-timing-function: ease
}
```

Shorthand Syntax:

```css
div {
  transition: <property> <duration> <timing-function> <delay>;
}
```

Formal syntax: `[ none | <single-transition-property> ] || <time> || <timing-function> || <time>`

Note: Order is irrelevant, as long as you have your duration number specified before you delay.

# Recipe Concept
### Technically all that *needs* to be specified is the duration. The rest will have defaults, like all, ease, and 0.

Long Example:
`transition: all 2s ease-in-out 1s;`

Short Example:
`transition: 2s`

# Concept
### **Vendor Prefixes**
Briefly mention Vendor Prefixes and how you might be able to use autoprefixer or a build tool like grunt when coding it up on your own at home.

- Ref the docs and canIUse.com
- Code Pen (uses [autoprefixer](https://github.com/postcss/autoprefixer))


# Concept
### We just looked at three things that can be trans. What all properties can be transitioned, though?
They are working towards all properties being able to transition. For now, if a property can have a middle state, then it can be transitioned. For instance, opacity.

# Concept
### Properties with a middle state

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

Otherwise you can just check out the full list:

#### List of transitional properties
https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_animated_properties
