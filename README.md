# LA LUCHA
La Lucha, meaning "The Fight" in Spanish is a Mexican resturant on wheels that travels the city of Athens, along with the surrounding munincipalies and brings heart-warming food to those eager to seek it out. 

## Features

### Existing Features

### Features Left to Implement

## Testing

### Validator Testing

### Unfixed Bugs
The Social links appeared to be connected with a hyphen that would open one of the social platforms in a new tab. Could not understand what had occured. Have temporarily left the issue & will address it again later.
Fixed the issue by changing the display from "inline" to "inline-block".
Resolved the issue of the background image size within their containers using the {background-size:100% 100%;} rule found in Stackoverflow.
With the help of my cousin, I was shown how to use flexbox styles wish instantly resolved the issue I was experiencing with placement & my items inexplicably being off center. I was also informed that I had been incorrectly using the postion:absolute; rule, that this was in turn responsible for much of my frustrations.
Ran the html files through W3C validator. Upon initial run through, some sections failed. Once I removed the paragraph elements from the the unordered list elements, the issue was resolved.
The same happened with running the style rules through the CSS validator. Two rules hadn't been written correctly, but once amended, it passed without any errors.

## Deployment
The repository was created on Github using the C.I. template. It was then pushed to Gitpod, where the initial layout was formed.
Spent a very long time frustrated wondering why my changes were not taking effect, and then realised that I had not linked my style.css to my index.html.
Next I worked on placing the hero image. I found that whilst I could easily set the dimensions of the container, I could not adjust the size of the photo within that container, & as a result, it was overly zoomed in. I removed the image from the style sheet, & added it to the html file instead. This assisted in fixing the size of the image, however it created a new problem in the styling, as the 'margin:0 auto;' was no longer centering the image. This was fixed by creating a 'margin-left:5%;'.
For now, there are scaling issues which will need to be addressed with the media queries, or possibly better style rules.
Decided the code was too complicated. I had guessed my way through acheiving the result I had wanted, & realised the method in which I got there was wrong. After reviewing what had occurred, I realised that I had not properly assigned my parent & child alterations to coincide with one another.
I'm still struggling with sizing the images within their containers, along with positioning the overlay text. I can control the positioning with percentages, but I would like to get them vertically aligned without it.
Leaving the issues with the home page for now, will need to seek guidance to resolve the matter.
Moving on to the 'Menu' page.
Was experiencing the same issues with the menu heading that I was on the main page. Enlisted the help of my cousin to aid me in seeing the error of my ways. Once that was finally in place & I understood how to get there, I moved on to completing the menu layout with the newly aqcuired knowledge. 
Moved on to the "locations" page. Reused the banner heading from the menu page with a few minor adjustments to accomodate the larger word. And added the locations of where the food truck will be each day of the week. Each day is linked to a page on google maps to fascilitate people in finding the truck.
Having completed most of the project (media queries still missing), I've realised that the site lacks content. I focused entirely on the design, and did not build up information to go with it. Will need to reconsider the layout, and possibly add in an "about" section. 

## Credits

### Content
- As my knowledge of implementation is limited at this point in my learning, the initial set up & style was set loosely on the 'Love Running' walk-through project. From there, I took inspitaion for the design of the navigation bar, along with the display of the social links in the footer element.
- Stackoverflow [Reply](https://stackoverflow.com/questions/16056591/font-scaling-based-on-width-of-container) was used to fix the issue with scaling font sizes, where I was reminded of how to size fonts with viewport widths & heights.
- Stackoverflow [Reply](https://stackoverflow.com/questions/1150163/stretch-and-scale-a-css-image-in-the-background-with-css-only) was used to fix the issue with image sizes within their containers, where I found the styling rule background-size: 100% 100%;.
- My cousin turned me on to [flex style rules](https://css-tricks.com/snippets/css/a-guide-to-flexbox/), & with those, I was finally able to fix my alignment issues both horizontally & vertically using the following three rules, 
1. display:flex; 
2. align-items:center; 
3. justify-content:space-between;
- Stackoverflow [Reply](https://stackoverflow.com/questions/1150163/stretch-and-scale-a-css-image-in-the-background-with-css-only) supplied the style rules to stretch the text in the "locations" page banner.
1. transform: scaleY(2);
2. transform-origin: 0 0;

### Media
- Hero image is called ["Food Truck in the Street"](https://www.thebalancesmb.com/thmb/IRZI2gmNsYFTTPCH774ohMD4uJE=/2088x1436/filters:fill(auto,1)/food-truck-in-the-street-496731672-863bfb69328341c1804fec18e39be715.jpg) by Maica

- [Three Purple Chairs - Pexel](https://www.pexels.com/photo/three-purple-plastic-chairs-3013212/)
- [Photo by Brett Sayles from Pexels - B&W Aztec food truck](https://www.pexels.com/photo/grayscale-photograph-of-two-people-standing-in-front-of-food-truck-1264937/)
- [Photo by Jess Loiterton from Pexels - shrimp tacos](https://www.pexels.com/photo/white-and-blue-bus-near-green-palm-tree-under-blue-sky-4609255/)
- [Photo by cottonbro from Pexels - chalk background](https://www.pexels.com/photo/black-wall-in-close-up-image-3826435/)
- [Photo by Andrea Piacquadio from Pexels - messy chalkboard](https://www.pexels.com/photo/woman-in-red-long-sleeve-writing-on-chalk-board-3769714/)
## Other General Project Advice
- [Photo by Rodnae Productions from Pexels - foodtruck staff](https://www.pexels.com/photo/man-and-woman-standing-in-front-of-the-food-truck-5779665/)
