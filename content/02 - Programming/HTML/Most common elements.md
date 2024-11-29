# What are the most common elements in HTML
## Paragraph
```html
<p>
	
</p>
```
- Used to separate long form text content
## Line break
- Used to force move text of the same element into another line
```html
<p>
	First line<br>Second line
</p>
```
## Image
- Visual enhancement
- Must include source
```html
<img src="yoyo.png" alt="yoyo">
```
## Anchor
- Links
- Require href (HyperText reference) [[Attributes in HTML]], that is the link we want the user to be sent to
```html
<a href="https://google.com">
	Go to Google
</a>
```
## Ordered lists
- Viewed as numbered lists
- Can be nested inside other lists
```html
<ol>
	<li>First</li>
	<li>Second</li>
	<li>Third</li>
</ol>
```
## Unordered lists
- Viewed as bullet points
- Can be nested inside other lists
```html
<ul>
	<li>First</li>
	<li>Second</li>
	<li>Third</li>
</ul>
```
## List item
- Used in [[#Ordered lists]] and [[#Unordered lists]] for each item
```html
<li>A list item</li>
```
## Button
- Can be used as links
- Can be used with CSS
```html
<button>
	Click me
</button>
```
## Forms
- Users can login, create posts, make payments and more
- Done by wrapping one or more [[#Input]] elements
```html
<form>
	<p>Text</p>
	<input type="text">
	
	<p>Email</p>
	<input type="email">
	
	<p>Password</p>
	<input type="password">
</form>
```
### Input
- Many types of inputs
	- Text
	- Email
	- Password
	- Checkbox
	- Radio
	- Dropdown menu
```html
<form>
	<p>Text</p>
	<input type="text">
	
	<p>Email</p>
	<input type="email">
	
	<p>Password</p>
	<input type="password">
	
	<p>Checkbox</p>
	<input type="checkbox">
	<input type="checkbox">
	<input type="checkbox">
	
	<p>Radio</p>
	<input type="radio">
	<input type="radio">
	<input type="radio">
	
	<p>Dropdown menu</p>
	<select>
		<option>First</option>
		<option>Second</option>
		<option>Third</option>
	</select>
</form>
```

You can link an input to a label with an ID on the input and a for  [[Attributes in HTML]] on the label. When you click the label it will activate your input.
```html
<form>
	<p>Checkbox</p>
	<label for="cb1">First</label>
	<input type="checkbox" id="cb1">
	<label for="cb2">Second</label>
	<input type="checkbox" id="cb2">
	<label for="cb3">Third</label>
	<input type="checkbox" id="cb3">
</form>
```
## Style
- Flips the language we are writing in
- Style flips to CSS
- To keep things organized, this is not much recommended because you can [[Link a file]]
```html
<style>
	h1 {
		font-size: 20px;
		color: white;
	}
</style>
```
## Script
- Flips the language we are writing in
- Script flips to JavaScript
- To keep things organized, this is not much recommended because you can [[Link a file]]
```html
<script>
	var element = document.querySelector('h1');
	element.style.color = 'red';
</script>
```
# [[Container elements]]
# Less common elements
- Can be done with CSS

```html
<u>
	underline
</u>
```

```html
<b>
	bold
</b>
```

```html
<i>
	italic
</i>
```

```html
<strong>
	bold, improves accessibility
	in reader view
</strong>
```

```html
<em>
	italic, improves
	accessibility in reader view
</em>
```