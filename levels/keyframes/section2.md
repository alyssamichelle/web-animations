
## Section 2 More Control

### Practical CS Example
A model notification that pops in at the bottom of the page, read more docs?, that is dismissable.

## Animation-fill-mode
The animation-fill-mode CSS property specifies how a CSS animation should apply styles to its target before and after it is executing.

### Animation-fill-mode properties

- none: default
- forwards: The element will stay set by the last keyframe encountered. **Important note: last key frame to execute, not defined.**

- backwards: Causes the first keyframe of an animation to persist before the animation starts. `animation-delay` period

**Fill-mode: backwards; example**
```css
 animation-delay: 2s;
 animation-fill-mode: backwards;
```

<p data-height="268" data-theme-id="5377" data-slug-hash="ByMRgq" data-default-tab="result" data-user="alyssamichelle" class='codepen'>See the Pen <a href='http://codepen.io/alyssamichelle/pen/ByMRgq/'>CSSA: Starting ball animation</a> by Alyssa Nicoll (<a href='http://codepen.io/alyssamichelle'>@alyssamichelle</a>) on <a href='http://codepen.io'>CodePen</a>.</p>
<script async src="//assets.codepen.io/assets/embed/ei.js"></script>

- both: The animation will follow the rules for both forwards and backwards, thus extending the animation properties in both directions. **I think this means: The element will stay set by the first keyframe encountered during the `animation-delay` period and after animating will be stay set by the last keyframe values.**

    “ The target of your animation will take on the styles of your first keyframe before the animation starts. Then, when the animation completes, it will maintain the styling from the last keyframe to be executed.”

Excerpt From: Val Head. “A Pocket Guide to CSS animations.” iBooks.

---

### Defining Multiple Animations in one Shorthand
To define multiple animations on one element using the shorthand, you need to separate the values for each animation with a comma. So an element with two animations applied to it would look something like this:

`animation: myAnimation 1s ease-in-out 2s 4, myOtherAnimation 4s ease-out 2s;`

## Progressive Enhancement
In our case this means designing our sight with people with lesser browser capabilities in mind. We want to build out content so that it will always be accessible (with or without css) but then layer in CSS nice-ities on top. For example, having an animation that is hidden by default (by being off screen) could be bad if our user does not have CSS capabilities and therefore just do not have access to that content at all. For more watch [Val Head’s 6 min video](https://vimeo.com/92054024).
