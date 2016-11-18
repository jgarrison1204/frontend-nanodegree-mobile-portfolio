## Website Performance Optimization portfolio project

The goal of this project was to make a troublesome web app more performant by applying optimization techniqures learned in two classes: Website Performance Optimization and Browser Rendering Optimization.

###Part 1: Optimize PageSpeed Insights score for *index.html*

**Goal:** Have PageSpeed Insights score > 90 for moblie and desktop. 
Please see link to optimized site https://jgarrison1204.github.io/frontend-nanodegree-mobile-portfolio/

To test the PageSpeed please copy and paste the link above to the following [site](https://developers.google.com/speed/pagespeed/insights/)

####Optimizations Made

1. Reduced the number of critical resources by moving all CSS to an internal style sheet and calling Google Fonts from a script tag.
2. Added `async` tags to js files to remove render blocking javascript.
3. Resized and compressed images.

###Part 2: Optimize Frames per Second in *pizza.html*

**Goal:** Optimize JS so frames per second rate is 60 fps or higher. 

####Major Optimizations Made

1. Changed `querySelector` to `getElementById` in `changeSLiderLabel function` to reduce scope of the dom selector has to travel.
2. Identified jank because of forced synchonous layout in a for loop. Refactored for loop to a forEach loop outside and accessed layout change outside the loop. 
