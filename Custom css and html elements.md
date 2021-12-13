# Custom css and html elements
## Custom css
You can add the following specific options to a page.  
How : in the top of the page, in the yaml section (between two ---), put
- cssclass: fullwidth, to make the page fullwidth
- cssclass: img-border-radius, to add border radius to your images in the page
- cssclass: img-box-shadow, to add box shadow to your page images
- cssclass: img-rounded, img-rounded-small (or img-rounded-medium or img-rounded-big), to make your images rounded in the page
- cssclass: blockquote-background, theme-light, to add a background for blockquotes in light theme page (theme-dark when in dark theme)
- cssclass: blockquote-serif, to choose the serif font for the blockquote
- cssclass: blockquote-bracket, to add a quotation mark for blockquote in the page
- cssclass: blockquote-text-center, to center the text in the blockquote

## Html and theme custom css
- you can display text in columns (.columns-2 or .columns-3) :
```
<div class=".columns-2">
YOUR TEXT
</div>
```

- you can add cards displayed in grid (.cards-2 -> 2 cards / row, .cards-3 -> 3 cards / row):
```
<div class="grid-cards">
	<div class="cards-2">
		<img="URL OF YOUR IMAGE">
		<div class="card-title">YOUR TITLE</div>
		<p>YOUR TEXT</p>
	</div>
	<div class="cards-2">
		<img="URL OF YOUR IMAGE">
		<div class="card-title">YOUR TITLE</div>
		<p>YOUR TEXT</p>
	</div>
</div>
```

- you can add buttons
```
<button><a href="TARGET URL">BUTTON TEXT</a></button>
```

- In a full width page, you can put text in "normal" width
```
<div class="text-normal-width">YOUR TEXT</div>
````

- Your can add a simple menu bar (.menu-page-v1 or menu-page-v2) in the top of the page, putting the following code :
```
<div class="menu-page-v1">
	<a href="OBSIDIAN URL OF THE PAGE 1">PAGE 1</a>
	<a href="OBSIDIAN URL OF THE PAGE 2">PAGE 2</a>
	<a href="OBSIDIAN URL OF THE PAGE 3">PAGE 3</a>
</div>
```

## Dataview and custom css
You can display an article view (like in blogs) with :
- In the yaml of the page: cssclass: dataview-articles-style
- In the page :
```dataview 
table without id ("<img src=" + cover + ">") as cover,file.ctime,file.name
from WHAT YOU WANT TO SHOW 
sort file.ctime desc 
```

