# Problem 1
### Need a prominent call to action on the product page

Users, like players on game board, must be guided.

We guide Users through, what could be treacherous User Experience waters, to what hopefully is, a beautiful, calming and successful experience.

On the Interwebs, we have things like CSS Animations to help aide us in guiding Users.

For example, on our WYSIT game site, our Users will have multiple goals set out before them — Understanding the game, Purchasing the game, and communicating with other game players.

It is our job as the web designer to distinguish *which* of these goals are most important to our User and create a UI that will guide them to that goal.

Purchasing the Game is top priority. IF the User does not own the game, how can they play it or commune with other players?

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
