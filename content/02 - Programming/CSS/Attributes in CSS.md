# What are CSS attributes
- The actual styles we want to apply
- Specificity
	- [[ID]] > [[Class]] > [[Elements]]
## Colour
- The most basic we apply are
	- Colour
		- Will get applied to text
	- Background colour
		- Will get applied to Content and Padding of [[Layout]] selectors
```css
.hero {
	color: white;
	background-color: skyblue;
}
```
## [[Layout]]
## Font
- Managed by **font-family** and **font-size**
	- Always select multiple in case some don't work
```css
html {
	font-family: 'Segoe UI', 'Rubik', 'Calibri';
	font-size: 4rem;
}
```
## More background properties
- Used to add a little more style to the background
- This includes
	- background-image
	- background-repeat
	- background-size
	- background-position
	- box-shadow
```css
div {
	background-image: ('yoyo.png');
	background-repeat: no-repeat;
	background-size: fixed;
	background-position: center;
	box-shadow: 10px 10px 5px 0px black;
}
```
## Animations
- Quite complex, it is much easier to search for animations and copying them from [codepen](https://codepen.io)