# Custom css and html elements
## Custom css
You can add the following specific options to a page.  
How : in the top of the page, in the yaml section (between two ---), put
- cssclass: fullwidth, to make the page fullwidth
- cssclass: img-border-radius, to add border radius to your images in the page
- cssclass: img-box-shadow, to add box shadow to your page images
- cssclass: img-rounded, img-rounded-small (or img-rounded-medium or img-rounded-big), to make your images rounded in the page
- cssclass: img-bw, to display black and white images in the page
- cssclass: img-float-left (or img-float-right)
- cssclass: blockquote-background, theme-light, to add a background for blockquotes in light theme page (theme-dark when in dark theme)
- cssclass: blockquote-serif, to choose the serif font for the blockquote
- cssclass: blockquote-bracket, to add a quotation mark for blockquote in the page
- cssclass: blockquote-text-center, to center the text in the blockquote

You can display each image in a different way with this synthax:

```
![img-border-radius](url image)
```

Works with the class for images above +
img-profile, img-portrait, img-banner

## Html and theme custom css
- you can display <aside>
```
<aside><p>YOUR TEXT</p></aside>
```
<img width="759" alt="Capture d’écran 2021-12-13 à 18 13 29" src="https://user-images.githubusercontent.com/29182877/145857817-bf71530b-e620-4f3d-899f-63a3f0068952.png">
	
- you can display text in columns (.columns-2 or .columns-3) :
```
<div class=".columns-2">
YOUR TEXT
</div>
```
<img width="903" alt="Capture d’écran 2021-12-13 à 17 53 16" src="https://user-images.githubusercontent.com/29182877/145854571-01515d3c-dfbd-464a-88fe-160d701e252c.png">

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
<img width="1088" alt="Capture d’écran 2021-12-13 à 17 56 32" src="https://user-images.githubusercontent.com/29182877/145855187-ac9c2020-0c1e-417d-9b3b-1bcd64456485.png">

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
<img width="1440" alt="Capture d’écran 2021-12-13 à 17 51 47" src="https://user-images.githubusercontent.com/29182877/145854325-ab8a1847-3a0f-4365-be79-7205182f6905.png">

## Dataview and custom css
You can display an article view (like in blogs) with :
- In the yaml of the page: cssclass: dataview-articles-style
- In the page :
```dataview 
table without id ("<img src=" + cover + ">") as cover,file.ctime,file.name
from WHAT YOU WANT TO SHOW 
sort file.ctime desc 
```
<img width="1294" alt="Capture d’écran 2021-12-13 à 17 50 27" src="https://user-images.githubusercontent.com/29182877/145854093-74ea892c-1298-4bb7-9c7f-b1981662a89a.png">

