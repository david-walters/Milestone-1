# My Personal Portfolio Website - Milestone Project 1

This is a website that I created which is my first assignment on the Front-End Web Development course with The Learning People. The tasks of my assignment were the following;

>-	Create an online Portfolio for yourself with a minimum of 3 pages or (if using a 
>single scrolling page), at least 3 separate page areas.
>-	 Home,  About and Contact Me. 
>-	You may create an empty Portfolio page also for you to upload future projects. 
>
>Mandatory Requirements Static front end project: 
>
>Information Architecture:
>-	Incorporate a main navigation menu and structured layout (you might want to use Bootstrap to accomplish this). 
>-	Incorporate a footer at the bottom of each page.
>-	Maintain clear separation between code written by you and code from external sources using clear comments. Include the url of where you found the code (e.g. libraries or tutorials).
>-	Write a README.md file for your project that explains what the project does and the value that it provides to its users. Attribute any code from other sources. 

## Initional Steps I Took to Complete This Assignment

Having no prior experience of buiding a website, I took to the internet to find some portfolio examples that fitted the assignment criteria. 
Doing this gave me an insight of what I wanted for my portfolio and an understanding of how to begin.

I used some course materials to learn basic coding with HTML and CSS and a few Youtube videos on how to understand Bootstrap — as I felt Bootstrap was essential for me to build a responive website.

I kickstarted my website off with the home page.

### Home Page (index.html)

I wanted the home page to be very simple and welcoming — nice message for the user and a funny face for light-hearted humour. I wanted it to be the main page for navigation to my future portfolio and to get to the other pages that provide details about me and a way to contact me.

As the main thing about this page is to get the user to see my portfolio, I didn't want to just use a hyperlink text to direct the user to it. I felt it had to be a button and it had to stand out. So, using bootstrap, I used some of their custom classes to make a button which are `class="btn btn-danger btn-lg"`. This presented the hyperlink **View Portfolio** as a large red button.

For navigation to the **about.html** and **contact.html** I created a header with three navigation links (Home, About me, Contact) using the bootstrap classes and enabled them to float to the top right of the page. Using the class `navbar-expand-lg`, the nav links to collapse into the `<i class="fas fa-stream"></i>` icon and that would act as a button to be toggled to reveal or hide the nav links for when the screen size went smaller than large (1200px).

I initially felt that the nav links weren't too easy to notice, so I increased the font size, and to match the colour of the portfolio button and to start a bit of a colour theme, I pragrammed the nav links to change to a red colour when they are hovered over by the mouse.
The coding for my header navbar would be used for all the pages.

For a footer, I used the `page-footer` bootstrap class in a footer tag and made three navigation links and placed them at the bottom right of every page. Instead of text, I used icons from ***www.fontawesome.com*** which make a relatively clear sign as to where the links would take the user. The Github icon will navigate directly to this Github profile of mine, the Linkedin icon will navigate to my personal Linkedin profile, and an award icon, which is currently a null link, that I hope will be setup to navigate to my Coding Certificate that I should receive from The Learning People.

Just like the header navbar, the footer links also become red when the mouse hovers over them, and using the code `target="_blank"` on each icon, it will open up each page in a new tab.

### About Me Page (about.html)

This page is intended to show information regarding myself to any employers. So, it will basically act like a summerised CV.

I began with a photo of myself, a title for presentational purposes, and I formally displayed my name, age, and current location.

The page is then governed by three sections as the user scrolls down the page;

- Three titles acting like a cover letter
- History section showing qualifications, education, and work history
- Personal interests showing my hobbies and likes for additional information

Each section on this page was constructed using the following code;

```
        <div class="container">
          <div class="row text-center">
            <div class="col-md-4">
```

The class `container` will make the whole entire div have a working space of 12 columns. The class `col-md-4` will occupy 4 of those 12 columns, so it will take up one third of the container div. I did this three times which then displayed the three divs as three columns in a row. The `md` will nicely stack all three divs in one line when the screen width gets to 970px or less.

Despite having the same HTML coding for each section, they appear differently due to using different CSS techniques such as bordering the divs, box shadow, and using different colours and list styles. I also chose some interesting icons that I found on ***fontawesome***.

### Contact Page (contact.html)

This page is intended for employers to contact me via email whilst keeping my contact details undisclosed.

The user is able to put their first and last name, their email address for me to get back to them, and the message they want to send to me. All the information the user has provided will be sent to me via email after they have gone through a quick verification process to protect me from spam. This is all done using **formspree**.

Formspree acts like the middle man when sending emails. Once you have made an account on ***https://formspree.io/***, you will be given a code to put into your form tag which will allow you to receive emails without disclosing your email address. It also saves you from having to do any JavaScript as it is all done for you.

For the design and layout of the contact form, I followed a youtube tutorial linked here https://www.youtube.com/watch?v=FBAfpj91hps. This showed a step-by-step process on how to build this fancy contact form, though, I added my own touches with some different HTML and CSS.

I came to realise that this tutorial showed how to present a contact form but not how to make a practicle one that can actually be utilised. So, I found another Youtube video showing how to use **formspree** which entailed building a practical contact form, which is linked here https://www.youtube.com/watch?v=0X0kovjzLrw. I also researched what attributes should there be on a contact form and what to have for good practices.

I tested the contact form and sent myself some emails and it works perfectly.

## Interesting Issues During Developing

Of course, as anyone would, I had many issues that I came across when developing my website from having an additional space in the coding syntax (preventing the code from working) and to using git version control with the incorrect origin  (and left me wondering why it isn't being pushed).

Often I would have rendered my webpage and it will appear just how I wanted it, but when viewed from mobile view I would encounter many display issues with the design and text allignment. I had to constantly compromise to achiev best results in different screen sizes.

Due to the issues I had regarding Github, I wasn't able to regularily commit my work, but instead I continued to develop my website locally until I was ready to resolve the Github issues.

Once I managed to push all the files to Github, only the index file was being loaded when hosting the website. I realised that Visual Studio Code is not case sensitive with the file names and Github is, so it worked locally but not remotely. It was a matter of one capital letter in the file names that prevented the files from being found.

All the issues I encountered were a great experience as I learned many things from them.


## Technologies Used

- [**HTML5**](https://developer.mozilla.org/en-US/docs/Web/Guide/HTML/HTML5)
    - The project uses **HTML5** to create the basic elements and content of my website.
- [**CSS3**](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS3)
    - The project uses **CSS3** to add custom styles to the elements and content of my website.
- [**Bootstrap v4.3**](https://getbootstrap.com/)
    - The project uses **Bootstrap v4.3** to add a responsive grid system, prebuilt components, plugins built on jQuery, and Bootstrap styles to my website, before adding my custom styles.
- [**jQuery**](https://jquery.com)
    - The project uses **jQuery** to simplify DOM manipulation. This is the standard jQuery that is built with Bootstrap components.
- [**JavaScript**](https://www.javascript.com/)
    - The project uses **JavaScript** from Bootstrap which is required to add functionality to some of Bootstrap's components.
- [**Font Awesome**](https://fontawesome.com/)
    - The project uses **Font Awesome** for the social media links and the hamburger button on my website.
- [**Visual Studio Code**](https://code.visualstudio.com/)
    - I've used **Visual Studio Code** as the development environment to write the code for my website.
- [**Git**](https://git-scm.com/)
    - I've used **Git** as a version control system to regularly add and commit changes made to project in Cloud9, before pushing them to GitHub.
- [**GitHub**](https://github.com/)
    - I've used **GitHub** as a remote repository to push and store the committed changes to my project from Git. I've also used GitHub pages to deploy my website in a live environment.
- [**Chrome DevTools**](https://developer.chrome.com/docs/devtools/)
    - I've used **Chrome DevTools** to view my website from different screen sizes and to play around with the HTML and CSS before deciding what code to implement.

## Deployment

The hosting platform that I've used for my project is GitHub Pages. To deploy my website to GitHub pages, I used the following steps:

1. Opened the main directory in documents folder, right clicked, selected "git bash here."
2. Initialised Git using the `git init` command.
3. Added all files to the Staging area (Git) using the `git add .` command.
4. Committed the files to Git using the `git commit -m "First commit"` command.
5. Created a new repository in GitHub called 'Milestone-1'.
6. Copied the below code from GitHub into the terminal window:

    ```
    git remote add origin https://https://github.com/david-walters/Milestone-1.git
    
    git push -u origin main
    
    ```

7. Entered my GitHub username and password to push the files from Git to GitHub.
8. Went into 'Settings' on my repository page in GitHub.
9. Selected the 'main branch' option under the 'GitHub Pages' section.
10. Opened the provided link to my website in a new tab.



### Link to My Website

**https://david-walters.github.io/Milestone-1/**




## Personal Overview

From the beginning to end of this assignment, it has been a big journey for me. I started with no experience and I experienced so much in such little time. I came across many hurdles that I overcame through perserverance, problem solving, and research — all of it went in my favour.

I have so much more to learn, more experience to gain, and I can imagine that I will look back at this website one day and think "What on earth was I thinking" :joy:

It has been a great experience and I'm looking forward to working on my other project assignments that I shall be uploading to my portfolio for people to see.

:+1: Thanks for checking this out! :+1:
