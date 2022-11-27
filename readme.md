# Egg Champion Website Readme File

[View the live project here] (https://lithill.github.io/New-Egg-Champion-Website/)

This website has been created for a fictional sport called Egg Champion. It gives up to date news on which egg is the current champion, history of the sport, a shop where fans can buy merchandise, and a quiz about eggs. It was been designed with a range of different screen sizes in mind. 

## Technologies Used

### Languages Used

- HTML5
- CSS3

### Frameworks, Libraries & Programs Used

- [Google Fonts] (https://fonts.google.com/) was used to import IM Fell Double Pica, Trirong, and League Gothic.
- [Font Awesome] (https://fontawesome.com/) was used on the footer for the social media icons.
- [Replit] (replit.com) was used as the main programm to write the code, which was then sent to GitHub for version control.
- [GitHub] (https://github.com/) was used to store the project's code after being pushed from Replit.
- [Paint.Net] (https://www.getpaint.net/download.html) was used to create the logos on each corner of the header.
- [InVideo] (https://invideo.io/) was used to create the video on the index page. 
- [YouTube] (https://www.youtube.com/) was used to host the video.
- [Zazzle] (https://www.zazzle.co.uk/) was used to create functioning merchandise links.

## Credits

### Code

- The table border code on the Quiz page came from [this Stack Overflow post] (https://stackoverflow.com/questions/3313456/css-borders-between-table-columns-only)
- I found code to help text wrap around an image on this [ThoughtCo article] (https://www.thoughtco.com/wrapping-text-around-image-3466530#:~:text=Enter%20.,the%20text%20wraps%20around%20it). I have lightly edited it.
- I borrowed some blockquote stying code from [CSS Tricks - blockquote styling] (https://css-tricks.com/snippets/css/simple-and-nice-blockquote-styling/), [Java2s] (http://www.java2s.com/Code/HTMLCSS/Tags/borderforblockquote.htm) and [CSS Tricks - html quotations] (https://css-tricks.com/quoting-in-html-quotations-citations-and-blockquotes/)
- To create columns for the Zazzle products, I used code from [W3Schools] (https://www.w3schools.com/howto/howto_css_three_columns.asp)
- Embed code from [Zazzle] (https://zazzle.co.uk) and [YouTube] (https://www.youtube.com/)

### Content

- All content was written by the developer

### Media

- The two Egg Champion logos in the menu bar were created by the developer, using Paint.net.
- The egg timer photograph used on the history page was taken and edited by Jordan Benton, and found on [Pexels] (https://www.pexels.com/photo/shallow-focus-photography-of-hourglass-1095602/). 
- The egg crack overlay used on the News page was created by b0red, and found on [Pixabay] (href="https://pixabay.com/vectors/crack-distress-effect-chip-distress-2249743/)
- The image for the News page background was created by Edward Jenner, and found on [Pexels] (https://www.pexels.com/photo/multiple-overlay-patterns-of-monochrome-design-4252890/)
- Replacement merchandise pictures were generated through [Spreadshirt] (www.spreadshirt.co.uk).
- [Dall-E 2] (https://openai.com/dall-e-2/) was used to create the rest of the artwork.
- The video was made by the developer, using [InVideo] (https://invideo.io/).

### Acknowledgements

- My tutor Robert Mclaughlin for helpful feedback.

## Testing

The [W3C Markup Validator] (https://validator.w3.org/) and [W3C CSS Validator Services] (https://jigsaw.w3.org/css-validator/) were used to validate every page of the project to ensure there were no syntax errors in the project.

- This website was tested on Google Chrome - add others browsers when you get to that stage
- This website was viewed on a variety of devices such as Desktop, laptop, iPhone SE - add other devices
- A large amount of testing was done to make sure the pages were correctly linked
- Friends, colleagues and classmates were asked to review the site and documentation to point out any bugs or user experience issues

## Known Bugs

## Deployment

### GitHub Pages

This project was deployed to GitHub Pages using the following steps:

1. Log into GitHub and locate the [GitHub Repository] (https://github.com/Lithill/New-Egg-Champion-Website)
2. Click the settings button (above the "add file" button)
3. Click on "Pages" on the left-hand-side column
4. Under "Source", click the dropdown called "Main", select folder ""/root" and click "save".
5. Refresh the page
6. Click on the "Visit site" button at the top of the page

### How to fork the repository

### How to clone the repository

## Difficulties I came across

1) Egg Champion left logo wouldn't change size through pixel width in css. So I put the ID in the <img> rather than <a>. I'm not sure why that worked.

2) I couldn't turn nav bar with 

nav {
	background-color: #000000
}

so tried this which didn't work

header {
	background-color: #000000
}

Then tried 

#header {
	background: #000000
}

Added width etc and it worked

3) Left logo is overspilling header. Tried overflow: hidden, and z-index but didn't work.

#left-logo {
	height: auto;
	width: 250px;
	float: left;
	z-index: 1;
	overflow: hidden;
}

Tried also giving header z-index 2, didn't work.

Then thought maybe it's because of the relationship between the header and the image, so I set left-logo image height to 100% and that worked. But then the rest of the nav words are out of line, so changed line-height.

4) changing line height of nav bar words made them out of line depending on width of screen. Don't know why. So used -

#menu, #left-logo {
/* 	line-height: 70px; */
	vertical-align: middle;
}

This still didn't align it. Figured it might be because the left logo is too big. So made it smaller. But changing left logo height didn't help.

5) Right-egg logo. Couldn't turn the header into position: relative;, because that messed it up. So I figured I needed something else to make the position relative. But couldn't figure it out, so I went back to what I did a while ago, although I can't remember how I got there.

6) nav bar looks rubbish on mobile. Words aren't verticaly centered. Tried display: flex;, didn't work. Tried a few other things but didn't work so gave up for now. 

7) For first big egg in index, looked at [Bit Degree] (https://www.bitdegree.org/learn/responsive-image#setting-background-size-to-fit-screen) and love running. It didn't show up without setting both height and width (auto height made it disapear again). so crossing my fingers this will do for now.

8) Used animation for big eggs - took code from love running

9) Had to change header height to pixels rather than % so that I could top-margin the 1st big egg without any gaps. But this messed up the text, so changed line-height: 60px; in #menu

10) Need a big-egg-1-outer so that the bottom line doesn't move on zoom effect. Plus overflow: hidden; & position: relative;

11) when I added a second big egg, I couldn't figure out how to stop the zoom spilling into second egg. So turned off zoom. 

12) Can't seem to center big egg text 3. Tried text-align, and margin-left & right auto. Didn't work. Used right: 38%; instead.

13) The index page needed a payoff so I made a video. Difficulty getting video to show. This website helped - [Free Code Camp] (https://forum.freecodecamp.org/t/youtube-refused-to-connect/245262). Then had difficulties with sizing, and used this as I wanted it full screen - [Stack Overflow] (https://stackoverflow.com/questions/24157940/iframe-height-auto-css). But it was too big and text got missed out when you played it. Nothing I tried worked out, so I made a div to fit the video to. Ended up doing this, but it isn't responsive:

 .container {
	 background-color: blue;
    width: 100vi;
    height: 655px;
 }

 .video {
	 height: 100%;
	 width: 100%;
 }

I wanted it to look less like a youtube video so used info here - [Freshy Sites] (https://freshysites.com/web-design-development/how-to-use-youtube-parameters-and-recent-changes/). And changed code to src="https://www.youtube.com/embed/-kl4j_AEC5k?rel=0&amp;controls=0" class="video".

14) used love running footer as basic for my footer. Having trouble with white space under footer. I read this - [Stack Overflow] (https://stackoverflow.com/questions/54836610/why-is-the-background-color-of-my-footer-not-filling-my-entire-footer) and changed my background colour. But now when i put height to 60px, the border rides up. Degbugged in chrome, it looks like it is something to do with the class "social-networks" it is overspilling the footer, but when i add this to the class - height: 60px;, doesn't change anything. Then debugged and figured out it was the margin on the social network class.

15) Wanted the page you are on to be yellow. But the 'active' class was being overidden by "menu a" text colour. Making it an id didn't work. So I took the text color out of "menu a" and created a "not-active" class where the text is white, and applied that to all other header links. 

16) Next trying to make h1 in index responsive. Thought there should be a way to make text position in relation to the div rather than the edges of the screen. But taking away the "top" property from "big-egg-1-text" and replacing it with "vertical-align: middle;" didn't work. Couldn't figure it out.

17) Mobile fix for header - created a new link image in the header and turned off display when not in mobile view. Decided to make big egg text not layer on div above under a certain screen width for ease of responsiveness.

18) When wrapped the img in history page, the caption didn't go with it. So applied class="img-right-wrap" to figure rather than img. But this made the image lose its padding and width sizing. So tried to seperate them into 2 different classes to apply to figure and caption, or img and caption, but couldn't figure it out, so got rid of caption.

19) Searching for html for quotes in articles. Found this [CSS Tricks, quoting in html] (https://css-tricks.com/quoting-in-html-quotations-citations-and-blockquotes/). and [CSS Tricks, blockquote styling] (https://css-tricks.com/snippets/css/simple-and-nice-blockquote-styling/). Wanted to add extra padding, so edited that bit of code too. Realised I needed unequal columns to make the photos sit better with the same amount of padding between them. Then turned my attention to the zazzle photos that are too blurry. 

20) I just learnt about boostrap and tried to utilise it for my columns on the shop page, but it messed up a lot of my current css, even when put it before my css link in the head. So I tried instead to take individual css code from bootstrap. I used [Stack Overflow] (https://stackoverflow.com/questions/44387827/where-to-find-bootstrap-classes-css-definitons) and the [Bootstrap source code] (https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/css/bootstrap.css) to try to do this, but I could not get it to work.

21) Wanted Egg titles to fill the screen. After testing on a larger screen it looked messy. So I changed the code to 100vh instead of width 100%. This had a known-on effect, so I decided to redo the images - making them consistent in size and dead space. I then changed the css to tidy up after the changes. Resonspiveness will need tidying up too later. 

22) I broke the website and wasn't sure why. So reset it back to a few commits behind. Noticed that #big-egg-outer in css should be a class, but if I change it to a class, I lose a lot of my text from index.html. This needs looking at. Also, noticed that if I locally host all my images, filepaths no longer work on git pages when linked from html pages. Only work when linked from the css page. Not sure why currently. Lost most of the uploaded images when reverting back to previou commit, as replit had a bug and wouldn't let me revert to the most recent commit.

23) Fixed positioning for index page. I found code on [Stack Overflow] (https://stackoverflow.com/questions/45641440/vertically-center-content-in-a-vh-height-div) which helped me to vertically centre the text in the div. Although I'm not entirely sure why this works. I realised the last text section didn't look centered because the image it was below wasn't centered. I also switched the Flikr hosting to local hosting for these images. 

24) The previous fixes changed how the @media code worked, so I re-wrote it. The shop page seems to be strangely indenting to the left in mobile view. 

25) The video didn't behave as expected in mobile view. It did not become full screen when the phone was rotated, so I found the code on [YouTube] (https://support.google.com/youtube/answer/171780?hl=en)

26) Found out how to create text-shadow via css at [MDN Web Docs] (https://developer.mozilla.org/en-US/docs/Web/CSS/text-shadow).
    
27) The video on the home page was too big for the container in tablet and mobile view. This resulted in a side scroll appearing at narrower screen widths. I used chrome developer tools to confirm that the video was the culprit. I pasted fresh embed code from YouTube, and then used code from [w3schools] (https://www.w3schools.com/howto/howto_css_responsive_iframes.asp) to make the video responsive. This removed the side-scroll. I then wanted to make the video smaller, but noticed that when I did, it was no longer centered. I fixed it by using code I found from [Stack Overflow] (https://stackoverflow.com/questions/8366957/how-to-center-an-iframe-horizontally)
    
28) Improved legibility of news page fight information, as users found the images confusing. I used the following sources to help with this code: [Stack Overflow for outlining] (https://stackoverflow.com/questions/4772906/css-is-it-possible-to-add-a-black-outline-around-each-character-in-text), [w3schools for centering text over an image] (o	https://www.w3schools.com/howto/howto_css_image_text.asp), and [CodePen] (https://codepen.io/gylidian/pen/zyabWX) for slanting text.
    
29) The images from the Zazzle embed code were blurry. I tried to get better images from the Zazzle website, but could not. Instead, I used [Spreadshirt] (https://www.spreadshirt.co.uk/create-your-own) to create mockup images of merchandise to replace the zazzle images on the Shop page.

30) There was too much space between title images and text in longer mobile views, which was difficult to lessen when the image was a background. So I starte on the history page, and switched the background-image to an img when the screen hit a lower width. I later decided this made the code unnecessarily complex, and made the title image imgs instead of background-images. Will refine this before changing all pages to this solution.
    
31) When testing on my iPhone SE, I noticed this new method made the title image and text spill under navigation bars. So I changed title image and text sizes to fit. 
    
33) When testing all mobile sizes in chrome developer tools, I noticed that the title image becomes distorted in 912px x 1368px - Surface Pro 7. So I changed the mobile media query to start at 912px instead.
    
34) When testing all mobile sizes in chrome developer tools, I noticed that the history link is pushed off the navigation bar in the Galaxy Fold view. So I made the link text slightly smaller in mobile view.
    
35) Added customisation for quiz radio buttons with code from [Useful Angle] (https://usefulangle.com/post/389/css-radio-button-color).
 
