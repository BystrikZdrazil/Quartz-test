# Welcome, Bystrík
> [!multi-column]
> > ![[Mobile dashboard#Your assignments]]
> 
> > ![[Mobile dashboard#Important dates to keep track of]]

---

> [!multi-column]
>
> >```tracker
> > searchType: fileMeta
> > searchTarget: numWords
> > folder: 09 - Daily notes/Journal
> > line:
> > 	title: Word Counter
> > 	yAxisLabel: Words
> > 	lineColor: '#9446f8'
> > 	yMin: 0
> > ```
>
> > ```tracker
> >searchType: frontmatter
> >searchTarget: Time Studied, Time Worked
> >datasetName: Time Studied, Time Worked
> >folder: 09 - Daily notes/Journal
> >line:
> >	title: Working and Studying
> >	lineColor: cyan, blue
> >	yAxisLabel: Hours
> >	showLegend: True
> >	yMin: 0
> >	yMax: 5
> >```
>
> > ```tracker
> >searchType: frontmatter
> >searchTarget: Day Rating
> >datasetName: Day Rating
> >folder: 09 - Daily notes/Journal
> >line:
> >	title: Day rating
> >	lineColor: orange
> >	yAxisLabel: Rating
> >	yMin: 0
> >	yMax: 10
> >```
> 
> >```tracker
> >searchType: frontmatter
> >searchTarget: Yoyoing
> >folder: 09 - Daily notes/Journal
> >datasetName: Yoyoing
> >month:
> >	startWeekOn: mon
> >	color: '#9446F8'
> >```

---

> [!multi-column]
>
> > [!tip]+ Recently Created
>>```dataview
> >List
> >From ""
> >sort file.ctime Desc
> >Limit 5
> >```
>
> > [!success]+ Recently Modified
>> ```dataview 
> > List 
> > From ""
> > sort file.mtime Desc
> > Limit 5
> > ```

---

> [!multi-column]
>
> > [!calendar]+ PONDELOK
> > **Európska Únia**
> > 09:15 - 10:45
> > D111
> > ---
> > **Marketing**
> > 13:30 - 15:00
> > B107
>
> > [!calendar]+ UTOROK
> > **Angličtina**
> > 11:00 - 12:30
> > D105
> > ---
> > **Základy Ekonómie**
> > 13:30 - 15:00
> > B205
> > ---
> > **Európska Únia**
> > 15:15 - 16:45
> > B202
> 
> > [!calendar]+ STREDA
> > **Právo**
> > 07:30 - 10:30
> > B104
> > ---
> > **Marketing**
> > 11:00 - 12:30
> > B204
> 
> > [!calendar]+ ŠTVRTOK
> > **Základy Ekonómie**
> > 07:30 - 09:00
> > B108
> > ---
> > **Kulturistika**
> > 11:00 - 12:30
> > Fitko Horský Park

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