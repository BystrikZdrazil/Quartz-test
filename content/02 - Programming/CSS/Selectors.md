# What are CSS selectors
- Select elements from HTML document
	- Can select
		- [[Elements]]
		- [[Class]]
		- [[ID]]
```html
<h1>
	Hello
</h1>

<h2 class="secondary">
	Welcome to my site
</h2>

<h3 id="main-text">
	Here's a paragraph
</h3>
```

- [[Elements]] are just plain symbols
- [[Class]]es start with a dot at the beginning
- [[ID]]s start with a hashtag
```css
h1 {
	/* styles here */
}

.secondary {
	/*styles here*/
}

#main-text {
	/*styles here*/
}
```
### Chains
- Comma chains multiple elements
- Select this *and* this
```css
h1, h2 {
	/*styles here*/
}
```
### Inside
- Space syntax together subelements
- Select this *inside* this
```css
h1 h2 {
	/*styles here*/
}
```
### Carrot
- Carrot (>) selects one level deep
- All elemts *one level deep in* .hero
```css
.hero > h2 {
	/*styles here*/
}
```