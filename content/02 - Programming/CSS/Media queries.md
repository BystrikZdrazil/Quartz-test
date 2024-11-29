# What are media queries used for
- Used for styling for mobile and different screen sizes
- Triggered by **breakpoints**
	- Similar to **if statements**
```css
body {
	background-color: tan;
}

/*if window less than 992 pixels*/
@media screen and (max-width: 992px) {
	body {
		background-color: blue;
	}
}

/*if window less than 600 pixels*/
@media screen and (max-width: 600px) {
	body {
		background-color: azure;
	}
}
```