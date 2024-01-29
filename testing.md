# South Wales Pottery Club

## Testing

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

On the initial lighthouse test I had a number of findings to address. I had not yet added aria-labels to the images and also had not used "h1, h2" etc in chronoligical order. This also improved the SEO score.

![Home page lighthouse](/assets/images/readme-images/home-page-lh-1.png)

When I added the testimonials I initially had the background set to the same colour as the footer but this was returning a contrast error. I tried changing the font to bolder but this looked strange compared to the rest of the website. I settled on making the backgrounds darker, although not ideal visually it did fix the contrast error.

![Home page lighthouse](/assets/images/readme-images/home-page-lh-2.png)

The final lighthouse score for the home page is displayed below. I was able to improve the performance slightly by compressing the image files.

![Home page lighthouse](/assets/images/readme-images/home-page-lh-3.png)

### Classes Page

The first lighthouse test for the class page came back with similar issues for the aria-labels and headings but the main issue was the performance as there are a lot of images on this page. I compressesed the images unitl the score was satisfactory/.

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

Responsiveness was checked both on Google Developer Tools and on [Am I Responsive](https://ui.dev/amiresponsive).

![Site Overview](/assets/images/readme-images/site-overview.png)
![Site Overview](/assets/images/readme-images/class-page-ov.png)
![Site Overview](/assets/images/readme-images/contact-page-ov.png)
![Site Overview](/assets/images/readme-images/gallery-page-ov.png)


### HTML Validation ###

I used W3C Markup Validation service and Jigsaw to ensure there are no errors in the html and CSS. 

On the initial W3C Validator test an error was found where I had used an "a" element as a decendent of a "button." I tried swapping them around and came back with the same error. I had not realised that a button could not be used for a link before this. I removed the button and simply left the "a" element with the styling applied in CSS. It looks the same and has the same functionality but now comes back with no error.

![Html error 1](/assets/images/readme-images/html-error-1.png)

I had missed closing a "div" on a few of the pages. I added that in and that resolved the error.

![Html error 2](/assets/images/readme-images/html-error-2.png)

The validator also found that I had mislabled the contact form. I eventually got rid of the lable altogether and used a "h3" element instead as it was more semantic.

![Html error 3](/assets/images/readme-images/html-error-3.png)

There was also a stray "div" which I removed to resolve this error.

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