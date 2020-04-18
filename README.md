# MDN-Fundamental-Layout-Comprehension
Project from MDN: "Fundamental Layout Comprehension
This project is from MDN webdocs. (https://developer.mozilla.org/en-US/docs/Learn/CSS/CSS_layout/Fundamental_Layout_Comprehension)
My goals for this project are to complete the assignment successfully and practice using github.

Update: Added initial files from project source:
1. index.html
2. style.CSS
3. img folder with images

Update:
First change is the nav bar.
The nav bar is currently in flow arranged on top of each other vertically.
I will create a flex container as the bar.
Then center the items on the nav bar as shown in the picture.

Actually needed to nav ul because that is the proper container for the nav items.
so i added
nav ul {
	display: flex;
	justify-content: space-between;
}

Now I need to float the balloon picture to the left. I added float left to class .feature.
Now I need to add space to the right. I went with the following:
.feature {
	padding-right: 1rem;
}

Next I want to arrange the main part of the article along side with the photography section to the right.
The body is already in a grid class which hints at using a grid system or the like.
Eyeballing the row it looks like 9 units for the left side and 3 on the other. So I will create a grid-template-columns with 12 fr1 and split about 8 / 4

Added some margin adjustments to image to create space.

Now next step is to get the aside to display correctly. i tried flex at first, but that didn't work because i wanted columns so i went with another grid.

finally I add grid-gap to the phots to create separation.

Page now looks like example page.

TODO edit documentation in a more readable format.  
