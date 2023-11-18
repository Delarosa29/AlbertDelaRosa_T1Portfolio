# Albert Dela Rosa - T1A2 Portfolio 

## Overview
This website is a personal portfolio to demonstrate what we have learned in lessons regarding HTML & CSS. My goal is to have a presentable and functional website that showcases myself as well as applying the skills i have developed in basic web development.

## Components of Website

### Header and Navigation Bar

```HTML
    <header class="header">
        <a href="./index.html" class="homelogo">Albert Dela Rosa</a>
    
        <nav class="navbar">
            <ul>
                <a href="./index.html">Home</a>
                <a href="./sites/about.html">About</a>
                <a href="./sites/blog.html">Blog</a>
                <a href="./sites/contact.html">Contact</a>
            </ul>
        </nav>
    </header>
```
Created a simple responsive navigation bar using some flex that has 2 extra breakpoints which will change depending on the pixels on the width of the viewport. Originally used an image for the header text which displayed my name however i had issues getting it to fit nicely when wrapping with nav bar items. Each nav element has a pseudo element which changes color when cursor is hovered over.

### Footer and Socials

```HTML
    <footer>
        <p>Connect with me!</p>
        <div class="socials">
            <a href="https://github.com" target="_blank">
                <i class="fa-brands fa-github fa-2x" style="color: #ffffff;"></i>
            </a>
            <a href="https://au.linkedin.com" target="_blank">
                <i class="fa-brands fa-linkedin fa-2x" style="color: #ffffff;"></i>
            </a>
            <a href="https://www.instagram.com" target="_blank">
                <i class="fa-brands fa-instagram fa-2x" style="color: #ffffff;"></i>
            </a>
        </div>
    </footer>
```

Footer contains 3 social links that redirect to a new page when icons are clicked. Used flexbox but didn't need as much breakpoints as there aren't many elements. Icons are linked to website in the form of fonts and given anchor tags for links.

### Landing Page
```HTML
    <main>
        <div class="wrap">
            <img src="./components/images/Screenshot 2023-11-18 161539.png" alt="me image">
            <div class="text">
                <h2>Hi!</h2>
                <p>My name is Albert! I'm an aspiring junior developer who's taken my first steps into the world of
                    programming. Here on my website hopefully i can display some of what i've learnt and what type of
                    new skills I'm planning to learn! Have a look around.</p>
            </div>
        </div>
    </main>
```
The home page contains a small introduction for me and the website along with a photo (only recent one i have). Flexbox was once again used for the layout to keep things simple and has 3 breakpoints which change it into a column style layout as the device width reduces.

### About Me Page
```HTML
    <main>
        <h1 class="title">About Me!</h1>

        <div class="columns">
        <div>
            <h2>Personal</h2>
            <p>I'm an excited newcomer to the programming background that was heavily influenced by those around me from my father to my friends who have IT backgrounds. Growing up and playing with technology it was only right to pursue something related! </p>
          </div>
          <div>
            <h2>Dev Skills</h2>
            <ul class="language-list">
                <h3>Web Development</h3>
                <li>HTML</li>
                <li>CSS</li>
                <h3>Programming Languages</h3>
                <li>Python</li>
                <li>Javascript</li>
                <li>Java</li>
                <li>C#</li>
            </ul>
          </div>
          <div>
            <h3>Things that i enjoy</h3>
            <ul class="interest-list">
                <li>Games (FPS, Sim Racing)</li>
                <li>Basketball</li>
                <li>Powerlifting</li>
                <li>Anime</li>
            </ul>
          </div>
        </div>
    </main>
```
The about me includes more info about myself and the skills that i'm currently learning on the path to become a programmer. It also lists hobbies.