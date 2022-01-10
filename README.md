<strong> NATURAL HEALTH BLOG </strong>


I created a Natural Health Blog focusing on Responsive design also using a small amount of JavaScript for my nav bar.

Whilst building projects I noticed the importance of building a responsive web page which is mobile friendly as well. I started building my project before I applied responsiveness , and realised when I changed my width to a smaller size, my content was all jumbled up. So I started fresh so I can learn from the beginning of making my web page how to build a responsive web page. I watched this tutorial that helped me a lot and would be using this method for future use as it is clearly structured.

In the tutorial he use the class .active on one of the properties. Having not knowing the use of .active I searched and found a blog which explained that .active is usually used in correlation which <a> or <button> as it is active when a user clicks on it- stands for active link. (see link below)
https://www.youtube.com/watch?v=At4B7A4GOPg


This futured my search flex/flex box and how to use the property properly.
  ![image](https://user-images.githubusercontent.com/92884422/148755609-34fac4c2-4f05-47b9-ba87-4ea1f9c905c9.png)
  
  I liked this explanation as it shows clearly the affect of responsive web design when flexed is used and how to implement it properly with @media queries.
  
  <strong> Using @media to fix over lapping </strong>
  
  My problem was that my <strong> h4 </strong> was overlapping onto the other screen and outside of its container when I reduced the width to a phone screen size. My main goal for this project was to make it responsive so I went ahead and used media quieries to solve this.
  
  I soon realised that it is better to finish your web page on the screen that you are using and <strong>then</strong> apply the @media quuries after all your main styling is done. 
  
  'On a side note. If you are using @media queries (such as @media screen (max-width:500px)) pay particular attention to applying @media query AFTER you are done with normal styles. Because @media query will be crossed out (even though it is more specific) if followed by css that manipulates the same elements.'
  <https://stackoverflow.com/questions/3047056/what-do-the-crossed-style-properties-in-google-chrome-devtools-mean>.
   

	 CSS Responsive Cards 
 <p>   As I was creating a blog I wanted my contents to be in a card layout form. I used this tutorial (see below) to help me make the cards be responsive. In researching I found that:
    When you are creating cards make them all with the same class as they are going to have the same layout and general style. Within the <div class="card" > This also refreshed my memory on how important parent and child containers are in CSS. </p>


You want to make a separate div with the class of "card -image" and then CLOSE the div right after as it is its own section as the only tging that would go inside the div is the image. After that put your heading and < p > text and then close the overall parent container.

Currently the card are placed in a single column since they are divs and take up their own line,  but we want them to be side by side so we have to make the container to be flex! <div>
	  Before when making a Card I would resize the image with height and width properties to make the image fit the parent container. However I found out that using:background-size:cover; will automatically reduce the size to fit the secelected container. i also then went to apply this to my main background images for each section I was creating.
    Whilst making the diferent sections in my blog, when reducing the screen size I noticed that my text in one section was overlapping the other. I used stackoverflow and found my answer and it because I was initially using <strong> height: 100%; </strong> in my sections. </div>

   https://stackoverflow.com/questions/48514628/text-overlaps-background-when-i-shrink-browser-size-even-when-height-set-to-100>/
	  Responsive Units 
	I quickly learned that the units that I size with in CSS had absolute correlation to my blog being responsive. 
    Using <strong> px </strong> all the time isnt going to benefit a responsive site as it is absoulte and rigid in different screens. Instead it is better to use <strong> % </strong> for width and height and <strong> em </strong> for padding and margin.  </div>
	<div> <strong> Breakpoints for width and media queries </strong> </div>
    
  <p>  When I was finished with the main styling and structure of my blog page , I wanted to search references to when I should set diffrent media queries.
    Now let’s see some common breakpoints for widths of devices:
• 320px — 480px: Mobile devices
• 481px — 768px: iPads, Tablets
• 769px — 1024px: Small screens, laptops
• 1025px — 1200px: Desktops, large screens
1201px and more —  Extra large screens, TV!
    https://www.freecodecamp.org/news/css-media-queries-breakpoints-media-types-standard-resolutions-and-more/>I learnt that you have to start with the largest (max-width) media querie and work down to the smallest width you want to set, as css works in a top down rule form.nWithin setting these media queries I wanted to remove the <strong> :hover </strong> psuedo-class when the screen is reduced. I learned about the style{  pointer-events: none; }  to remove this effect.


    Vanilla JavaScript 

In this project it required me to use vanilla JavaScript.
    I learned about what an <strong>array like object </strong> is and why it is used for 
	- document.getElementsByClassName('toggle-button')[0]

It doesn't have the same method as an array such as push, pull , etc but it has similarities of index properties and length.

Summary
    
 <p> Overall I enjoyed working this blog project as it refreshed my css skills and I also took it a step further to add some Vanilla JavaScript. My main focus was to build a responsive web-page which I acheieved, and because this is a key factor when building good web-pages and projects. I will continue my study on using @media queries correctly and implementing more Javascript into my future projects. </p>
