# Problem 2
### Assigning Multiple Transitions
We want to transition multiple properties on this button, to provide prominence and feedback to the user. Let us both lighten the bg color on hover and the color of the text.

# Solution
### Transitioning Multiple Properties
```css
.button {
  /* Button Color Transition */
  transition: background-color 0.4s ease, color 0.4s ease;
  color: #92539E;
}

.button:hover {
  background-color: hsl(0, 0%, 85%);
  color: #AD7EB6;
}
```

<p data-height="268" data-theme-id="5377" data-slug-hash="QwPZjp" data-default-tab="result" data-user="alyssamichelle" class='codepen'>See the Pen <a href='http://codepen.io/alyssamichelle/pen/QwPZjp/'>QwPZjp</a> by Alyssa Nicoll (<a href='http://codepen.io/alyssamichelle'>@alyssamichelle</a>) on <a href='http://codepen.io'>CodePen</a>.</p>
<script async src="//assets.codepen.io/assets/embed/ei.js"></script>
