# Concept 1
### Transition Recipe
From here on transitions will follow this pattern, there is also an optional delay property (not often used).

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

Note: Order is irrelevant, as long as you have your duration number specified before the delay.

# Recipe Concept
### Technically all that *needs* to be specified is the duration. The rest will have defaults, like all, ease, and 0.

Long Example:
`transition: all 2s ease-in-out 1s;`

Short Example:
`transition: 2s`
