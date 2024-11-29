# Welcome, Bystrík
## Your assignments
**You have no pending assignments**
## Important dates to keep track of
```dataviewjs

var a = moment("2024-11-20");
var b = moment("2024-12-11");


var n = moment()
var t = moment().startOf('day');

let q =  b.diff(a, 'days');
let p =  b.diff(t, 'days');
let r =  t.diff(a, 'days');

let h = n.diff(a, 'hours');
let i = b.diff(a, 'hours');

let html = `**MRK TEST**     <progress style="height:10px;width:20%" value="`+h+`" max="`+i+`"></progress>`

if (r>0 && r<q) {
	html +=  `    **` +(h/i*100).toFixed(0)+`%** 
	| `
	html += +p+` days remaining` 
} else if (r==0) {
	html += `    **` +(h/i*100).toFixed(0)+`%** 
	| `+ p + ` days remaining`
} else if (r==q) {
	html += `   
	Ends today`
} else if (r>q) {
	html += `   
	Ended `+-p+` days ago`
}else {
	html += `   `+-r+` days remaining`
}

dv.paragraph(html)
```

```dataviewjs

var a = moment("2024-11-20");
var b = moment("2024-12-11");


var n = moment()
var t = moment().startOf('day');

let q =  b.diff(a, 'days');
let p =  b.diff(t, 'days');
let r =  t.diff(a, 'days');

let h = n.diff(a, 'hours');
let i = b.diff(a, 'hours');

let html = `**OAHPR TEST**     <progress style="height:10px;width:20%" value="`+h+`" max="`+i+`"></progress>`

if (r>0 && r<q) {
	html +=  `    **` +(h/i*100).toFixed(0)+`%** 
	| `
	html += +p+` days remaining` 
} else if (r==0) {
	html += `    **` +(h/i*100).toFixed(0)+`%** 
	| `+ p + ` days remaining`
} else if (r==q) {
	html += `   
	Ends today`
} else if (r>q) {
	html += `   
	Ended `+-p+` days ago`
}else {
	html += `   `+-r+` days remaining`
}

dv.paragraph(html)
```

```dataviewjs

var a = moment("2024-11-19");
var b = moment("2024-12-03");


var n = moment()
var t = moment().startOf('day');

let q =  b.diff(a, 'days');
let p =  b.diff(t, 'days');
let r =  t.diff(a, 'days');

let h = n.diff(a, 'hours');
let i = b.diff(a, 'hours');

let html = `**ZEK TEST**     <progress style="height:10px;width:20%" value="`+h+`" max="`+i+`"></progress>`

if (r>0 && r<q) {
	html +=  `    **` +(h/i*100).toFixed(0)+`%** 
	| `
	html += +p+` days remaining` 
} else if (r==0) {
	html += `    **` +(h/i*100).toFixed(0)+`%** 
	| `+ p + ` days remaining`
} else if (r==q) {
	html += `   
	Ends today`
} else if (r>q) {
	html += `   
	Ended `+-p+` days ago`
}else {
	html += `   `+-r+` days remaining`
}

dv.paragraph(html)
```

```dataviewjs

var a = moment("2024-11-22");
var b = moment("2024-12-13");


var n = moment()
var t = moment().startOf('day');

let q =  b.diff(a, 'days');
let p =  b.diff(t, 'days');
let r =  t.diff(a, 'days');

let h = n.diff(a, 'hours');
let i = b.diff(a, 'hours');

let html = `**FTVŠ TEST**     <progress style="height:10px;width:20%" value="`+h+`" max="`+i+`"></progress>`

if (r>0 && r<q) {
	html +=  `    **` +(h/i*100).toFixed(0)+`%** 
	| `
	html += +p+` days remaining` 
} else if (r==0) {
	html += `    **` +(h/i*100).toFixed(0)+`%** 
	| `+ p + ` days remaining`
} else if (r==q) {
	html += `   
	Ends today`
} else if (r>q) {
	html += `   
	Ended `+-p+` days ago`
}else {
	html += `   `+-r+` days remaining`
}

dv.paragraph(html)
```

```dataviewjs

var a = moment("2024-10-27");
var b = moment("2025-01-25");


var n = moment()
var t = moment().startOf('day');

let q =  b.diff(a, 'days');
let p =  b.diff(t, 'days');
let r =  t.diff(a, 'days');

let h = n.diff(a, 'hours');
let i = b.diff(a, 'hours');

let html = `**KARATE EXAM**     <progress style="height:10px;width:20%" value="`+h+`" max="`+i+`"></progress>`

if (r>0 && r<q) {
	html +=  `    **` +(h/i*100).toFixed(0)+`%** 
	| `
	html += +p+` days remaining` 
} else if (r==0) {
	html += `    **` +(h/i*100).toFixed(0)+`%** 
	| `+ p + ` days remaining`
} else if (r==q) {
	html += `   
	Ends today`
} else if (r>q) {
	html += `   
	Ended `+-p+` days ago`
}else {
	html += `   `+-r+` days remaining`
}

dv.paragraph(html)
```
## School Timetable
| **Predmet**      | **Deň**  | **Čas**       | **Miesto** |
| :--------------- | :------- | :------------ | :--------- |
| Európska Únia    | PON      | 09:15 - 10:45 | D111       |
| Marketing        | PON      | 13:30 - 15:00 | B107       |
| **————**         | **————** | **————**      | **————**   |
| Angličtina       | UTO      | 11:00 - 12:30 | D105       |
| Základy ekonómie | UTO      | 13:30 - 15:00 | B205       |
| Európska Únia    | UTO      | 15:15 - 16:45 | B202       |
| **————**         | **————** | **————**      | **————**   |
| Právo            | STR      | 07:30 - 10:30 | B104       |
| Marketing        | STR      | 11:00 - 12:30 | B204       |
| **————**         | **————** | **————**      | **————**   |
| Základy ekonómie | ŠTV      | 07:30 - 09:00 | B108       |
| Telesná          | ŠTV      | 11:00 - 12:30 | Fitko      |
```dataviewjs
// Calculate days since first note
const files = dv.pages()
const oldestFile = files.sort(f => f.file.ctime)[0]
const daysSinceStart = Math.floor((Date.now() - oldestFile.file.ctime) / (1000 * 60 * 60 * 24))
// Count total notes
const totalNotes = files.length
// Count unique tags
const allTags = files.flatMap(p => p.file.tags).distinct()
const totalTags = allTags.length
// Create a visually appealing display that works in both light and dark modes
dv.paragraph(`<div style="
  background-color: var(--background-secondary);
  border: 1px solid var(--background-modifier-border);
  border-radius: 10px;
  padding: 20px;
  text-align: center;
  font-family: var(--font-text);
  color: var(--text-normal);
">
  <h2 style="color: var(--text-normal);">📊 Obsidian Stats</h2>
  <p style="font-size: 18px; margin: 10px 0;">
    🗓️ You've been using Obsidian for <strong>${daysSinceStart}</strong> days
  </p>
  <p style="font-size: 18px; margin: 10px 0;">
    📝 You have <strong>${totalNotes}</strong> notes
  </p>
  <p style="font-size: 18px; margin: 10px 0;">
    🏷️ You're using <strong>${totalTags}</strong> unique tags
  </p>
</div>`)
```