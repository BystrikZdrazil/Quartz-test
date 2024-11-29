# What layout options are in CSS
## The box model
- Each layout consists of
	- [[#Content]]
	- [[#Padding]]
	- [[#Border]]
	- [[#Margin]]
![[Box model graph.png]]

```css
.hero {
	width: 100px;
	height: 20px;
	padding: 10px;
	border: 1px solid black;
	margin: 10px;
}
```
- Values can also be set to percentages **%** for better access and usability
### Content
- Text alignment
	- Left
	- Right
	- Center
```css
.hero {
	text-align: center;
}
```
### Padding
- Can be set by 1, 2 or 4 values
- Affected by **background-color** attribute
```css
.hero {
	padding: 10px;
	/*same all round*/
}
```

```css
.hero {
	padding: 10px 20px;
	/*top & bottom + left & right*/
}
```

```css
.hero {
	padding: 10px 20px 30px 40px;
	/*top + right + bottom + left*/
}
```

- Padding can also be set individually
```css
.hero {
	padding-right: 10px;
	padding-top: 20px;
	padding-left: 30px;
	padding-bottom: 40px;
}
```

- Padding can use REM size
	- REM is relative measurement to the base font size
	- If base font size changes, everything changes
	- Useful for responsive design
```css
.hero {
	padding: 1rem;
	/*the 1x size of the font*/
}
```
### Border
- Has a 3 part syntax
	- Size, type and colour
```css
.hero {
	border: 1px solid black;
}
```
### Margin
- Works the same as [[#Padding]]
- Not affected by **background-color** attribute
## Display property
- **Inline** for continuous line
- **Block** to space things out
- **Inline-block** to get the benefits of both
	- Ability to set top and bottom padding
	- It all being in the same line
```css
.hero {
	display: inline;
}
```

```css
.hero {
	display: block;
}
```
### [[Display-flex]]
### [[CSS grid]]
## Pseudo classes
- Added with a column **:**
- Pseudo classes include
	- [[#Hover]]
	- [[#Other pseudo classes]]
### Hover
- Activates when mouse hovers over the element
```css
button:hover {
	background-color: red;
	transition: .3s ease all;
	transform: translateY(-5px);
}
```
- **Background-color** changes the backgound color
- **Transition** makes the animation last for a specified time
- **Transform** changes the position and size
### Other pseudo classes
- first-child
	- Selects the first child of an element
- nth-child(n)
	- Selects the n-th child of the element

```html
<div>
	<p>First paragraph</p>
	<p>Second paragraph</p>
	<p>Third paragraph</p>
</div>
```

```css
div p:first-child {
	color: green;
}

div p:nth-child(2) {
	color: red;
}
```