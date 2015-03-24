## Section 1 Keyframe Animations
- animation-name: none
- animation-duration: 0s
- animation-timing-function: ease
- animation-delay: 0s
- animation-iteration-count: 1
- animation-direction: normal
- animation-fill-mode: none
- animation-play-state: running

## Recipe
Formal syntax: `<single-animation-name> || <time> || <timing-function> || <time> || <single-animation-iteration-count> || <single-animation-direction> || <single-animation-fill-mode> || <single-animation-play-state>`

Shorthand Syntax:
`animation: myAnimation 1s ease-in-out 2s 4;`

animation: `<animation-name> <animation-duration> <animation-timing-function> <animation-delay> <animation-iteration-count>`

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

### **Vendor Prefixes**
Briefly mention Vendor Prefixes and how you might be able to use autoprefixer or a build tool like grunt when coding it up on your own at home.

- Ref the docs and canIUse.com
- Code Pen (uses autoprefixer)
