# Horiseon Website SEO And Accessibility Optimization

## About Horiseon

Horiseon is a marketing agency that offers Search Engine Optimization, Online Reputation Management, and Social Media Marketing solutions to businesses. Their website, updated to 2019, shows several issues that we will analyze in detail in the following section. You can visit the Horiseon website by clicking [HERE](https://nikola84ca.github.io/Horiseon-SEO-Project/).

## Website description

The website is a single page that consists of these elements, listed from top to bottom.

* An Header were we find the company name/logo and includes three links pointing to specific sections of the page.
* A big background image that is indicative to the company sector
* A main article that occupies the 75% of the screen, divided in a big article consisting of three sections describing the company services, each one accessible through the relative links in the header.
* A side column that occupies the 20% of the screen on the right of the main article that describes the benefits of working with Horiseon.
* A footer with the copyright, now updated to 2023.

Here is an example of the functionality implemented in the header links; when clicked they direct the user to the relative section of the main article.

![Gif animation of the header links, when clicked they will redirect the user to the relative section of the main article](/assets/readme-assets/Horiseon-Website-links-gif.gif).


## What is this project about?

This project is meant to improve SEO and Accessibility of Horiseon Website, in order to make the company website rank better on search engines and offer a more inclusive experience for all users, especially those with disabilities who require assistive technologies such as video captions, screen readers, and braille keyboards. This is a fundamental improvement that will allow not only a better SEO but also will avoid litigation that can occur when these cannot access their website due to accessibility issues. As a marketing agency, it is fundamental that their website reflects the services they provide, in order to make their website not only rank high on search engines but also make the website accessible to all users. Accessibility, together with a semantic HTML structure are some of the pillars of SEO, and in this project, we are going to improve those elements to make sure Horiseon's website complies with modern standards.

## My Process

* The first thing I did was looking for all the non-semantic elements, unnecessary and/or generic divs and create a more organized, clear and logical structure of the HTML code. This image shows an example of the original HTML code.

![Screenshot of the original code with non-semantic elements](/assets/readme-assets/original-code-divs.JPG).

*I replaced it with semantic HTML elements, assigning to each part of the code it's logical tag. From the image above we can see that the header was set as a class named header, styled with CSS in the relative class in the CSS file. Also, all the element were inside generic div tags; search engines do not love this way of coding, so I assigned the correct semantic elements to each portion of the HTML code. The class header become an element, and I replaced it in the CSS too, (same thing happened for the footer). Here is the edited code, where I also replaced the link's div with a more logical nav tag to contain them.*


```HTML
<header> <!-- Replaced the div with an header, removed the class .header and fixed the relative CSS -->
        <h1>Hori<span class="seo">seo</span>n</h1>
        <nav>  <!-- This is the navigation part of the header, I replaced the generic dev with a nav -->
            <ul>
                <li> 
                    <a href="#search-engine-optimization">Search Engine Optimization</a> 
                    <!-- Added the id for search-engine-optimization and now point to the
                     relative section in the main content article -->
                </li>
                <li>
                    <a href="#online-reputation-management">Online Reputation Management</a>
                </li>
                <li>
                    <a href="#social-media-marketing">Social Media Marketing</a>
                </li>
            </ul>
        </nav>
    </header>
```    

* Following the same example, I decided to restructure the main body of the website dividing the main article into sections, linked to the links in the nav of the header. I did the same for the column on the right, assigning an aside tag to that portion of the page. Here is what the non-semantic HTML code of the main content looked like before:

![Screenshot of the original code with non-semantic elements in the main content article](/assets/readme-assets/original-code-main-content.JPG).

*Here is what I decided to implement. The main article is now divided into three sections. While I was working on this, I noticed that thes first section, the search engine optimization, wasn't responding to the link in the header because, as shown in the picture above, the section didn't include the relative id search-engine-optimization. I included it and not the navigation in the header is fully working*

```HTML
<main>
        <figure class="hero" title="Team Working"></figure> 
        <article class="content">
                <section id="search-engine-optimization" class="search-engine-optimization">
                <img src="./assets/images/search-engine-optimization.jpg" alt="immage of search engine optimization" class="float-left" />
                <h2>Search Engine Optimization</h2>
                        <p>
                          The dominance of mobile internet use etc...
                        </p>
            </section>
            <section id="online-reputation-management" class="online-reputation-management">
                <img src="./assets/images/online-reputation-management.jpg" alt="immage of reputation management" class="float-right" />
                <h2>Online Reputation Management</h2>
                     <p>
                         The web is full of opinions etc...
                    </p>
            </section>
            <section id="social-media-marketing" class="social-media-marketing">
                <img src="./assets/images/social-media-marketing.jpg" alt="immage of social media marketing" class="float-left" />
                <h2>Social Media Marketing</h2>
                    <p>
                        Social media continues to have a sizable etc...
                    </p>
            </section>
        </article>
```

* I made sure that all images and icons had a proper alt text to be show in case of an image broken link or for those users who require assistive technologies such as video captions, screen readers. The following image shows the original non-semantic code where the images and icons had no alternative text.

![Screenshot of the original code with non-semantic elements in the main content article](/assets/readme-assets/original-code-img-no-alt.JPG).

*I included a relative text description for each picture and icon implementing for each img it's relative alt tag as shown in the new HTML code below*

```HTML     <section id="search-engine-optimization" class="search-engine-optimization">
                <img src="./assets/images/search-engine-optimization.jpg" alt="immage of search engine optimization" class="float-left" />
                <h2>Search Engine Optimization</h2>
```




## Upcoming Improvements

Although the website is optimized for desktop view, it is still not responsive for tablet and mobile usage. The next steps to offer a more accessible and performant user experience is to work on the CSS of the website in order to make the website responsive and easy to navigate on all other devices as well. Other important additions could be implemented with detailed JavaScript code to make the website more functional and interactive for users.

## Collaborations and Contributions

I welcome all the brilliant coders out there to join me in this project. Join effort can result in a fundamental learning experience for a beginner coder like me, so feel free to reach out with tips and advice. If you want to contribute to this project, pull requests are welcome, but if you want to make major changes, please open an issue first so that we can discuss what you would like to change. You can contact me on my GitHub profile [HERE](https://github.com/Nikola84ca) and visit this project repository, Horiseon-SEO-Project, by clicking [HERE](https://github.com/Nikola84ca/Horiseon-SEO-Project).

## License

[MIT](https://choosealicense.com/licenses/mit/)
