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
Created a simple responsive navigation bar using flex. Originally used an image for the header text which displayed my name however issues arose getting it to fit nicely when wrapping with nav bar items. Each nav element has a pseudo element which changes color when cursor is hovered over.

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

Footer contains 3 anchors in forms of icons which are styles from external website. Icons enlarge when cursor hovers.

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
The home page contains a small introduction for me and the website along with a photo. Flexbox was once again used for the layout to keep things simple and has 3 breakpoints which change it into a column style layout as the device width reduces.

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

### Blog Landing Page
```HTML
    <main>
        <div class="blog">
            <div class="blog-content">
                <!-- a href has an added # at the end of directory to auto jump to element that i have given an id to in the related blog post -->
                <a href="./blogs/blogspage.html#workplace">
                    <img src="../components/images/kari-shea-1SAnrIxw5OY-unsplash.jpg">
                    <h3>Worksplace Studies</h3>
                    <p>14/08/2020</p>
                </a>
            </div>
            <div class="blog-content">
                <a href="./blogs/blogspage.html#global">
                    <img src="../components/images/nasa-Q1p7bh3SHj8-unsplash.jpg">
                    <h3>Global Network</h3>
                </a>
                <p>29/06/2011</p>
            </div>
            <div class="blog-content">
                <a href="./blogs/blogspage.html#tips">
                    <img src="../components/images/lauren-mancke-aOC7TSLb1o8-unsplash.jpg">
                    <h3>Tips for Productivity</h3>
                    <p>1/12/2015</p>
                </a>
            </div>
            <div class="blog-content">
                <a href="./blogs/blogspage.html#technology">
                    <img src="../components/images/sean-pollock-PhYq704ffdA-unsplash.jpg">
                    <h3>Technology Today</h3>
                    <p>19/11/2023</p>
                </a>
            </div>
            <div class="blog-content">
                <a href="./blogs/blogspage.html#trends">
                    <img src="../components/images/scott-graham-5fNmWej4tAA-unsplash.jpg">
                    <h3>Technology Trends</h3>
                    <p>5/25/2020</p>
                </a>
            </div>
            <div class="blog-content">
                <a href="./blogs/blogspage.html#programming">
                    <img src="../components/images/joan-gamell-ZS67i1HLllo-unsplash.jpg">
                    <h3>Modern Programming</h3>
                    <p>24/3/2022</p>
                </a>
            </div>
        </div>
    </main>
```
Added a simple blog landing page which showcases 6 blog posts with an image, title and date published. Used flex to have it evenly display at multiple pixels. Added a #id tag to href locations to automatically jump to location of corresponding blog post in separate page. Blog posts enlarge when cursor hovers over.

### Blog Page
```HTML
            <h2 class="maintitle">Blog Page!</h2>
        </span>
        <!-- Article semantic -->
        <article class="grid-container">
            <!-- Figure semantic -->
            <figure class="image">
                <img src="../../components/images/kari-shea-1SAnrIxw5OY-unsplash.jpg" alt="Image 1">
            </figure>
            <div class="text">
                <div id="workplace">
                    <h2>Workplace Studies</h2>
                    <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit. At, dolorum, facere iste, facilis
                        aspernatur velit dolores libero vel eligendi labore ipsum ullam fugiat nostrum a? Necessitatibus
                        mollitia veniam expedita similique. Lorem ipsum dolor sit, amet consectetur adipisicing elit.
                        Eligendi nemo repellat cupiditate voluptates obcaecati nesciunt saepe tempora quos consectetur
                        earum, numquam non ipsam itaque quo, eaque dolor maiores ipsa placeat!</p>
                </div>
            </div>
        </article>
```
Blog list page includes all blog posts and texts using CSS Grid layout. Used only 1 HTML page to contain all blog posts rather than opening a different link for each individual blog post.