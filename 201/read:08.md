# Read: 08 - More CSS Layout
## Layout
- **CSS** treats **HTML** elements as boxes
- if we have a bigger box that has a smaller box inside it
	- the bigger box is considered a parent
	- the smaller box is considered a child
- **CSS** can control the positioning of the elements
	- normal flow:
		- elements sit on top of the next one
	- relative positioning:
		- moves elements to where it would be in normal flow 
	- absolute positioning:
		- the box no longer affects other elements position
	from duckett html. link:
	file:///C:/Users/LTUC/Desktop/duckett_html.pdf
- you can also use box offset properties:
	- fixed positioning 
	- floating elements
- liquid layouts:
	- uses percantages to specify the width of each box
	
from duckett html. link:
	file:///C:/Users/LTUC/Desktop/duckett_html.pdf

### screen sizes
- not all screens have the same size so the webpage can crash or look different when openen in 
	different screen sizes so css came with a solution to this which is
	@media (min-width: 767px) and (max-width: 1024px)
	this is an example i got from link:
	https://intercom.help/elegantthemes/en/articles/2800710-applying-css-changes-for-a-specific-screen-resolution
	- it's bascially working if screen size is bigger then 767px 
		but is samller than 1024px
### css
- you can use multiple sheets to style your code
	- can use one for colors
	- one for sizes..etc
