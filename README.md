# My Personal Portfolio Website - Milestone Project 1

This is a website that I created which is my first assignment on the Front-End Web Development course with The Learning People. The tasks of my assignment were the following;

-	Create an online Portfolio for yourself with a minimum of 3 pages or (if using a 
single scrolling page), at least 3 separate page areas.
-	 Home,  About and Contact Me. 
-	You may create an empty Portfolio page also for you to upload future projects. 

Mandatory Requirements Static front end project: 

Information Architecture:
-	Incorporate a main navigation menu and structured layout (you might want to use Bootstrap to accomplish this). 
-	Incorporate a footer at the bottom of each page.
-	Maintain clear separation between code written by you and code from external sources using clear comments. Include the url of where you found the code (e.g. libraries or tutorials). 
Documentation: 
-	Write a README.md file for your project that explains what the project does and the value that it provides to its users. Attribute any code from other sources. 

## Initional Steps I Took to Complete This Assignment

Having no prior experience of buiding a website, I took to the internet to find some portfolio examples that fitted the assignment criteria. 
I eventually came accross a simple one but I wasnt't too happy with the user experience that I received from it. Doing this gave men the insight of what I wanted for my portfolio and an understanding of how to begin.

I used some course materials to learn basic coding with HTML and CSS and a few Youtube videos on how to understand Bootstrap — as I felt Bootstrap was essential for me to build a responive website.

I kickstarted my website off with the home page.

### Home Page (index.html)

I wanted the home page to be very simple and welcoming — nice message for the user and a funny face for light-hearted humour. I wanted it to be the main page for navigation to my future portfolio and to get to the other pages that provide details about me and a way to contact me.

As the main thing about this page is to get the user to see my portfolio, I didn't want to just use a hyperlink text to direct the user to it. I felt it had to be a button and it had to stand out. So, using bootstrap, I used some of their custom classes to make a button which are `class="btn btn-danger btn-lg"`. This presented the hyperlink **View Portfolio** as a large red button.

For navigation to the **about.html** and **contact.html** I created a header with three navigation links (Home, About me, Contact) using the bootstrap classes and enabled them to float to the top right of the page. Using the class `navbar-expand-lg`, the nav links to collapse into the `<i class="fas fa-stream"></i>` icon and that would act as a button to be toggled to reveal or hide the nav links for when the screen size went smaller than large (1200px).

I initially felt that the nav links weren't too easy to notice, so I increased the font size, and to match the colour of the portfolio button and to start a bit of a colour theme, I pragrammed the nav links to change to a red colour when they are hovered over by the mouse.
The coding for my header navbar would be used for all the pages.

For a footer, I used the `page-footer` bootstrap class in a footer tag and made three navigation links and placed them at the bottom right of every page. Instead of text, I used icons from **fontawesome.com** which make a relatively clear sign as to where the links would take the user. The Github icon will navigate directly to this Github profile of mine, the Linkedin icon will navigate to my personal Linkedin profile, and an award icon, which is currently a null link, that I hope will be setup to navigate to my Coding Certificate that I should receive from The Learning People.

Just like the header navbar, the footer links also become red when the mouse hovers over them, and using `target="_blank"` on each icon, it will open up each page in a new tab.

### About Me Page (about.html)