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
