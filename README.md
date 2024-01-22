# South Wales Pottery Club

## Contents
* [UX - Strategy](#ux---strategy)
  * [Project Goals](#project-goals)
  * [Business Goals](#business-goals)
  * [Competitor Review](#competitor-review)
     * [Cardiff Pottery Workshop](#cardiff-pottery-workshops)
     * [Peggy's Pots](#peggys-pots)
     * [Stupots](#stupots)
  * [User Goals](#user-goals)
  * [User Stories](#user-stories)
* [UX - Scope](#ux---scope)
  * [Limitations Identified](#limitations-identified)
  * [Current Phase](#current-phase)
* [UX - Structure](#ux---structure)
  * [Sitemap](#sitemap)
* [UX - Skeleton Plane](#ux---skeleton-plane)
  * [Wireframes](#wirerames)
* [UX - Surface Plane](#ux---surface-plane)
  * [Design Choices](#design-choices)
   * [Colour Palette](#colour-pallette)
   * [Typography](#typography)
  * [Features](#current-features)
* [Testing](#testing)
* [Known Bugs](#known-bugs)
* [Deployment](#deployment)
* [Technologies Used](#technologies-used)
* [Acknowledgements](#acknowledgements)



## UX - Strategy 
### Project Goals

The goal of this project is to create a user-centric website for an up and coming pottery class business in South Wales.

The business has not yet begun trading so at this time they are looking to establish an online presence ahead of their launch. The project aims to identify the potential market for pottery classes by evaluating similar businesses and researching customer needs. 

The outcome of this project will target consumers appropriately and add value to their experience by utilising UX design principles. The site will be cleanly presented, easy to navigate and encourage enquires through clickable links. The user will also have easy access to all relevant information wihtout having to search through multiple pages. 

### Business Goals

* To create an online presence for the business
* To attract customers and build membership
* To provide information on classes, contact information and the location of the studio

### Competitor Review

#### Cardiff Pottery Workshops 

 [Cardiff Pottery Workshops](https://www.cardiffpotteryworkshops.com) are a successful business based in Cardiff. They have  wide range of classes and membership options available including lessons, studio space for rent and social evenings.
 
  Although very informative, the website is not the most intuitive and seems to lack responsiveness when viewed on a larger screen. There is a lot of empty space when you first navigate to the home page and the menu sits in the middle of the screen, it not immediately obvious that there is more content on the page. The navigation menu is a long list of things they offer in no particular order which may cause issues with users not being able to find the appropriate content quickly. 

 Further down, they have links to different pages within the about section. These link to new pages with class descriptions, however on testing a number of the links don't work. Presenting the class descriptions in this way makes it quite challenging for the user, as it relies on them scrolling down to the appropriate section, reading the about section where you would not intuituvely look for class information, and then unable to find the information with broken links. 

The contact page doesn't respond to being on a larger screen, while not unusable it doesn't create the best UX experience as the input boxes seem disproportionately large for the amount of content they are designed to contain.

Lastly, the booking system is quite sporadic. Rather than having a dedicated booking section they have hidden the booking forms within the individual class pages. The personal tuition is at the bottom of the throwing classes page, which would not be where a user is likely to look for it.

While the site is comprehensive and contains a lot of useful information, it could be made more user friendly by better organising the information into relevant categories. Having a dedicated classes and booking page would rectify some of the navigation problems, while addressing some of the responsiveness issues would improve the user experience. 

![Cardiff Pottery Workshops](assets/images/readme-images/cardiff-workshops-1.png)
![Cardiff Pottery Workshops](assets/images/readme-images/cardiff-workshops-2.png)
![Cardiff Pottery Workshops](assets/images/readme-images/cardiff-workshops-3.png)
![Cardiff Pottery Workshops](assets/images/readme-images/cardiff-workshops-4.png)
![Cardiff Pottery Workshops](assets/images/readme-images/cardiff-workshops-5.png)
![Cardiff Pottery Workshops](assets/images/readme-images/cardiff-workshops-6.png)
![Cardiff Pottery Workshops](assets/images/readme-images/cardiff-workshops-7.png)

#### Peggy's Pots

[Peggy's Pots](https://www.peggyspots.co.uk/Default.aspx) is another successful business based in Cardiff. They offer pottery painting experiences and parties for people of all ages, especially catering for families.

The website is easier to navigate than the Cardiff Pottery Workshop but could also be improved upon. The navigation menu again is quite a long list that could be better organised into categories and sits below the logo.

They have included a classes section on the home page, providing a clear overview of the different class types. Clicking on these leads to a dedicated class page with descriptions and what to expect. Further down they have testimonials, the subscribe form and address all sitting within the footer. There seems to be an issue with the form size making a lot of empty space next to it. The form could perhaps be moved to another section to avoid this. 

The site has been designed with Bootstrap so seems to avoid any issues with resizing, and in fact looks better on a smaller screen as there is less blank space. The contact and booking pages contain lots of information, while useful it is possibly too much text which could be moved elsewhere or edited. These pages could also potenially benefit from some adjustments to the layout as the containers seem to sit randomly across the screen on a larger screen. Overall it is a good basic site which is relatively easy to navigate, however it could be made more user friendly with some tweaking to the design and layout. 


![Peggy's Pots](assets/images/readme-images/peggys-pots-1.png)
![Peggy's Pots](assets/images/readme-images/peggys-pots-2.png)
![Peggy's Pots](assets/images/readme-images/peggys-pots-3.png)
![Peggy's Pots](assets/images/readme-images/peggys-pots-4.png)
![Peggy's Pots](assets/images/readme-images/peggys-pots-5.png)

#### Stupots 

[Stupots](https://www.stupots.co.uk/) is a pottery workshop based in Bristol. They offer a wide range of classes and experiences including corporate team building sessions.

The website is really nicely laid out and responsive. The navigation is organised into relevant categories and the logo sits nicely within the menu without being too big. They have used a video in place of a hero image on the home page which creates a welcoming experience. They have added a modal advising on extra spaces available in the taster sessions on the right of the screen which is a bit detrimental to the video, but does grab your attention. 

As you scroll down there is information on the highlighted experiences that they offer, testimonials, a scrolling gallery incorporating Javascript and finally a large footer which contains a lot of information inluding the address and contact information. It is well presented with interesting graphics, the layouts include images and descriptions defined into sections by different background colours and the descriptions are comprehensive without being too long. Each section includes a link to a dedicated page with more information encouraging clicks.

The booking and contact pages are also well laid out with well proportioned containers and are clean without too much information. The site is responsive and works well on both large and small screens. They've used a number of frameworks including Yoast SEO and seems to have been built on Wordpress. Overall this is a really user friendly website that looks professional and stands out as a good example from the research for this project.

![Stupots](assets/images/readme-images/stupots-1.png)
![Stupots](assets/images/readme-images/stupots-2.png)
![Stupots](assets/images/readme-images/stupots-3.png)
![Stupots](assets/images/readme-images/stupots-4.png)
![Stupots](assets/images/readme-images/stupots-5.png)
![Stupots](assets/images/readme-images/stupots-6.png)
![Stupots](assets/images/readme-images/stupots-7.png)
![Stupots](assets/images/readme-images/stupots-8.png)

### User Goals

Based on the competitor research, a number of key features have been identified. Users of the site will be able to:

* Browse different classes and events
* Find class and event timetables
* Find the location of the studio
* Find contact information for the business
* View a gallery of the studio in action
* View information on the benefits of pottery for wellbeing

### User Stories

* User 1 is looking for new activities to do with the kids over the school holidays

* User 2 is looking for a new hobby and the opportunity to make new friends

* User 3 is an intermediate potter looking to improve their skills

* User 4 is looking for fun new date night ideas

* User 5 is looking for a unique experience gift for a loved one

* User 6 was referred by the local mental health team


## UX - Scope

### Limitations Identified 

It is not possible to implement all desired features at this stage for a number of reasons. The contact form will not be linked to a database without back-end development, and the gallery will be static as there will be no Javascript. There will also be limited pages due to time contraints and the assesment criteria required for the project.

I have used Bootstrap to enable a responsive menu in the design but chosen to limit the use of this framework in other areas of the site. The reason for this decision is that I wished to have a good understanding of CSS and did not want to always be reliant on Bootstrap to help with responsiveness. The outcome of this has been learning to 
successfully impliment CSS grids for layouts and media queries to enable responsiveness.

### Current Phase

* Build a functioning website to create an online presence for the business 
* Present class information and timetable 
* 

## UX - Structure

### Sitemap

Navigation

![Site map wireframe](assets/images/wireframes/site-map.png)

## UX - Skeleton Plane

### Wirerames

Home Page

![Home page wireframe](assets/images/wireframes/home-page.png)

Classes Page

![Classes page wireframe](assets/images/wireframes/class-page.png)

Gallery Page

![Gallery page wireframe](assets/images/wireframes/gallery-page.png)

Contact Page

![Contact page wireframe](assets/images/wireframes/contact-page.png)


## UX - Surface Plane 

### Design Choices 

#### Colour Pallette

Pottery is a relaxing and slow-paced activity so I chose to keep the colour palette quite neutral to ensure that none of the elements would be overpowering and create a calm aesthetic. 

![Colour Palette](assets/images/readme-images/colour-palette.png)

#### Typography

The font for the website is **Montserrat**, generated by Google Fonts. This was chosen due to being a clean contemporary font that gives the document a touch of sophistication. It is clear and easy to read without compromising on style.
![Montserrat Font Example](assets/images/readme-images/font-example.png)

#### Layout 

Colours/fonts/layout/images/order/sequence/brand

Screenshots 

## Features

### Current Features

Screenshots

* Home page with hero image
* Navitagion to:
  * About section
  * Classes
  * Gallery
  * Timetable
  * Contact
* Class sub navigation:
  * Children's classes page
  * Adult's begginner classes page
  * Adult's improver classes page
  * Wellbeing classes page
  * Events page
  
### Future Features

* Book classes online
* Purchase memberships online
* Create an online shop to sell student's work

## Technologies Used

* HTML
* CSS
* Git
* Github
* Codeanywhere/VS code/Gitpod
* Bootstrap
* Balsamiq
* Google Fonts
* Font Awesome
* GIMP

## Testing
03/01/23 - All social links working

## Known Bugs

## Deployment

### How to run project locally

## Credits

### Content

### Media

Map 

[Google Maps](https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d19876.57543532705!2d-3.6157785047719218!3d51.4843713332673!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x486e6da60f85f263%3A0x50d8b23d4977cb0!2sEwenny%2C%20Bridgend%20CF35%205BL!5e0!3m2!1sen!2suk!4v1704639927687!5m2!1sen!2suk)

Images

Many thanks to all the creators of the free stock images used to create this website. Links to the source for each image are available below: <br>
[Background Image Main](https://www.pexels.com/photo/person-holding-wooden-rolling-pin-7559748/) |
[Pot painting](https://pixabay.com/photos/hand-art-pot-master-man-handmade-5441435/) |
[Country house](https://pixabay.com/photos/country-house-villa-ingrown-lonely-5019947/) |
[Mum and Son](https://www.freepik.com/free-photo/mother-with-son-pottery-class_10705274.htm#query=pottery%20class&position=47&from_view=search&track=ais&uuid=15eefbbd-5591-44f1-a7ae-5bea9a06561a) |
[Children](https://www.freepik.com/free-photo/brothers-pottery-class-together_10703805.htm#query=pottery%20class&position=37&from_view=search&track=ais&uuid=15eefbbd-5591-44f1-a7ae-5bea9a06561a) |
[Couple](https://www.freepik.com/free-photo/mutual-creative-work-adult-elegant-couple-casual-clothes-aprons-people-creating-bowl-pottery-wheel-clay-studio_10164980.htm#query=pottery%20class%20couples&position=48&from_view=search&track=ais&uuid=b3ad02d6-f0d1-41af-a080-5162b03a9e45) |
[Pots on shelf](https://www.pexels.com/photo/pottery-on-a-wall-shelf-6615807/) |
[Workshop](https://www.pexels.com/photo/photo-of-ceramic-kitchenware-on-shelves-3094041/) |
[Plant pot](https://www.pexels.com/photo/photo-of-ceramic-kitchenware-on-shelves-3094041/) |
[Studio Class](https://www.pexels.com/photo/couple-creative-working-indoors-9733232/) |
[Cactus](https://www.freepik.com/free-photo/still-life-with-cactus-plant_44590359.htm#query=website%20background%20pots&position=14&from_view=search&track=ais&uuid=5241e72f-f9bc-465d-915b-89e26216952c) |
[Plate](https://www.freepik.com/free-photo/top-view-brown-plate-empty-light-blue-plate-food_10543301.htm#page=3&query=Website%20background%20pottery&position=21&from_view=search&track=ais&uuid=a6dbcc91-eeb2-4210-b3a3-0a365894d206) |
[Multi-coloured](https://pixabay.com/users/hans-2/?utm_source=link-attribution&utm_medium=referral&utm_campaign=image&utm_content=9367) |
[White jugs](https://pixabay.com/users/noname_13-2364555/?utm_source=link-attribution&utm_medium=referral&utm_campaign=image&utm_content=4465357) |
[Hanging Mugs](https://pixabay.com/users/publicdomainpictures-14/?utm_source=link-attribution&utm_medium=referral&utm_campaign=image&utm_content=21905) |
[Lady Sculpture](https://pixabay.com/users/disappearingdiamonds-3977653/?utm_source=link-attribution&utm_medium=referral&utm_campaign=image&utm_content=3394318) |
[Cats](https://pixabay.com/users/leoleobobeo-1487549/?utm_source=link-attribution&utm_medium=referral&utm_campaign=image&utm_content=2759936) |
[Student](https://www.pexels.com/photo/pottery-making-classes-15096491/) |
[Child](https://www.pexels.com/photo/girl-in-art-class-3965526/) |
[Happy pot](https://www.pexels.com/photo/green-leafy-plant-potted-on-clay-pot-993626/) |
[Men in Studio](https://www.freepik.com/free-photo/side-view-man-doing-pottery_31124478.htm#query=pottery%20class&position=7&from_view=keyword&track=ais&uuid=8218caed-1a9f-4aae-88af-c016115a128) |
[Random pots](https://www.freepik.com/free-photo/various-ceramic-vases-with-paint-pottery-concept_10267527.htm#page=3&query=ceramics%20colourful&position=33&from_view=search&track=ais&uuid=87aa8cf3-c79b-4126-bf35-7f4bef18996a)

### Code

[Rounded corners tutorial](https://unused-css.com/blog/css-rounded-table-corners/#:~:text=If%20you%20are%20only%20rounding,done%20with%20a%20box%2Dshadow%20.)

[Responsive background images with Bootstrap 5](https://www.youtube.com/watch?v=W87XNjvXiWw&t=178s)

[Bootstrap Navbar](https://getbootstrap.com/docs/4.0/components/navbar/)

[Autofit CSS Grids](https://www.youtube.com/watch?v=QO-vcJFRgOg)
