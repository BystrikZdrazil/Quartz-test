Obsidian official accent colour 138-92-245

Remove journal from graph view
>[!quote] Code
>-path: "09 - Daily notes"

[Dataview fundamentals](https://obsidian.rocks/dataview-in-obsidian-a-beginners-guide/#The-fundamentals-of-Dataview)
[Obsidian cheatsheet](https://obsidian-school.com/obsidian-basics/obsidian-cheat-sheet/)
[PDF to MD converter](https://notegpt.io/pdf-to-markdown-converter)
# Callouts
Callouts are a great way to visualize important information. You can add custom callouts with a simple CSS script.
## Obsidian originals
>[!note]
>```
>>[!note]
>>Lorem ipsum dolor sit amet
>```

>[!abstract]
>```
>>[!abstract]
>>Lorem ipsum dolor sit amet
>```
Aliases: **summary**, **tldr**

>[!info]
>```
>[!info]
>Lorem ipsum dolor sit amet
>```

>[!todo]
>```
>>[!todo]
>>Lorem ipsum dolor sit amet
>```

>[!tip]
>```
>>[!tip]
>>Lorem ipsum dolor sit amet
>```
>Aliases: **hint**, **important**

>[!success]
>```
>>[!success]
>>Lorem ipsum dolor sit amet
>```
>Aliases: **check**, **done**

>[!question]
>```
>>[!question]
>>Lorem ipsum dolor sit amet
>```
>Aliases: **help**, **faq**

>[!warning]
>```
>>[!warning]
>>Lorem ipsum dolor sit amet
>```
>Aliases: **caution**, **attention**

>[!failure]
>```
>>[!failure]
>>Lorem ipsum dolor sit amet
>```
>Aliases: **fail**, **missing**

>[!danger]
>```
>>[!danger]
>>Lorem ipsum dolor sit amet
>```
>Aliases: **error**

>[!bug]
>```
>>[!bug]
>>Lorem ipsum dolor sit amet
>```

>[!example]
>```
>>[!example]
>>Lorem ipsum dolor sit amet
>```

>[!quote]
>```
>>[!quote]
>>Lorem ipsum dolor sit amet
>```
>Aliases: **cite**
## Custom callouts
>[!calendar]
>```
>>[!calendar]
>>Lorem ipsum dolor sit amet
>```

>[!banana]
>```
>>[!banana]
>>Lorem ipsum dolor sit amet
>```
# Code box setup
```C#
int age = 20;

if (age > 18 && age < 65) {
	Console.WriteLine("This person is an adult");
}
```

Universal ALT code for backtick: __96__

Check out [Envato Elements](https://elements.envato.com/?utm_campaign=yt_tutsplus_B-ytMSuwbf8&utm_medium=referral&utm_source=youtube.com&utm_content=description)
# Date progress bar
```dataviewjs

var a = moment("2024-01-01");
var b = moment("2024-12-31");


var n = moment()
var t = moment().startOf('day');

let q =  b.diff(a, 'days');
let p =  b.diff(t, 'days');
let r =  t.diff(a, 'days');

let h = n.diff(a, 'hours');
let i = b.diff(a, 'hours');

let html = `**YEAR 2024** <progress style="height:10px;width:20%" value="`+h+`" max="`+i+`"></progress>`

if (r>0 && r<q) {
	html +=  `    **` +(h/i*100).toFixed(0)+`%** 
	| `
	html += +p+` days remaining` 
} else if (r==0) {
	html += `    **` +(h/i*100).toFixed(0)+`%** 
	| `+ p + ` days remaining`
} else if (r==q) {
	html += `   Ends today`
} else if (r>q) {
	html += `   Ended `+-p+` days ago`
}else {
	html += `   `+-r+` days remaining`
}

dv.paragraph(html)
```
# Commander layout
![[comander-layout-visual.png]]
# Heading 1
## Heading 2
### Heading 3
#### Heading 4
##### Heading 5
###### Heading 6
Normal 
**Bold**
*Italic*
>[!warning] Does this look good?
>Well it seems like it

>[!tip] Here's a tip for you
>Don't give up

| Syntax  | Description |
| ------- | ----------- |
| `- [ ]` | to-do       |
| `- [/]` | incomplete  |
| `- [x]` | done        |
| `- [-]` | canceled    |
| `- [>]` | forwarded   |
| `- [<]` | scheduling  |
| `- [?]` | question    |
| `- [!]` | important   |
| `- [*]` | star        |
| `- ["]` | quote       |
| `- [l]` | location    |
| `- [b]` | bookmark    |
| `- [i]` | information |
| `- [S]` | savings     |
| `- [I]` | idea        |
| `- [p]` | pros        |
| `- [c]` | cons        |
| `- [f]` | fire        |
| `- [k]` | key         |
| `- [w]` | win         |
| `- [u]` | up          |
| `- [d]` | down        |
