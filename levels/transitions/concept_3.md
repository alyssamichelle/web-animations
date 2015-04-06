# Concept 3
### Properties that can be transitioned
We just looked at three things that can be trans. What all properties can be transitioned, though?
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
