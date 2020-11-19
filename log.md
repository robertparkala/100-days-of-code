# 100 Days Of Code 2020-2021 - Log by Robert Parkala



#Day 1: October 28, 2020



**Today's Progress**: Started a new project called Blue Origin Cloud Hosting, added HTML structure and css styling to navbar, showcase section and submit form.

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

**Link to work:** Check my GitHub @robertparkala, Twitter @thelunarcoder and Instagram @thelunarcoder ! Everything's active :)



#Day 2: October 29, 2020



**Today's Progress**: Today's main draw were flexbox and grid. Created the stats section, CLI section and bottom Cloud and Read more section.

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

**Link to work:** Check my GitHub @robertparkala, Twitter @thelunarcoder and Instagram @thelunarcoder ! Everything's active :)



#Day 3: October 30, 2020



**Today's Progress**: Today I finished the supported languages and footer sections. Added social media links and media queries for both tabled and mobile.

**Thoughts:**

ADDING SUPPORTED LANGUAGES SECTION

Created a languages section and h2 with the medium class, with text center and we’ll do my-2 for margins. Feels like we’re using Bootstrap but it’s actually thorough and custom CSS. We’re going to use flex for this because we want to align them into a row and each one will be wrapped in a card and h4 and an image underneath. Images/logos.
CSS that we’re adding .languages .card with text align and margins for top/left side bottom and right side. And adding onto the flex we’re adding flex-wrap and set that to wrap.

Increased h4 size and margin bottom. Also, set the hover attribute to the card elementso that the images would move up a little bit and that’s the transform property on the Y axis and up means a negative value on the axis.
For the smoother effect we’ll add a transition onto the transform property with the ease in.

FOOTER SECTION

Creating the footer bar starts with a footer tag with a class of bg dark and padding py-5
Container is going to be grid 3 and we’ll have a div with the site name in the h1 and a paragraph with the Copyright, &copy gives us the copyright symbol. That was the firs grid item
We’ll do a NAV tag with the ul and links to Home, Features and Docs and a Privacy policy but I didn’t want to create links that go nowhere.
Final DIV as the grid item will be the Social. With font awesome the social media icons will be FAB abbreviation.
Also, we added in to make the social media link anchor tags white and spaced out our social media icons with margin from left and right.

ADDING MEDIA QUERIES TO MAKE THE PAGE RESPONSIVE

Adding two separate media queries in our style.css. First one for tablets and under and the second one for mobile. For Tablets, anything under 768x will be styled here. For mobile we want to capture anything under 500px. For the menu that’s going to be fine on tablets even if there’s more items but for mobile we’ll change things up.

In mobile Navbar height set to 110px, to put the menu items under the logo. Navbar we have a class flex, so it’s a row by default so we’ll set it to column with flex direction which will put the logo and the UL on top of each other. For the navbar UL we’ll add padding and a transparent background.

Style all the grids first and I want to stack everything, so tablets and under. Instead of two and three columns I want everything in one column. Grid classes first! Setting the grid template columns to 1fr so it would take up the entire column and in the CLI area we have two rows so we’ll set the grid template rows to 1fr as well for it to take up only 1.

Initially the showcase is 400 px and we’ll set the showcase height to auto so it would take up the entire space.  So to form wouldn’t be on the text. Showcase-text we’ll align to the center and we’ll push it down with the margin top for 40px.
I want to move the showcase form to the middle and we’ll use the justify-self: center; to do that. We’ve used justify content a bunch so that’s going to be on a flexbox or a grid container.
Justify-self we use on an actual grid or flex item to justify just that item. Margin to auto. Now the form’s in the middle.

**Link to work:** Check my GitHub @robertparkala, Twitter @thelunarcoder and Instagram @thelunarcoder ! Everything's active :)



#Day 4: October 31, 2020 Happy Halloween, boo!



**Today's Progress**: Today got an early start and I thought that I’d first spend an hour or more on Stack Overflow answering some of my first questions ever. As far as coding today, I created the Features page, which is the second of the three pages that are going to be on it. Added the navbar, features heading, img and footer.

**Thoughts:**

CREATING THE FEATURES PAGE

Created a new file features.html and copied all of the content from index.html and we’re keeping the nav bar, footer. Removed everything UP from Footer and until Showcase included.

This page is not going to be as complex because we already have all the helper classes ready and most of the elements.

Now, we’ve added the Head section  and a subsequent DIV, that also is styled with the container an now a grid attribute. We’re using the same bg-primary and py-3 classes to style our background and padding. Also, using the XL class for H1 and LEAD for our paragraph.
We entered an image as our second grid item.
Then we added the Features CSS for the picture and made it smaller and pushed it to the end of the container grid with justify-self: flex-end;

**Link to work:** Check my GitHub @robertparkala, Twitter @thelunarcoder and Instagram @thelunarcoder ! Everything's active :)

#Day 5: November 1, 2020

**Today's Progress**: Finished the Features page with subhead and subhead grid.

**Thoughts:**

CREATING THE SUBHEAD AND SUBHEAD GRID

Created the features sub head section and a new container grid. Added heading H1 with a class of medium and paragraph with some dummy text. Added a new image server 2.

Modified CSS to push the subhead image to the container end and modified the width to be a bit bigger than the features server logo.

We’re making a grid of cards but we’re also adding the FLEX because we want to align these items using flex.
Adding an icon with Font Awesome and then we’ll add a paragraph and add lorem30 dummy text. Now we need 6 of those divs and just modify the icons with font awesome.

We’re adding special styles so that the grids would not be sitting next to each other. So specifically, in the features main we’re targeting the icons and adding a margin to the right to push then away from the text a little bit.

For the grid itself we’re going to do some spanning but before we’re going to set the grid-3 onto the div container class to give it 3 columns and add a bit of padding to the features main in CSS.

Now, we want the firs grid element to take up (span) one row and span three columns. Also the second element to span one row and take up 2 columns. We can do that by addressing the first child in the grid and subsequently with the nth-child(2) we can address the second child. WOW, totally now stuff here!

**Link to work:** Check my GitHub @robertparkala, Twitter @thelunarcoder and Instagram @thelunarcoder ! Everything's active :)



#Day 6: November 2, 2020



**Today's Progress**: Finished the Blue Origin Cloud Hosting Website, which is now responsive across platforms.

**Thoughts:**

CREATING THE DOCUMENTATION PAGE

We copied the features page as a boiler for the docs.html and also changed the section class from features-head to docs-head.

DOCUMENTATION MAIN

The docs main is going to be a similar container grid class DIV that has second DIV with the card class in it. We’re adding a heading H3 and a navbar with an unordered list with list items and also a second heading with an H3 and a similar list.

INTRODUCTION

We create another DIV with the class card an since it’s housed in a div container grid then it’ll format into 2 columns of 1fr. Inside the card we have a heading h2 and a paragraph with an alert alert-success DIV that houses a font awesome icon. 

LINKS AND LISTS 

We added a heading in the card and a paragraph. Under the paragraph we created a link with an <a> tag. And set it up as a button Install CLI. Now, under the button we added the Requirements heading h3 and formulated those requirements into a unordered list. 
Under the list we added another H3 and a Paragraph with a pre code tag that allows us to add in the terminal code lines. Make sure to read more about this!

We’ll add a margin to the docs main heading and we will also modify the docs-main .grid to take up 1fr for the first grid item and 2fr for the second grid item. 

ALERT SUCCESS AND ERROR

Now, we’re styling the Alert class and it’s similar to the Bootstrap alerts where you can see SUCCESS, DANGER etc. 

We’re setting the alert class color to light color with the custom properties (variables)

STYLING THE CODE IN PRE TAGS

We’re making the pre tags look like they would be off of a real documentation page.

STYLING THE PRIMARY COLOR OF LI ITEM

We’re setting a text primary class to the Introduction LI item. Using the bg. background colors and btn colors and copying down but changing the background color to just color to make the Introduction blue. 

MAKING THE INNER PAGES RESPONSIVE 

We added the features main grid and the docs main grid to the 768x. Now the Features grid starts to stack up. Now we want to center  our images on both the features head, subhead and on the docs head. Now we’re working on the Features grid span and we’re targeting the grid’s first child and the nh-child(2)
and setting the grid-columns to 1 so they would stack underneath each other.

ANIMATIONS

We’re creating animations in our style.css under Footer with @keyframes and adding slide-in’s to certain elements for right, left, top and bottom. We’re actually manipulating translate X and translate Y.

We want it to start off screen and it will start negative 100% on the left with this keyframe.

And end up in it’s normal position 0 at 100%

Same thing for the slide in from the Right. Now it will start at positive 100% to the right and will return to its original position 0 at 100%
We’re doing the same with Top and Bottom but remember that now we’re manipulating the Y axis and returning the element back to its position in the X axis. Super cool stuff here! 

Slide in from the Left is going to go in the Showcase Text (which we need to create) and Slide in From Right will go on the showcase form. We specified the animation action from our keyframes, then the duration and what kind of movement. Now we want the STATS to come out the bottom.

DEPLOYING TO NETLIFY

Deploying to Netlify and creating a Git Repository there.

ADDING THE FORM FUNCTION FROM NETLIFY

So that our form would actually work on our home page. Adding this to our index.html

ADDING THE SPAM FILTER

Recaptcha or Honeypot. Recaptcha would mes up our layout bot we’re adding the honeypot so if you’re a bot you’ll fill it out and if you’re a human you wont. 

Also we’re adding in the paragraph wit the hidden like so. This is going to hide the honeypot based on the hidden class. Also, we’re going to add CSS to style.css and hide the visibility and since it will still take up space, we’ll set the height to 0.

NOW WE’RE SET TO DEPLOY

Opening up our VSCode terminal with command + tilde (which is right under the escape button) and adding 
git init. GitHub's got our repository. Now, we’re going to Netlify again and creating a new repository. Following the steps that are laid ouf by Netlify. Deployed at https://blue-origin-cloud-hosting.netlify.app/

**Link to work:** Check my GitHub @robertparkala, Twitter @thelunarcoder and Instagram @thelunarcoder ! Everything's active :)



#Day 7: November 3, 2020 



**Today's Progress**: Started a new project, a product landing page for Audio-Phonics headphones.

**Thoughts:** 

HTML and INTRO

Creating a product landing page, for headphones, with lightbox gallery and submit form. Deploy it to Netlify.
We’ll have a navbar, showcase area, dark overlay area and a photo gallery with grid and lightbox (simple lightbox). In the footer we’ll have menus, email subscribe form.

Bringing on the css and js from lightbox. Using Google Font Catamaran.

IMPLEMENTING AJAX GOOGLE APIS
ADDING A jQUERY SCRIPT 

Implemented the Ajax.googleapis.com so we could run the simple-lightbox.min.js file with our gallery and links.
And the script function is a line of jQuery. jQuery is a JavaScript library designed to simplify HTML DOM tree traversal and manipulation, as well as event handling, CSS animation, and Ajax.

CREATING THE NAVBAR

Created the navigation bar with hash links and added the id to body so when we click the home link.

ASSIGNING ROOT COLORS

CREATING OUR RESETS

Box sizing to border  box, so that padding and boarders don’t ad width to the element. Zeroing out the margin and padding.

BASE STYLES

For the body we’re setting the font family, line height, color and font size.
Headings will have a different line height.
Links will have a custom properties color and a text decoration of none so there’s no underline.
From the unordered list we take away the bullet points with list style set to none.
For any image we have on this site we want it to take a 100Q% of the width of the container.

CREATING THE CONTAINER CLASS AND GRID SYSTEM

We’ll be creating the container class and we’re also going to use the grid system to align the logo on the left and the menu on the left. 

For the container we’ll set the max width 1100px which is pretty common and margin auto so it gets put in the middle and here’s even margin from the left and right. 
Overflow will be hidden because we don’t want anything breaking out of the container. 
Padding will be set to 0 from top and bottom and 2rem from left and right.

STYLING THE NAVBAR 

We don’t want to display grid on the navbar class, because if we do that then the container is going to be the grid item but we want to display the H1 and the UL as our two grid items. Setting the display to grid for the navbar container and specifying the way the space will be laid out, 1fr and 1fr or repeat

SHOWCASE AREA

We’re going to us a section and give it a class of section-a and have a DIV with a container underneath to push everything in the middle just like with the navbar. Another DIV with H1 and Paragraph and an anchor link with a button class underneath. 
Under the DIV we’ll have an image showcase.jpg

MAKING THE GRID LAYOUT

We want to display the grid on the container not on the section-a because when we do it on section-a the container will be the only grid item but we want two.
Now were’ creating a section-a separately because we want to add some margin top and bottom. We could also create some utility classes for margin, padding if we’d want like we did with the previous project but we’re keeping it simple.

On the container we’ll set the display to grid and grid template-columns to repeat 2 1f
Creating a small grid gap and now with align-items and justify-content set to center we’ll center everything 

Also, we added a bit of margin to the navbar because the photo of th headphones is touching too close to the Home and About.

We added a font-size to the section-a H1 and a color from the custom properties.
And section-a paragraph got a margin top of 1rem to help spread it out a bit more and a fon-size of 1.2 rem to help the text be more evenly distributed.


**Link to work:** Check my GitHub @robertparkala, Twitter @thelunarcoder and Instagram @thelunarcoder ! Everything's active :)



#Day 8: November 4, 2020 



**Today's Progress**: Creating the overlay section and gallery.

**Thoughts:** 

STYLING THE BUTTON 

We’re using display as inline-block so we can add width and padding. It doesn’t take up its own line compared to block items. Don’t forget to add a cursor pointer and change the font size to match the purpose of the page. For a product landing page, we’re making everything a bit bigger to make it stand out. And of course the border radius and here we’re going strong with this one to match the curves of the headphones as well.
We’re also setting the button hover to be a bit different so it’s noticeable when clicking.

CREATING THE OVERLAY SECTION

Let’s add the markup for that first and we’re breaking everything up into sections. Adding a div with the class overlay and in that one a section-b with H3 and H2 and a paragraph.

OVERLAY TEXT

So, with section b’s CSS we’ll position it relative, because we’re going to position the overlay absolute withing section-b and since section-b is its container it needs to be positioned relative. And this is where we’ll add the image as our background ../img meaning up one level to the img folder. Adding no repeat, so it doesn’t repeat, positioning bottom center and cover the whole space. We’ll set the height of the img to 600px.

Position is set to absolute withing the section -b or within wrapper is relative. Top 0, left 0 so the top left corner (remember how you learned about the square positioning with Angela Yu, this is it). And we want it to expand a 100% height and also a 100% width. So it cover ther whole area. Setting the background color to rgba which comes from our custom properties color. We can also change the color opacity as the last value of the rgba.

SECTION B TEXT
Setting the color to white and set the height 100% of its container. We’re using flex, however I don’t want it to be aligned horizontally, so we want to change the flex direction to column. We want to align everything to the center with algin items and justify content and text align

CHANGING THE SIZE OF THE TEXT

We canged the h3 font size to x2 larger. The h2 fon size to a whopping almost x5 larger and added margin top
With the paragraph we made it a bit bigger and added some padding as well.

THE GALLERY

We’re making a section-c and but not using a container because we want it the gallery to go from end to end. Gallery is going to be our GRID container and then we’re going to have links with images. Using a link to our image, and a class BIG which is part of the simple lightbox and we have the location of the image.

Now we want to target each picture and modify the grid so that they all span across and take up room appropriately. We don’t need to give them all classes because we can use pseudo selectors like first child to assign them properties. We can do it this way or there’s a shorter way as well. This means that we’re assigning the picture to start from the edge and take up rows 1-3 and columns 1.3

**Link to work:** Check my GitHub @robertparkala, Twitter @thelunarcoder and Instagram @thelunarcoder ! Everything's active :)



#Day 9: November 5, 2020 



**Today's Progress**: Working on adding the lightbox feature and making the footer also adding media queries.

**Thoughts:** 

CREATING THE LIGHTBOX

Creating the lightbox turned out the be easier than expected. Instructions from the developer Andre we’re simple and structured. Added the dist folder wit the simple lightbox css and js files. Added a link to my markup regarding css and a script at the bottom regarding js. I’m so happy that it turned out looking great.

CREATING THE FOOTER

First we’re creating a section footer class with the footer tag. Then We’ll proceed to add a container DIV which will have grid items inside.

Now, we’re adding in two more grid items which will be Company info and Blog Post. Each will have a list, first one will have an unordered list and list items, second one will have just list items.

We’re adding another grid item with the heading of Subscribe and a paragraph. Now we’re entering a form with a name of email-form , method POST for it to work and an attribute of data-netlify and set that to TRUE and that’s how we can use their form submission system.
Now, we’re going to have a new div with a class of email-form in order to style the form and then a span with a class of form-control-wrap and in that span is where will have the input. We also added a button with a type of submit and a class and added an icon from font awesome.

We’re targeting the section footer and assigning it a background color from our custom properties and a text color of white. Also, some padding of 4 rem

Now moving on we’re targeting the container itself and setting the display to grid and grid template columns to 4 equal 1fr’s and a grid gap of 1rem.

Added attributes to the headings and also to the links. Went back and wrapped the Blog post list in <ul> tags so it would get rid of the bullet points.

Now, we’re targeting the section footer links that have the i tag in them. We used similar targeting in the previous project but I need to practice it more. 

The idea is to move the submit over to the right, we’re positioning it absolute withing the email form which is positioned relative. And we’re making the width and height 45px and we’re moving it to the top and right, so we’re moving it over as we can see compared to where it was first. 

Background color change, padding and margin 0 and we want the rounded corners on the right and bottom
 
ADDING MEDIA QUERIES 

Now we want to have the headphones come first so we need to target the first element which is the DIV in the section a with the text and put that in the second place and image in the first place. We can use pseudo selectors to achieve that.

Modified the footer to be in one column with 1fr and text in the center and also set display to none regarding the company name and blog post columns so it would look more minimal.

NETLIFY FORM

DEPLOYING TO NETLIFY

Pushed my project to GitHub and then deployed in Netlify.


**Link to work:** Check my GitHub @robertparkala, Twitter @thelunarcoder and Instagram @thelunarcoder ! Everything's active :)



#Day 10: November 6, 2020 



**Today's Progress**: Debugging the footer email form

**Thoughts:** 

I knew what I wanted to do today but I didn’t expect for it to be this difficult, let me explain. Although I finished the Audio-Phonic’s product landing page yesterday, I noticed that when I deployed it to Netlify and checked it out on my mobile (iOS) the email form wasn’t appearing in the footer column. 

It was already late yesterday evening and I set a goal for today, that instead of starting with a new project I’d spend a day, or however long it took to figure out what the issue is with the footer. So, around comes today and I’m excited to get going on the debugging and it just ain’t happening, I mean I’m new at coding, fresh, but from todays experience I can tell that it’s even more difficult to debug something than code. 

I knew where the problems was but to pinpoint it is another matter entirely. Did the fix work, yes, eventually and I got the form back on the mobile portrait layout as well. Is the bug fix working exactly like I want it to, no, not yet and I’ll continue working on that tomorrow. 

I want to understand how using .section-footer div:nth-child(2) and .section-footer div:nth-child(3) exactly makes my form disappear just on the Netlify platform, because I had it deployed on GitHub pages as well and its visible there. Am I content, no. 

Am I closer to being content, definitely but I just need to get the page working the way I want it to operate and then we’re good to proceed on to greener pastures.

**Link to work:** Check my GitHub @robertparkala, Twitter @thelunarcoder and Instagram @thelunarcoder ! Everything's active :)


#Day 11: November 7, 2020 



**Today's Progress**: Debugging the footer email form a bit further

**Thoughts:** 

Found the fix for the footer email form. I added a class to the form tag and styled in CSS with display flex and flex-direction column. It worked in placing the email form at the bottom of the footer in Netlify.

**Link to work:** Check my GitHub @robertparkala, Twitter @thelunarcoder and Instagram @thelunarcoder ! Everything's active :)



#Day 12: November 8, 2020 



**Today's Progress**: Started a new project, Satellite Web Development Grid page

**Thoughts:** 

INTRO

Making a responsive grid CSS website, CSS theme. Fundamentals of grid in a real project. One great resource is the Wes Bos’s course. Using CSS variables, rem units. Sections, fractional. Grid template areas using named template areas, SVG icons. Fractional columns. Fully responsive.

HTML and BASE

Copied Font Awesome with SVG with JS. Everything’s going to be wrapped inside of a wrapper. 

CREATING THE NAVBAR

CREATING THE TOP CONTAINER

Showcase and Top box A and B.

The header element represents a container for introductory content or a set of navigational links.
We’re doing a section with a class of top container and inside we’ll have a a header with a class of showcase. Showcase is going to have an h1 and a paragraph with lorem 15. Also an a tag with a class of btn which will be a custom button Read More, so we can make our links look like buttons.

Now, still withing the top container section we’re going to do the first top box, so it’s going to be a class of top-box and another class of top-box-a in the same div. Inside here, we’ll have an h4 and a paragraph and an a tag with a class of btn. We’ll have two of these divs and we’ll change the second one to top-box top-box-b. That’s it for the top container.

CREATING THE BOXES SECTION

We’re going to use a section tag with a class of boxes and each box will have a class of box. In each of these we’ll have an icon and we’re getting them from Font Awesome and adding fa-4x to make the icon bigger.
Under the icon we’ll have an H3 with analytics and then a paragraph with lorem 10. Now we need four of these boxes so we’re coping the whole box div and past it down. We’re changing up the icons, second one will be a globe icon with the heading Marketing, third one will be a cog icon with the heading Development and the last icon will be users with a heading of Support. Paragraph text stays the same at the moment.


CREATING THE INFO SECTION

We’re creating a class with section info section and inside well put our image. Image is going to be in the img folder. Underneath that we’ll have a div and inside the div we’ll have an h2 then a paragraph and then an a tag wit the class of btn for a button Learn More.




**Link to work:** Check my GitHub @robertparkala, Twitter @thelunarcoder and Instagram @thelunarcoder ! Everything's active :)



#Day 13: November 9, 2020 



**Today's Progress**: Creating the portfolio section and the footer. Also, creating CSS variables applying base styles to HTML, BODY and styling the navbar.

**Thoughts:** 

CREATING THE PORTFOLIO

We’re adding another section called portfolio and now what we can do is add random images from UNSPLASH with the unslplash.com/random URL and a specified size of 200x200 for example. Now that will give us all of the same pictures but if we want to get every photo to be different we just need to change one pixel for example 201, 202 etc. Now that won’t matter for the gird because the images are contained within the container – within their parents. Also, decided to not use random images, since I want my page to look more custom.

CREATING THE FOOTER

Now, we’re creating a simple footer and adding a footer tag that houses a paragraph and an ampersand copy to get us the copyright symbol.

BASE STYLING WITH CSS

CREATING CSS VARIABLES

Using CSS variables as in custom properties for our primary, dark, light and shadow color. Now, the rgba consists of 4 values first being red, second green, third blue and the last being alpha which is the opacity. We can use these throughout our CSS. 

BASE  STYLING HTML AND BODY

Box-sizing will be set to border box, that will make it so that if we use any padding or anything, it doesn’t affect the width of the element. Font family will be set to Arial, Helvetica, sans-serif and base color will come from the CSS variable of dark color.

Body will have a background of #ccc, that’s not going in the variable because that’s the only time we’re using this. We’re using a container for the wrapper, I want it to be full width but I do want to have a bit of margin on both sides. And the line height will be 1.4

BASE STYLING THE BUTTON

We’re using the btn class to style the button and using a background color of variable dark. Color refers to the text color so we’ll set that to light. With the padding we’re establishing 0.6em from top and bottom and 1.3rem from right and left. Text decoration will be set to 0 as that will remove our underline. Border will be 0 since we don’t want to add that. 

STYLING THE NAVBAR

We’re styling the main-nav and we want to style the ul. Display is set to grid like most things on this page. Grid gap is going to be 20px, padding to 0. By default UL’s have padding. We don’t want any bullets so we’re setting the list style to none. Grid template columns will be set to repeat 4, 1fr because we have 4 links.

We want to style each individual link so we’re going to capture the main nav a tag and setting the background to primary color. Display will be set to block and text decoration to none. We’ll set some padding and make text align to the center. Color of the text will be set to dark color and text-transform the letters to uppercase.
Font-size will be increased to 1.1 rem and we’re also creating the box shadow with the shadow color variable. 

We’re also setting the hover state with the dark color variable and the text will be light color variable.



**Link to work:** Check my GitHub @robertparkala, Twitter @thelunarcoder and Instagram @thelunarcoder ! Everything's active :)



#Day 14: November 10, 2020 



**Today's Progress**: Page is finished when it come to layout but I still need to add media queries. Today was a busy day with styling the top container area, making the grid layouts for both showcase, info sections and gallery. Footer now has social media links as well.

**Thoughts:** 

STYLING TOP CONTAINER

Displaying the top container with grid and a grid-gap of 20px. This is where we’re going to to our grid template areas. 
What the 

showcase showcase top box a
showcase showcase top box b means is that if we look at the yellow overlay, we see that we can format the grid template areas as our text is placed. Showcase taking up two columns and two rows. Top-box a and b are taking up one column each. 
Grid system is two dimensional unlike Flexbox which is just one dimensional. We can use grid template areas just as that, templates for our grid system and we can see how our grid is going to look in our CSS.


ADDING GRID AREA TO SHOWCASE

Now, we’re assigning the grid area to showcase because if we don’t do it, it doesn’t know what this means Showcase so we’re assigning it here. Also, we’re assigning the top box a and top box b matching grid areas so the grid would know where to place them. Now we just need to add separate styling to each grid.

We’re adding a background image one folder up in the img and showcase.jpg. Background size is set to cover. Cover means Resize the background image to cover the entire container, even if it has to stretch the image or cut a little bit off one of the edges. Also, background-position will be set to center.


STYLING SHOWCASE

One misconception is that if you’re using grid you can’t use flexbox at all. But we’re going to use flexbox for the showcase text. Grid is good for the site layout, boxes, areas, UI of the application and then flexbox to align things inside of those elements.

We’re setting the align items to flex-start and justify content to center. That will bring the text down and center. Also, we’re giving the container a box-shadow with our custom properties.

Showcase heading h1 will get a font-size of 4rem and a margin bottom of 0 to bring it closer to the paragraph.
Also a color of variable light so it would stand out.


STYLING TOP BOX

We’re styling the top-box separately, setting the display to grid, aligning and justifying items to the center and also applying a box shadow.


STYLING BOXES SECTION

For grid template columns we’re using repeat autofit with the minmax function that comes with the grid and inside there we’ll say we want a minimum on 200px, 1fr. If we now make the window smaller it will actually go on the next line. We don’t have to specify template columns for each media query for each size.


Additionally we’re styling the separate boxes which will a background of our var primary with text align to center, padding and box shadow.

STYLING INFO SECTION

The info section got a background color of var primary and we used grid template columns to repat 2 grids of equal 1fr since there’s two grid items.


STYLING PORTFOLIO

We are setting the display to grid and adding a grid gap. Doing the same with grid template columns as with the boxes section. Using autofit and minmax.




**Link to work:** Check my GitHub @robertparkala, Twitter @thelunarcoder and Instagram @thelunarcoder ! Everything's active :)



#Day 15: November 11, 2020 



**Today's Progress**: Finished off the page with medai queries and adding an additional information section.

**Thoughts:** 

MEDIA QUERIES

We’re modifying the grid template areas for 768px by saying that showcase is takin up two columns and top box and be are on another row and also taking up two columns.

Now, we’re modifying the navbar ul list and although it looks great it will look better all stacked in one columns again.

The grid template areas layout will be as follows with 
showcase
top box a 
top box b



**Link to work:** Check my GitHub @robertparkala, Twitter @thelunarcoder and Instagram @thelunarcoder ! Everything's active :)



#Day 16: November 12, 2020 



**Today's Progress**: Started working on updating my Space X tribute page that I submitted before to freeCodeCamp

**Thoughts:** 

Instead of taking on a new learning process with a unfamiliar project, I went back and started overhauling the tribute page that finished and submitted to freeCodeCamp. It has been bugging me a while now and I scrapped the whole page and started fresh. 

I knew it was going to be about Space X because the Dragon 2 Demo mission (watched the whole 32 hours of live feed!) was such an inspiration when it comes to human exploration, pushing beyond and taking on new challenges that I felt it resonated with how I felt and feel in my personal life as well. 

Hence taking on the journey of becoming a software developer! I tried to utilize what I have learned so far but also tried something new with Semantic UI that I have not done before.  

I started off with a wireframe of the page and how I wanted it to look. Inspiration for this comes from Space X's homepage.

In HTML I finished the navbar area and currently there’s just a big showcase photo right below it, also a the top section below the showcase. That wasn’t a lot for today but I feel like I spent a good amount of time just figuring out how I wanted the page to look. It’s starting to take shape and I feel like I have an idea how it’s going to turn out.

CSS is just starting to take shape as well and pretty much used the same techniques I have in previous projects. Also I want to incorporate an element into my page that comes from Semantic UI and thus I have to use a CDN but all it means is I’ll be using some css that’s pre-built. I’m not sure if this is ideal but I’d like to try it out and see how it feels. For example I haven’t touched Bootstrap or Tailwind at all yet learning and implementation wise and I know they make building stuff easier but I also want to learn to do it myself so that’s why I’m a little skeptical as to how Semantic’s going to look.


NAVBAR

Navbar has a logo on the left and added three menu items to the grid.

SHOWCASE PHOTO

Added a showcase photo and will create buttons later on so it will draw more attention to Reading More.
  



**Link to work:** Check my GitHub @robertparkala, Twitter @thelunarcoder and Instagram @thelunarcoder ! Everything's active :)



#Day 17: November 13, 2020 



**Today's Progress**: Continuing with revamping the Space X Tribute Page and added a quote section, timeline section and facilities.

**Thoughts:** 

I have a better idea of what I want to achieve with the Space X Tribute Page I’m revamping. It’s looking much different now than it did this morning and that’s a good thing. 

I’m trying to give it that Space X look while also being a bit different and let’s face it, their page is super high tech for me to go and replicate it one on one right now, so I’m trying my own version but incorporating certain images and elements they use. Also, I think the background colour needs to be black so that would really pull things together and maybe I’ll grab their logo instead of just writing it out. 

With HTML I added a quote section which gives the page a nice touch and as your scrolling you’re greeted with quotes from Elon and it’s hopefully a bit inspiring and makes visitors stop and read. But I already know that I’m going to structure and write it out different in CSS. 

Originally that quote structure comes from Semantic UI which is just easy to use but really it’s just bunch of h1 in a div with a display:block; so I’ll just write it out and use my own classes instead of theirs. The timeline section is a bit trickier and currently as it stands I’m using Semantic UI’s HTML with their pre-built CSS but I’ll see what I can come up with and probably will reverse engineer it as well so there’s the added bonus of a learning curve instead of just using their structures.


With CSS as I said for certain parts I planned on using Semantic UI’s pre-built style but I want to reverse engineer it so I would actually know how to build a timeline section like that. I mean, sure it’s just CSS but another thing is actually understanding how it works and what it creates. 

So, I’d like to do that and will probably spend a good few hours or a day just staring at the screen but I also enjoy that part so all is well. 



**Link to work:** Check my GitHub @robertparkala, Twitter @thelunarcoder and Instagram @thelunarcoder ! Everything's active :)



#Day 18: November 14, 2020 



**Today's Progress**: Added a new color palette to the body, timeline- and footer sections.

**Thoughts:** 

NAVBAR

Changed the navbr links color and hover color.

SHOWCASE

Added a button to the showcase photo.

TIMELINE

Modified the color palette of the whole timeline section.

FACILITIES

Updated facilities section with additional elements.

FOOTER

Modified the color of the footer section.



**Link to work:** Check my GitHub @robertparkala, Twitter @thelunarcoder and Instagram @thelunarcoder ! Everything's active :)



#Day 19: November 15, 2020 



**Today's Progress**: Finished the Space X Tribute Page revamp and moving on to an e-commerce project. 

**Thoughts:** 

I decided to change the layout of the page so that there's a facilities section in the end and then the footer otherwise on mobile the page would have been too long. I added some animations to the navbar, showcase button and also made everything responsive on web, tablet and mobile.



**Link to work:** Check my GitHub @robertparkala, Twitter @thelunarcoder and Instagram @thelunarcoder ! Everything's active :)



#Day 20: November 16, 2020 



**Today's Progress**: Started a new project and this one will be an e-commerce website called The South Face.

**Thoughts:** 

Complete e-commerce store which is fully responsive. Nav menu with Home, Products, About, Contacts and Account. Different products for Features and Exclusive Products, Testimonials and Popular brands section and a Footer area with four columns.

Products page featuring products, dropdown option for sorting and page numbers at the bottom of the products. Clicking on the product will lead to a product details page and we also have Related Products. Adding products to car will act as a full cart solution. The account page features a login and register form.

HTML and SETUP

Using border box and setting the margin and padding to 0 and this will be applicable for all of the HTML elements.

NAVBAR AND LOGO

We’re creating a navbar with UL and LI tags that feature our five inner pages.
Adding display flex because we want to work with flexbox and aligning items to the center with 20px padding for the navbar container.
We’re styling the nav tag contents now and assigning flex 1 so it would take up one space in the flexbox grid.
Now we want to style the navbar UL and LI items further 
We’re removing the text decoration and changing the color of the anchor a tags
Also, we’re setting the paragraph color the same as our anchor tags so if we write any content it will appear the same.
We added the whole navbar element to its separate container and styling that container with max-width so it will not go more than that, we’ll add margin so it will be in the center and some padding from left and right side.

SHOWCASE AND IMAGE

We’re adding a new with a class of row which will be our tagline for the homepage. See that by adding a line break with br we’re setting the two sentences apart although they are a part of the same h1.
Now we’re adding the paragraph and using the same line break to style our paragraph a bit better because some of the text would be so long in one row.
We will use the row class to display our items flex and align-items to the center.
Next up we have the img and we’re setting it to occupy 100% of the area and also padding so there’s a bit space from top and bottom and 0 from left and right. Next we’ll style the col-2 h1 and increase the font size and, line height to space things out and margin from top and bottom to give it some space. 



**Link to work:** Check my GitHub @robertparkala, Twitter @thelunarcoder and Instagram @thelunarcoder ! Everything's active :)



#Day 21: November 17, 2020 



**Today's Progress**: Finished the showcae area and created the featured category items

**Thoughts:** 

ADDING THE BUTTON
Created a button for the front page and styled to match the logo sow it draws attention.
HEADER BACKGROUND COLOR
Adding the background color to the header and will modify the image transparent sw we can change the background color.
FONT FAMILY
We we’re adding the font family to the body from Google Fonts.
We’re adding some more margin for the row class.
FEATURED CATEGORY
Creating a new div with the class name categories and we’ll add a class row which we have already created. And we are using col-3 for our three columns and adding our images which are all the same size.
We’re adding some margin 40px from top and bottom and 0 from left and right. With col-3 we are adding flex-basis 30% so that all of the columns would occupy 30% of the space. We’re adding min-width to the images to specify a minimum width. Width 100%
SMALL CONTAINER
Now we’re creating a small container and housing our images in there so we could style it further.
We’re setting the max-width and also setting the margin to center the elements. Padding is applied from the right and left.




**Link to work:** Check my GitHub @robertparkala, Twitter @thelunarcoder and Instagram @thelunarcoder ! Everything's active :)



Day 22: November 18, 2020 



**Today's Progress**: Finished the featured products section and added ratings and hover effect

**Thoughts:** 

FEATURED PRODUCTS
We’re adding the same small container to our Featured Products section and applying the row class that we already have styled in CSS.
Now, we’re styling the area similar to featured and with adding the flex basis 25% to the section because we want 4 images side by side and then specifying the width 100% on the image we’re fitting out products in nicely into the 25% area in their separate containers.
See how adding the width 100% takes up the 100% the width of the 25% container.
ADDING RATINGS
and now we’re adding the start icons using the font awesome’s icon links.
Now similarly to the first image, we’re adding rest of the 3 images.
We added a text-align on the title and formatted with margin, position set to relative and also added some line-height.
We used the ::after function to add a line after the featured products and that gives us a nice line after the Featured Products title with a width, height and border radius
Transform translateX helps us to place the line under our title.
We’re changing the font weight of the product titles and also added letter spacing to push everything onto two rows so the middle two photos would not drop down creating an uneven look.
Also, we’re decreasing the font size for the p tag which is the price.
Changed the rating icons color by adding a ratings class and then font awesome fas and far icon classes and styling them to be var third color.
Now, we want to add a hover effect to the pictures so were’ doing transition transform for 0,5s on all of the col-4’s and then adding a separate hover to col-4 a well. 



**Link to work:** Check my GitHub @robertparkala, Twitter @thelunarcoder and Instagram @thelunarcoder ! Everything's active :)



Day 23: November 19, 2020 



**Today's Progress**: Finished the You may also like section, added new arrival area and testimonials

**Thoughts:** 

YOU MAY ALSO LIKE SECTION
You may also like section was identical to the Featured products but the product names, reviws
NEW ARRIVAL SECTION
Also added a Buy Now button which is similarly styled as the 
TESTIMONIALS
I reused the small-container class and also row and col-3 to add in different content. Next, we’re adding in the quote icon, paragraph with the testimonial text, and then the ratings section. After that there’s an image and then a name with the h3.
Now we just populated the and made three extra reviews
We’re adding some padding to the top to space it out. Also, we’re moving the text to the middle and adding some more padding but now on the col-3 and with the col-3 image we are setting the width of the image to make it smaller, adding some padding and also adding a border radius to make the pictures rounded to look like modern testimonial pictures.
Now, we’re adding a box-shadow to the col-3 to raise the columns and create a 3d effect.
We’re increasing the font-size of the quotation marks and also the color.
With making the font-size smaller we’re also creating a more compact look. Adding some margin from top and bottom spaces out the text evenly. And a primary color makes the text stand out more.
Now, finally for this section we’re changing the font-weight and color and also the font-size.




**Link to work:** Check my GitHub @robertparkala, Twitter @thelunarcoder and Instagram @thelunarcoder ! Everything's active :)




