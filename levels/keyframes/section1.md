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

# Form Inputs (more steps)
## Kuro
```css
.input__field:focus,
.input--filled .input__field {
	opacity: 1;
	transition-delay: 0.3s;
}

.input__field:focus + .input__label::before,
.input--filled .input__label::before {
	transform: translate3d(-10%, 0, 0);
}

.input__field:focus + .input__label::after,
.input--filled .input__label::after {
	transform: translate3d(10%, 0, 0);
}

.input__field:focus + .input__label .input__label-content,
.input--filled .input__label-content {
	animation: anim-2 0.3s forwards;
}

@-webkit-keyframes anim-2 {
	50% {
		opacity: 0;
		transform: scale3d(0.3, 0.3, 1);
	}
	51% {
		opacity: 0;
		transform: translate3d(0, 3.7em, 0) scale3d(0.3, 0.3, 1);
	}
	100% {
		opacity: 1;
		transform: translate3d(0, 3.7em, 0);
	}
}
```

## Madoka

```css
.input__label-content {
	transform-origin: 0% 50%;
	transition: transform 0.3s;
}

.graphic {
	transform: scale3d(1, -1, 1);
	transition: stroke-dashoffset 0.3s;
	pointer-events: none;

	stroke: #7A7593;
	stroke-width: 4px;
	stroke-dasharray: 962;
	stroke-dashoffset: 558;
}

.input__field:focus + .input__label,
.input--filled .input__label {
	cursor: default;
	pointer-events: none;
}

.input__field:focus + .input__label .graphic,
.input--filled .graphic {
	stroke-dashoffset: 0;
}

.input__field:focus + .input__label .input__label-content,
.input--filled .input__label-content {
	transform: scale3d(0.81, 0.81, 1) translate3d(0, 4em, 0);
}
```
