# South Wales Pottery Club

## Testing

### Contents

* [Manual Testing](#manual-testing-table)
* [Lighthouse Testing](#lighthouse-testing)
* [Responsiveness](#responsiveness)
* [HTML Validation](#html-validation)
* [CSS Validation](#css-validation)
* [Bugs Resolved](#bugs-resolved)
* [Bugs Unresolved](#bugs-unresolved)

### Manual Testing Table

| Component | Expected Outcome | Test | Result |
| --- | --- | --- | --- |
| Navbar brand | Links to home page | Clicked logo | Pass |
| Navigation links | All links go to the correct page | Clicked on links | Pass |
| Footer icons | All links correct and open in new window | Clicked on icons | Pass |
| Explore classes button | Links to class page | Clicked on button | Pass |
| Contact us button | Links to contact page | Clicked on button | Pass |
| Enquire now links | Links to contact page | Clicked on link | Pass |
| Contact form | All input required | Filled out form | Pass |
| Contact form | Formdump working | Submit form | Pass |
| Google map | Shows correct place | Click on map | Pass |
| Responsiveness | Site works across all breakpoints | Google Dev tools | Pass |
| Lighthouse testing | Check accessibility | Run lighthouse | Pass |
| HTML Validator | Check for errors | Run validator | Pass |
| CSS Validator | Check for errors | Run validator | Pass |

## Lighthouse Testing 

### Home Page

On the initial lighthouse test I had a number of findings to address. I had not yet added aria-labels to the images and also had not used `h1`, `h2` etc in chronoligical order. Fixing these issues improved both the accessibility and the SEO score.

![Home page lighthouse](/assets/images/readme-images/home-page-lh-1.png)

When I added the testimonials I initially had the background set to the same colour as the footer but this was returning a contrast error. I tried changing the font to bolder but this looked strange compared to the rest of the website. I settled on making the backgrounds darker, although not ideal visually it did fix the contrast error.

![Home page lighthouse](/assets/images/readme-images/home-page-lh-2.png)

The final lighthouse score for the home page is displayed below. I was able to improve the performance slightly by compressing the image files.

![Home page lighthouse](/assets/images/readme-images/home-page-lh-3.png)

### Classes Page

The first lighthouse test for the class page came back with similar issues for the aria-labels and headings but the main issue was the performance as there are a lot of images on this page. I compressed the images unitl the score was satisfactory without compromising the quailty of the images.

![Class page lighthouse](/assets/images/readme-images/class-page-lh-1.png)

Updated score

![Class page lighthouse](/assets/images/readme-images/class-page-lh-2.png)

### Gallery Page

Again the gallery images were missing aria-labels, after these were added the score improved. I had already compressed the images as I was going along so the performance was at a level I was happy with for the number of images.

![Gallery page lighthouse](/assets/images/readme-images/gallery-lh-1.png)

Updated score

![Gallery page lighthouse](/assets/images/readme-images/gallery-lh-2.png)

### Contact Page

The contact page also had the same issues as pervious pages. The best practice score is slightly lower due to a cookie relating to the Google map.

![Contact page lighthouse](/assets/images/readme-images/contact-lh-1.png)

Updated score 

![Contact page lighthouse](/assets/images/readme-images/contact-lh-2.png)

### Responsiveness 

Responsiveness was checked both on Google Developer Tools and on [Am I Responsive](https://ui.dev/amiresponsive). Bugs encountered are discussed in the resolved bugs section.

![Site Overview](/assets/images/readme-images/site-overview.png)
![Site Overview](/assets/images/readme-images/class-page-ov.png)
![Site Overview](/assets/images/readme-images/contact-page-ov.png)
![Site Overview](/assets/images/readme-images/gallery-page-ov.png)


### HTML Validation ###

I used W3C Markup Validation service and Jigsaw to ensure there are no errors in the HTML and CSS. 

On the initial W3C Validator test an error was found where I had used an `a` element as a decendent of a `button`. I tried swapping them around but it came back with the same error. I had not realised that a button could not be used for a link before this. I removed the button and simply left the `a` element with the styling applied in CSS. It looks the same and has the same functionality but now comes back with no error.

![Html error 1](/assets/images/readme-images/html-error-1.png)

I had missed closing a `div` on a few of the pages. I added that in and that resolved the error.

![Html error 2](/assets/images/readme-images/html-error-2.png)

The validator also found that I had mislabled the contact form. I eventually got rid of the lable altogether and used a `h3` element instead as it was more semantic.

![Html error 3](/assets/images/readme-images/html-error-3.png)

There was also a stray `div` which I removed to resolve this error.

![Html error 4](/assets/images/readme-images/html-error-4.png)

There are some warnings present on the contact page where I have applied aria-labels to the font awesome icons in lieu of titles. This did not show up on Lighthouse or Wave testing so I decided to leave them in. 

![Html warning 1](/assets/images/readme-images/html-warning-1.png)

There are a number of info flags present in the validation. Most are relating to the metadata, code for external frameworks including Bootstrap and Google Fonts or comments that I have put in the code. These have been left in as they do not effect functionality.

![Home Page Validation](/assets/images/readme-images/home-page-validation.png)

### CSS Validation ###

The Jigsaw validator found an error where I had used an invalid value with the transform property. I changed the value from a percentage to a decimal which resolved the error.

The parse error was an unclosed media query near the end of the document. 

![CSS error 1](/assets/images/readme-images/css-error-1.png)

This warning was returned, but as it does not effect functionality it was left as is.

![CSS error 2](/assets/images/readme-images/css-error-2.png)

After fixing these errors the validator returned a result of no errors.

![CSS Validation](assets/images/readme-images/css-validation.png)

## Bugs Resolved

### Navbar 

When adjusting the screen size the `navbar-brand` was not fitting along with the rest of the menu, forcing it to split over two lines. I applied CSS `display: none` to the navbar-brand so that it does not display on small screens which solved this, however there was then no link to the index page on the navigation menu. I added an index page link to the menu and set that to be hidden on larger screens. This enabled full navigation across all screen sizes.

![Navbar error](/assets/images/readme-images/navbar-error-1.png)

I wanted the hamburger menu to sit in the right hand side of the screen, but not the navbar brand. I applied `d-flex` to the nav items to enable this, however the navigation then became stuck open and due to time constraints I decided to change it back. This is something I may wish to look at again in the future if I revisit this project.

![Navbar error](/assets/images/readme-images/navbar-error-2.png)

### Footer

I had some initial trouble with the footer floating above the bottom of the page when I wanted it to be sticky. I eventually worked out it was due to the `margin` being set to something other than zero.

![First draft home page](/assets/images/readme-images/first-draft-home-6.png)

### Home Page

I was using Bootstrap at first which was causing there to be too many columns on the page. The heading was also sitting on the same line as the paragraph. I decided to move away from Bootstrap and looked at other ways of organising the layouts using CSS only. Inititally, I followed a tutorial which involved displaying the content as a table and using float/clear properties but I still felt there must be a better way. Eventually I changed it to `display: block` and used `column-count` then applied a media query to enable responsiveness as this seemed like the smoothest solution. I could of also used a grid, but didn't feel it was particularly neccessary for just two components.

![First draft home page](/assets/images/readme-images/first-draft-home-2.png)

### Classes Page

When I started building the class page grid the class descriptions were sitting in their own grid area. I felt this could be improved upon as it wasn't immediately obvious the description and the image were connected. This was resolved by containing all the content of each class description in a `div` as only direct decendents become grid items.

![First draft classes page](/assets/images/readme-images/class-page-fd-1.png)

Once I got the image and description to be contained as a single grid item I had a lot of difficulty getting the images to sit within the containers. I tried lots of different combinations to solve this, it was eventually solved by setting the `object-fit` property to `cover` and setting the height and width of the images.

![First draft classes page](/assets/images/readme-images/class-page-first-draft.png)

Before I set the height and width of the images, with `grid-template-rows` set to `auto` it displayed the whole image but I felt this looked untidy. To keep the size of the rows consistent it was neccessary to set the height and width of the images. I eventually decided on applying height of 50% to the images as this worked best on all screen sizes.

![First draft classes page](/assets/images/readme-images/class-page-first-draft-2.png)

There were some major problems with the responsiveness on the classes page. It was not sitting in the centre and a lot of the content was spilling over the edge. It was resolved by removing the `padding` and `margin` from the grid. I then applied padding to the class description content instead so that it would not sit too close to the edge of the screen.

![First draft classes page](/assets/images/readme-images/class-page-fd-3.png)
![First draft classes page](/assets/images/readme-images/class-page-fd-4.png)

### Gallery Page

It was a bit challenging figuring out how to position the images on the gallery grid. Sometimes they were stretched or didn't fit where I had hoped to place them. I tried different layouts before deciding on the final draft. 

![First draft gallery page](/assets/images/readme-images/gallery-page-fd.png)

To make the gallery responsive I used a media query to apply `display: block` and `column-count,` rather than designing a whole new grid as it seemed more efficient to do it this way. However, as it was no longer a grid the gap between the rows no longer applied so the images were all crammed together. I eventually discovered setting the images to have a `margin` resolved this.

![Gallery error](/assets/images/readme-images/gallery-error-2.png)

### Contact Page

When building the contact page I tried to put the timetable within the grid which initially seemed to work. However, once testing the responsiveness it spilled out of the container and the grid did not resize as it was supposed to. I tried setting it to span across two columns but this was also ineffective. I eventually removed it from the grid entirely and placed it underneath. 

![Timetable error](/assets/images/readme-images/contact-page-error-1.png)

### After Deployment

When I deployed the project to Github Pages the background images disappeared. They were still visible locally, and all the other images were working so I knew there must be an issue with the CSS file. I looked on a number of forums where others had had the same issue and dicovered it was an issue with the filepath. Github Pages was not recognising the URL so I tweaked it a few times until the images appeared.

![Deployment error](/assets/images/readme-images/deployment-error.png)

## Bugs Unresolved

When dropping down to a small screen the timetable heading does not sit directly above the timetable. I cannot find the reason for this, neither the timetable nor the heading seem to have any padding or margin set that would cause it to behave this way so this has remained unresolved.

![Unresolved timetable heading error](/assets/images/readme-images/timetable-unresolved.png)