# Problem 2
### Input Label morph

```css
.input__label-content{
	transition: transform 0.3s;
}

.input__label::before,
.input__label::after {
	content: '';
	position: absolute;
	left: 0;
	z-index: -1;
	width: 100%;
	height: 4px;
	background: #6a7989;
	transition: transform 0.3s;
}

.input__field:focus + .input__label::before,
.input--filled .input__label::before {
	transform: translate3d(0, -0.5em, 0);
}

```
