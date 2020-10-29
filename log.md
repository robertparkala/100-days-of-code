# 100 Days Of Code 2020-2021 - Log

#Day 1: October 28, 2020


**Today's Progress**: Started a new project, added HTML structure and css styling to navbar, showcase section and submit form.

**Thoughts:** It's the first day of this challenge but I've been learning HTML and CSS for exactly a month now. I'm seeing progress in relations to understanding classes better when going through my HTML structure and am thinking in more complex terms when it comes to CSS. For example I feel more confident now with flexbox, grid and also relative and absolute positioning.

A modern website with CSS, Flexbox, Grid, Animation, Span, Column, Rows

Creating an index.html and styles.css. and a boilerplate HTML content.

We used cdnjs.com font Awesome and copied this into our head element

Also, installed a atom-live server package because then it’ll automatically update my HTML preview on the web browser.

BASE CSS INPUTS

For example we set the body font-family to what we imported, color and also a more spaced out line height. We make sure that the lists are not bulleted and the anchor tag links don’t have an underline and text decoration is set to none and color.
For headings h1 and h2 we change the font weight to 300 for it to be a bit lighter also space out the line height and set a new margin of 10px to top and bottom and 0 to left and right.

MAKING A FLEXBOX CONTAINER CLASS

I don’t want to add a flex display to the container itself so I’m adding a utility class called flex. Remember how to bootcamp showed you how to do this as well.

NAVBAR LINKS

Setting the navbar links as in class navbar ul to display flex

SHOWCASE AREA

We’re using the container class again to maintain the specifications from our CSS and now adding grid so we can have similar functions as we did with flex.

SHOWCASE AREA USING GRID
As we can see, that by using the grid utility class in the container we are making it possible for us to style the container using the display attribute GRID. Now, by setting that to just GRID nothing happens, but we also need to specify the grid-template-columns and their width. In the screenshot we can see that each of the DIVS in the container is now changed into a grid item similar to a flexbox item and the first DIV is the size of 300px and the next one is fitted into a 200px container.

SHOWCASE AREA CARD WITH FORM

We pushed the form down with the relative position and then with the specification top and also gave it a height of 350px which gave us the scroll bar which we don’t want. What’s happening is we’re overflowing that element and we need to adjust it.

SHOWCASE INPUTS

Since we want to style the inputs that we created for the form but NOT the button itself we’ll create the style specification above and style the types TEXT and EMAIL thus targeting the values NAME, COMPANY NAME and EMAIL.

**Link to work:** Check my GitHub, Twitter @thelunarcoder and Instagram @thelunarcoder ! Everything's active :)

#Day 2: October 28, 2020


**Today's Progress**: Today's main draw were fexbox and grid. Created the stats section, CLI section and bottom Cloud and Read more sectio.

**Thoughts:** CREATING THE STATS AREA WITH GRID

Moving on to HTML now and creating the STATS area. Let’s break it down. First we created the section and containers because we don’t want the content to stretch out all the way and end where the rest of the stuff ends. We’ll have h3 and some utility classes for text, margin classes. my-1 is the margin class for Y axis. Those are utility classes so we don’t need to add so much CSS like margins and paddings on the element itself. Three areas for the stats, Deployment, Published and Projects.

Also, we’re adding 3 grid columns so we need a grid-3 class. my-4 is a larger margin class

i tag is for ICONS. Text-secondary is for our text color. Fa meaning Font Awesome and 3x meaning 3x times larger font.

We used the grid class remember, and what that’s doing is taking the firs two grids out of the three and splitting them into two. Now, we need to change that to three in the grid class to get them to align nicely.
We don’t want to use the original GRID class but we’ll use the one we intended for the icons.

CREATING A NEW CSS FILE TO SPLIT THING UP

Now we have the utilities in a new css file and also we added a link to our HTML to link the two css files. SO COOL!
Utility styles are for styles that are to be repeated throughout the page and basics styles reside in the style.css file.

ADDING MARGIN AND PADDING CLASSES

We added my-1-5 margin classes and set the margin for my-1 to 1rem for the H3 and my-4 to 3rem for the grid.

MODIFIYING THE STATS ICONS AREA

To set the STATS heading in the center and give it a max-width we will move it from a single line text to a max-width of 500px in the center of the page.

Changing the font-size to 35px. NOW, what I didn’t know is that you can move withing classes, for example, we are targeting the H3, that is in the grid class and is also in the stats class. WOW!

CREATING THE LOWER CLI WITH GRID

This is some clever work here. Pay attention that we are first using the CONTAINER class for everything because we already modified it and we can reuse the class. Now, also, we’re using the GRID class since we already have that on hand as well. WOW WOW WOW!

ADDING ANOTHER SECTION FOR READ MORE

Now this is interesting again. We’re creating another section and a class cloud so instead of adding the blue background color right on cloud, we’re adding another bg-primary class so we could use our variable with the primary color. Now, we’re going to center the text and we have a heading h2. Specific size class for headings, like lg = large.
Paragraphs are going to a bit bigger using the class lead.
Now, adding in the button with the anchor tag and also the styling is going to come from the same btn class we used before but we’re going to use the btn-dark and style that.
Also, we currently had the one DIV and we’re going to be adding in a second DIV as the image so we can take advantage of the two grid spaces we have witch are laid out with 1fr


**Link to work:** Check my GitHub, Twitter @thelunarcoder and Instagram @thelunarcoder ! Everything's active :)
