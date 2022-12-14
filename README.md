# Beatrix Chis Hunyadi

![Site landing page](assets/readme/responsive.jpg)
#### [**Live Website**](https://noemichis.github.io/beatrix-ch-portfoliowebsite/)


This project is a portfolio website for illustrator, Beatrix Chis Hunyadi. The main purpose is to create an online presence for the artist and showcase her work. The site will target anyone interested in digital art and illustration, future collaborators, employers. It is a responsive design and it can be viewed on different sized devices.

## User goals 

- Understand the purpose of the site immediately.
- Become more familiar with the artist and her work.
- Navigate easily between sections and pages.
- Enjoy the diversity and creativity.
- Get in touch easily.

## Design

The design is based on the work of Beatrix and the colors were chosen with the help of [Coolors](https://coolors.co). I found this a great tool to identify combinations of colors used in an image, which afterwards can be used on other elements to create consistency.

- The combination obtained is the following:

![Purple-blue sky color palette result](assets/readme/image-palette.jpg)

- After considering the contrast, the following color palette was chosen with addition of a darker purple for text and reduced opacity when used as a container.  

![Four color collage](assets/readme/project-palette.png)


The fonts were matched in [Google Fonts](http://fonts.google.com) and imported. `Recursive` is used for the larger headings and navbar, while `Merriweather Sans` for smaller headings and paragraphs. 


## Features

### Navigation
- The navigation bar is part of the header and it stays at the top of the page, offering better accessibility for the user at all times.
- On the left, the logo creates a link to the landing page. 
- On the right, the navigation links lead to the `About` section, `Gallery` and `Get in touch` pages.
- Navigation elements scale up on hover, improving user experience.
- An active class is set so the current page is underlined.  

#### Navigation on larger screens
![Navigation bar for larger screens](assets/readme/nav-desktop.jpg) 
#### Navigation on mobile
![Navigation bar for mobile](assets/readme/nav-mobile.jpg)

### Hero section
The Hero section is the landing page of the website containing one of the illustrations of Beatrix, her name and a link that leads to the Gallery page.

![Hero section](assets/readme/hero.jpg)

- Scale up hover effect is added to the `Portfolio` link and styled to appear as a box.

### About

Contains a short introduction of the artist under the Hero section.
- The `About` navigation hyperlink leads to the beginning of the section.

![Message from the artist and four round images](assets/readme/about.jpg) 

- *Social media* and *contact form* are links, are highlighted on hover and can be clicked.

![Introduction message with highlighted social media mention](assets/readme/message-hover.jpg)

- Responsive image links to gallery and specific projects with scale up hover effect.

#### Image links on mobile

![Four round images displayed in a grid](assets/readme/image-links.jpg)

### Footer

The footer contains links to social media platforms, which open in a new tab.

- Two different styles were used for the footer: 

- one is used on the main page using the same pattern as the Hero image.

![Purple-blue footer with social media icons](assets/readme/footer-index.jpg)   
- one is matching the header and is used on the Gallery and Get in touch pages.

![Clear footer with social media icons](assets/readme/footer-second.jpg) 

### Gallery

A showcase containing some of the artist's bigger projects and sketches organized in a responsive grid.

![Gallery displaying images of different sizes](assets/readme/gallery.jpg)

- There are multiple ways to navigate to this page as contains what users would be looking for:
    - `Gallery` navigation link in Header
    - `Portfolio`
    - image links from About section that lead to the exact project

- The background is following the pattern of the Hero image, while the header and footer stay neutral

### Get in touch

The Get in touch Page is a simple contact form where users can send their enquiries and thoughts to the artist.

![Get on touch mobile display, containing form](assets/readme/get-in-touch.jpg)

- This page can easily be accessed through:
    - the `Get in touch` navigation link. 
    - the *contact form* mention included in the message from the About page.
     
- The form requires the selected fields to be completed before submitting. 
- The body background uses the same image as the Gallery page, while the form background matches the neutral header and footer. 

## Features to add in the future

- The Gallery page would benefit from an additional navigation element to make viewing projects more efficient. The idea would be similar to the image links used on the About page, with much smaller cards and styled differently. 
- Make images so they can be viewed enlarged when clicked
- Create own *Thank You* page  

## Testing

### Automated testing

- All html pages were tested with [W3C Markup validation Service](https://validator.w3.org/)
![Markup validation result](assets/readme/html-valid.jpg)

- The CSS code was tested with [The W3C CSS Validation Service](https://jigsaw.w3.org/)
![CSS validation result](assets/readme/css-valid.jpg)

- [Code Spell Checker](https://open-vsx.org/extension/streetsidesoftware/code-spell-checker) Github extension was used throughout development

- [Lighthouse](https://developer.chrome.com/docs/lighthouse/overview/) was used to measure performance, accessibility and best practices. Every page was tested both on mobile and desktop and the results were good.

#### The test for the landing page returned the same result for mobile and desktop
![Lading page lighthouse result](assets/readme/index-mobile-test.jpg)

#### Gallery page test had a better result on desktop
![Gallery page desktop result](assets/readme/gallery-desktop-test.jpg)

#### Lower on mobile, due to some larger images - I tried to use lower resolution images where possible, but had to ensure relatively good quality. Compression helped a lot, but still place for improvement.
![Gallery page mobile result](assets/readme/gallery-mobile-test.jpg)


### Manual testing

- The responsiveness was tested throughout development with [Chrome Dev Tools](https://developer.chrome.com/docs/devtools). 
- It is tested to work in different browsers.
- The links have been thoroughly tested and no broken links have been found.
- External links open in a new tab.
- Tests on different mobiles and large screens were performed too, the website responded well.
- Contact form was also tested, fields require validation, submit is successful.

### Bugs

#### Resolved

1. Lighthouse pointed out issues with the size of the images: 
    - re-sized files for a better fit and converted them into .webp, which helped increase performance score.

2. Background was re-positioning on the screen when on mobile:
    - I tried multiple approaches to fix this issue and the solution included all of them:
        - adjust background height
        - adjust background position and size
        - modify html structure 
        
3. Footer moves on Get in touch page:
    - Several unsuccessful attempts were made to debug, was found that the background image was wrapping under the footer only on specific tablet sized screens
    - Lowered background image z-index and seems to have fixed the issue for now. 

#### Unresolved

1. When clicked the image links from the About page don't navigate to the title, but just below it.
    - I tried to move the ID around, but that doesn't resolve the issue
    - Seems to be caused bu the sticky header

## Deployment

This project was developed and deployed through [GitHub](https://github.com), using [Gitpod](https://gitpod.io) as development platform and [VSCode](https://code.visualstudio.com/) as the default code editor. 

The following *`git commands`* were used to commit and push the changes to the repository: 
- **git status** - list changes to files
- **git add** - add modified files to staging  area
- **git commit** - explain changes made to files
- **git push**  - push all files from staging area to main **Github** repository

[GitHub Pages](https://pages.github.com/) was used to deploy the project with the following steps:
1. Log into **Github** and open project repository
3. Navigate to `Settings`
4. Find and click on `Pages` in the left-hand side menu
5. Under `Source` select `Deploy from branch` 
6. Click the dropdown menu under `Branch` and select `main` and **Save**
8. Refresh the page and find link to deployed project at the top

## Technology and resources

- [HTML5](https://en.wikipedia.org/wiki/HTML5)
- [CSS](https://en.wikipedia.org/wiki/CSS)
- [Github](https://github.com) - create, develop and deploy project
- [Gitpod](https://gitpod.io) - used as remote development platform to write and test code
- [Google Fonts](http://fonts.google.com) - online font library 
- [Coolors](https://coolors.co) - color palette generator used to identify the colors of the hero image and create a matching combination
- [Fontawesome](https://fontawesome.com) - online icon library and toolkit for the social media section
- [Chrome Dev Tools](https://developer.chrome.com/docs/devtools) - great tool for checking responsiveness on different screen sizes, making test changes and troubleshooting 
- [Figma](https://www.figma.com) - design tool 
- [Online Converter](https://www.online-convert.com/) - convert .jpeg and .png images to .webp for better site accessibility
- [Favicon](https://favicon.io/) - generate favicon used in head of page
- [Am I Responsive](https://ui.dev/) - test responsiveness and create main image
- [Lighthouse](https://developer.chrome.com/docs/lighthouse/overview/)
- [W3C Markup validation Service](https://validator.w3.org/)
- [The W3C CSS Validation Service](https://jigsaw.w3.org/)

## Credits

#### All images across the site are designed and created by **Beatrix Chis-Hunyadi**, including the logo and favicon. 


Several learning sites were visited throughout the development of the project, as:
- [Code Institute Program](https://codeinstitute.net/)
- [W3Schools](https://www.w3schools.com)
- [MDN](https://developer.mozilla.org/en-US/) 
- [CSS-tricks](https://css-tricks) 
- [Stack Overflow](https://stackoverflow.com/)

Found great inspiration and help in more `CSS` tips and tricks, including `flexbox` and `grid` by following [Kevin Powell](https://www.youtube.com/@KevinPowell/featured)'s channel 

[CodePen](https://codepen.io) was very useful to see some more complex styling possibilities - inspiration for **border-radius** by [Michael Picker](https://codepen.io/mp/pen/kBEeKw)

