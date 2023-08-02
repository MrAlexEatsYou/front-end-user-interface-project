# User Centric Front End Development

## Idea - Residential Conveyancing Quote Form

### Mission Statement:

Create a simple, easy to use quote form for clients that need residential conveyancing services.

## Goals

### Business Goals:

Gain as many leads as possible
Collect data for a mailing list
Make on-boarding easy and efficient

### Customer Goals:

Get a quote in a simple and easy way

## Features To Achieve These Goals

Form to collect user data and generate quote
Easy to use navigation

## Pages Needed

### Home

Logo - Navigation
Hero
Option to choose Purchase or Sale quote

### Quote Form

Logo - Navigation
Quote Form

### About

Logo - Navigation
Explanation of services and business

## Header Footer

### Header

Logo - Navigation - External Social Media

### Footer

Business info - Map - Address

## Quote Form

### Information Needed To Make Quote

#### Minimum/Required

Name
Email
Type of Quote
Freehold or Leasehold
Property location
Using a Purchase Scheme
Misc property options (Newbuild, Unregistered, Auction, Buy To Let, Repossession, High-Rise Leasehold)
Is this an additional property

#### Nice to Have

Phone
Address
Wireframe
Using Figma - figma.com

# Wireframes

## Desktop

![Desktop Wireframe](/assets/images/desktop.png)

## Tablet

![Tablet Wireframe](/assets/images/tablet.png)

## Phone

![Phone Wireframe](/assets/images/phone1.png)
![Second Phone Wireframe](/assets/images/phone2.png)

I mainly used HTML and CSS to code this project. Bootstrap 5 has been used to enable easy styling of the project. There is also a small section of Javascript embedded in the Quote Page and the Bootstrap JS dependencies are also included.

I began by coding the header. I wanted to have a clean, simple to navigate header. In order to achieve this I use minimal colour and rely on visual indicators like thickness and fades to make the navigation intuitive. I also made the header responsive by hiding certain sections on different screen sizes and creating a ‘reveal’ button to show the full menu when viewed on a small screen.

I used a trick whereby you create a button by using a checkbox input and a label. The checkbox button is placed above the element that will be revealed, and the label for that checkbox is placed where the button will appear. Then pseudo class :checked can be used to trigger the reveal of the hidden element.

The next section I created was the footer. I wanted three sections, showing the address, a map and some blurb about the company. I used the bootstrap ‘order’ utility classes to change the order of these depending on screen size.

I then duplicated the code to make two more pages (three in total). I could then add the body code separately on each page.

The Home page and About page are quite basic, simple text based information. The quote page however, includes two separate forms contained in modals. These forms don’t go anywhere when submitted, but this is only a proof-of-concept and in the future, would realistically get put into a database and/or processed by a calculator function to provide the client with an estimated quote.

I made sure to keep all IDs unique while making this form.

# Deployment

I deployed this project using the code institute recommended process of hosting on Github Pages. I included the images from the readme in the assets folder.

After deployment, my styles and images weren't loading properly. I quickly realised that the links were wrong and had been set to `/assets/image.png` and needed to be replaced with `./assets/image.png`

If I had more time, I would like to make the layout a bit more interesting. While I like the simple design, as the idea for an elven solicitors firm grew, I could have linked the design closer to the theme.

I also realise that some of my custom CSS code is not necessary and could have been implemented with pure bootstrap utility classes. As I progressed through development, I noticed this more and more. This led me to deleting and replacing some CSS with Bootstrap code instead. If I had more time I would go back through the project and look at where else I could replace CSS with Bootstrap.