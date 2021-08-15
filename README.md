# udacity-landing-page

Abdelhady's Udacity Landing Page
`Version: 1.0.0`
`License: GNU GPL v3`

## INTRO

This project is maintained by Abdelhady Salah, the purpose of this project is creating a responsive landing page that works well on mobile devices.

## ARCHITECTURE

- css
    - style.css
- img
    - donut-icon-1.png
    - emerald-icon.png
    - 'IMAGE COPYRIGHT NOTICE.txt'
- js
    - app.js
- index.html
- LICENSE
- README.md

## FEATURES

- Content is dynamically created using JavaScript
- Code is properly structured and documented inside the source files
- Make proper use of document fragments and reduce the use of event listeners for best performance
- Random paragraphs and headers generated per section
- Add as many sections as you like
- Active state for both navigation and section elements
- Easy navigation
- Scroll to top
- Collapse sections by double click
- A little use of animations for decoration
- HTML layout consists of: Navigation, Content and Footer
- Hamburger list for mobile devices
- Responsive and functional on mobile devices

P.S. I'm using the best JavaScript practices as much as I could

## INITIALIZE

```js
function main() {
    //This function is the thing that processes all the code we created, to actually make use of it.

    //Create the logo, use our emerald image and my... well.. name :)
    customNav.createNavLogo('img/emerald-icon.png', 'Abdelhady\'s');

    //Add our hamburger list at the beginning
    customNav.createNavHamburger();

    //You can create a billion (wouldn't be out of bounds? idk)
    createSections(11);

    //Create navigation list based on how many sections you created!
    customNav.createDynamicNavSections();

    /* Scroll top functionality */
    const scrollTopElement = document.querySelector('.scroll-top');
    scrollTopElement.addEventListener('click', function() { //If you click it, you go up
        window.scrollTo(0, 0);
    })
    return true;
}
```

## LICENSE NOTICE

```js
/*
 *     AUTHOR: 
 *     -   Abdelhady 'H2O' Salah
 * 
 *     VERSION:
 *     -   1.0.0
 * 
 *     REPOSITORY:
 *     -   https://github.com/h2o-creator/udacity-landing-page
 * 
 *     LICENSE NOTICE:
 *     -   This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation; 
 *         either version 3 of the License, or (at your option) any later version.
 * 
 *     -   This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; 
 *         without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
 * 
 *     -   You should have received a copy of the GNU General Public License along with this program. If not, see https://www.gnu.org/licenses/.
 */
```

