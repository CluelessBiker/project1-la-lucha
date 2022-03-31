# LA LUCHA
La Lucha, meaning "The Fight" in Spanish is a fictional Mexican restaurant on wheels that travels the city of Athens, along with the surrounding municipalities, and brings heart-warming food to those eager to seek it out. It is targeted at an audience of all ages, who's only requirement is a love for food, and the will to seek it out.

The intent of the  website is to aid our audience in locating the Food Truck throughout the various days of the week. Provide them with the current menu. And last but not least, provide a brief description on who & what the company is.

![Site view across devices](/assets/images-readme/devices-layout.png)

The La Lucha site is live, the link to which can be found [HERE](https://cluelessbiker.github.io/project1-la-lucha/)

## Features

### Existing Features
#### Navigation bar:
this is included across all three pages, and provides people with an easy reference to navigate between the 'Home', 'Location' & 'Menu' pages.

![Navigation bar](/assets/images-readme/navigation-bar.png)

#### Landing Page:
This defines the feel of the website, providing the user with an image that they can easily associate to what the company is & does.

![Hero image](/assets/images-readme/home-heroimage.png)

The About section is listed right beneath the Hero Image, to provide more clarity on the company, and give a better feel to who & what it is.

![About us](/assets/images-readme/home-aboutus.png)

#### Locations Page:
A big, bold banner has been installed at the top of the page, clearly reminding the users of the page's intent. It also includes the words "Food Truck", to really instill the concept of the site to the user. As well as providing an easy to read graphic that quickly supplies the viewer with the operating hours of the company.

![Locations banner](/assets/images-readme/locations-banner.png)

Next on this page is a short blurb outlining that the locations are regularly updated, as well as the day & time they can expect the next release of locations to be provided.

![Description of locations page](/assets/images-readme/locations-description.png)

Finally, this weeks locations have been included in big, bold type, made accessible by including a link to Google Maps for each location. Additionally, the text colour changes when hovered over, to alert the user to the fact that there is a clickable link there.

![Find the truck](/assets/images-readme/locations-truckstops.png)

#### Menu Page:
The banner has been repeated once more, this time changing the keyword to "Menu". This has been done for consistency of design between the pages, and to reiterate the key information to the end user in a quick & easily accessible manner.

![Menu banner](/assets/images-readme/menu-banner.png)

A summary of the page along with a photograph has been provided, informing the users of the fresh & locally sourced, & seasonal ingredients.

![Food philosophy](/assets/images-readme/menu-description.png)

Last but not least, the current menu has been provided for the current items on offer. This again has been done in big, bold type, and divided into three sections "sides", "mains" & "drinks", so that the user can quickly distinguish what is on offer.

![What's on the menu](/assets/images-readme/menu-dishes.png)

#### Social Links:
Links to the companies social media pages can be found on the bottom of each page, & each one will take the user to the social media platform being references.

![Social Links](/assets/images-readme/social-links.png)

#### Footer comments:
A comment has been added to the footer to indicate that the site is intended for educational purposes only. This has been done as the hero-image used was sourced from a google search, and I do not have the rights to the image. The image has been credited in this document.

### Features Left to Implement
- Contact & Sign Up Page
- Gallery.

## Testing
The Social links appeared to be connected with a hyphen that would open one of the social platforms in a new tab. I could not understand what had occured. After much deliberation & viewing the style rules one by one, making adjustments or removing them altogether, I fixed the issue by changing the display from "inline" to "inline-block".

Having placed my hero images, as well as the "times" image on the menu & locations banner, I was having an issue with the size of the images themselves. Either the images were zoomed in more than what they should be, or they were not showing at all, being too large for their containers. The issue with the hero image was resolved by adding the following style rule 
```
background-size:100% 100%;
```
This solution was brought to my attention in a thread found in Stackoverflow. The graphic in the menu/locations banner was then fixed by adding the images to the html documents as image elements, & then defining their size in the CSS rules. This same method was then used to add in additional images to each page.

Next I struggled with centring the different elements on the page, and often found that the elements would align to the left of the page, despite having set the rule to {margin:0 auto}. I fought with this issue for longer than I should, forcing the placements of the images with numerous style rules. Knowing that my method of attack was incorrect, I enlisted the assistance of my cousin, who then informed me that the main source of my frustration was the 
```
position:absolute;
```
rule, and directed me towards the 'flex' styling rules that immediately made things much easier & my code far less unruly.

Ran the html files through W3C validator. Upon initial run through, some sections failed. Once I removed the paragraph elements from the the unordered list elements, the issue was resolved.

The same happened with running the style rules through the CSS validator. Two rules hadn't been written correctly, but once amended, it passed without any errors.

I tried to add a static navigation panel at the top that would always be visible no matter how far down the page a user scrolled. However what ended up occurring, was that whilst I was able to achieve this, the section element below (such as the Hero Image), would then shift up in its placement & move behind the navigation element. The navigation element would also shift to the left of the page, & would need creative adjustments to the margins to return back to its original position of being centred. I was unable to figure out how to resolve this, and returned the navigation bar to its original design. I may revisit this feature later on & try to correct it.

The media queries proved to be a challenge. It took a lot of trial & error in the Chrome Dev tool to adjust everything accordingly so that it would not display horribly out of sync when the page was to be resized. I found undoing my horizontal alignments where I had applied flex styles to be particularly challenging, however eventually phrased my my conundrum correctly in my google search, & was able to locate the resolution on Stackoverflow.

As I moved through the different sizes of queries, managing the banner & wording I had overlaid on the hero image became near impossible. After several hours of fiddling and beating my head against the wall, I decided to try it from a new approach. I moved the banner png into the index.html file, and removed it as a background image from the css style sheet. This ultimately gave me more control over the size & continuous position of it, and allowed me to move it around the page & overlay the text much more effortlessly. What I did end up having to do however, was create a media query for each 100px bracket, as the overlaying text would still move to far. 

### Validator Testing
- html files pass through the [W3C validator](https://validator.w3.org/) with no issues found.
- html files pass through the [Jigsaw validator](https://jigsaw.w3.org/css-validator/) with no issues found.
- page has an excellent Accessibility rating in Lighthouse

![Accessibility score](/assets/images-readme/accessibility-score.png)

- Tested the site opens in Brave, Chrome & Safari without issues.
- All links open to external pages as intended.

### Unfixed Bugs


## Deployment
The site was deployed to GitHub pages. The steps to deploy are as follows:
- In the GitHub repository, navigate to the Settings tab
- From the source section drop-down menu, select the Master Branch
- Once the master branch has been selected, the page will be automatically refreshed with a detailed ribbon display to indicate the successful deployment.
- The live link can be found [HERE - La Lucha](https://cluelessbiker.github.io/project1-la-lucha/index.html)

## Credits

### Content
As my knowledge of implementation is limited at this point in my learning, the initial set up & style was set loosely on the 'Love Running' walk-through project. From there, I took inspiration for the design of the navigation bar, along with the display of the social links in the footer element.

Stackoverflow [Reply](https://stackoverflow.com/questions/16056591/font-scaling-based-on-width-of-container) was used to fix the issue with scaling font sizes, where I was reminded of how to size fonts with viewport widths & heights.

Stackoverflow [Reply](https://stackoverflow.com/questions/1150163/stretch-and-scale-a-css-image-in-the-background-with-css-only) was used to fix the issue with image sizes within their containers, where I found the styling rule 
```
background-size: 100% 100%;.
```
My cousin turned me on to [flex style rules](https://css-tricks.com/snippets/css/a-guide-to-flexbox/), & with those, I was finally able to fix my alignment issues both horizontally & vertically using the following three rules:
```
1. display:flex; 
2. align-items:center; 
3. justify-content:space-between;
```
Stackoverflow [Reply](https://stackoverflow.com/questions/1150163/stretch-and-scale-a-css-image-in-the-background-with-css-only) supplied the style rules to stretch the text in the "locations" page banner.
```
1. transform: scaleY(2);
2. transform-origin: 0 0;
```
Stackoverflow [Reply](https://stackoverflow.com/questions/63437323/how-to-remove-display-flex-in-media-query) provided the answer on how to undo my flex styling rule.

Stackoverflow [Reply](https://stackoverflow.com/questions/4888377/how-to-add-a-browser-tab-icon-favicon-for-a-website) explained how to add an icon to the browser tab of the web page.

Support was provided by my fellow student [Mats](https://github.com/Pelikantapeten/p1-nacka-tomato-society) by aiding me in bouncing off ideas & venting frustrations. They were also immeasurably helpful in explaining Media Queries in a way that I was able to grasp.

### Media
- Hero image is called ["Food Truck in the Street"](https://www.thebalancesmb.com/thmb/IRZI2gmNsYFTTPCH774ohMD4uJE=/2088x1436/filters:fill(auto,1)/food-truck-in-the-street-496731672-863bfb69328341c1804fec18e39be715.jpg) by Maica

The following images came from Pexel:
- [Three Purple Chairs - Pexel](https://www.pexels.com/photo/three-purple-plastic-chairs-3013212/)
- [Photo by Brett Sayles - B&W Aztec food truck](https://www.pexels.com/photo/grayscale-photograph-of-two-people-standing-in-front-of-food-truck-1264937/)
- [Photo by Jess - shrimp tacos](https://www.pexels.com/photo/white-and-blue-bus-near-green-palm-tree-under-blue-sky-4609255/)
- [Photo by cottonbro - chalk background](https://www.pexels.com/photo/black-wall-in-close-up-image-3826435/)
- [Photo by Andrea Piacquadio - messy chalkboard](https://www.pexels.com/photo/woman-in-red-long-sleeve-writing-on-chalk-board-3769714/)
- [Photo by Rodnae Productions - foodtruck staff](https://www.pexels.com/photo/man-and-woman-standing-in-front-of-the-food-truck-5779665/)
- [Photo by Roberto Nickson - palm trees](https://www.pexels.com/photo/green-and-brown-coconut-trees-under-clear-blue-sky-2486168/)

Stocksnap supplied this one:
- [Photo by Bruce Mars - vegetable stand](https://stocksnap.io/photo/vegetable-stall-KZ19NV9MVY)
