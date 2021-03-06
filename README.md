# Static Comp Challenge 1

## Introduction

### Website Create By JP Carey

[My GitHub Repository](https://github.com/jaypeasee?tab=repositories)

[Turing School of Software and Design](https://turing.io/)

This was my second solo project and first project where I created a page from scratch using HTML and CSS.

The prompt was to create a new page based on an original design. The structural specs and elements of the page needed to match the layout of the provided design. That said, I had a creative license for some styles such as images, copy, icons and color palette. See the image of the required layout below.

![Static Comp Example Layout](assets/static-comp-challenge-2.jpg)

The goal was also to make this page compatible across different browsers such as Firefox, Safari and Chrome and have smooth transitions into different breakpoints for tablets and smartphones.

## Progression

The projects started with creating a repo on Github and adding directories for the `index.html`, `styles.css`, `normalise.css`, assets, and initializing them with necessary tags and hrefs.

From there, I made a low-fidelity wireframe of the design to help conceptualize the structure and how it might relate to certain HTML tags as well as CSS grid or flexbox strategies. See wireframe below.

![Low-fidelity Wireframe of the Design](assets/wireframe.png)

I was able to start organizing specific HTML tags, classes, placeholder content, and colours to give the page a rough vertical structure. I first started organizing the cards in the `<section/>` of the page, where the recipes could be found. Then I moved on to the `<nav/>`. Using the CSS grid method, I was able to align `<div>` s from each section horizontally to closer match the comp. See image below.

![First Pass at Web Structure and Design](assets/basic-structure.png)

Using additional styling techniques such as `grid-gap`, `font-sizes`, and then a `flex` method within my `grid` `<nav/>` aligned the elements closer to the comp and in finer detail.

I changed the content and images on 7 other cards to make sure that I could standardize the cards dynamically.

![Added Content, Styling, and Flex](assets/detail-dt.png)

To make the page adaptive, I created 3 media queries for different breakpoints and mostly used relative measurement units in my CSS file. Once those breakpoints kept the structure of the page usable and consistent, I played with subtle styling such as hovers, cursors, box shadows, and font sizes.

![Final product](assets/final-1.png)

![Final product](assets/final-2.png)

## Key Concepts and Challenges

### Concepts:

The `<nav/>` and the `<section/>` of cards were structured using `grid`. This allowed for a flexible, yet simple implementation. Within the `<nav/>`, I used  `flex` to align the elements properly within their grids. I mostly used relative measurement units to allow the page to be fluid and used `media queries` for multiple breakpoints to make the page more responsive.

### Challenges:

1. Using `flex` within the children of `grid` elements on the `<nav/>` was tricky to play with at first. I had to use a lot of custom padding aroung elements and icons.

2. The `<nav/>` was especially tricky to condense in smaller screen sizes. It would extend the width of the page and make all the elements below unresponsive to mobile. I ultimately changed them fro column grids to row grids at my 500px media query which made the `<nav/>` tall but at least all of the elements fit on the page.

   ![Mobile not condensing in the nav](assets/bad-mobile.png)

3. The images were different sizes, making it hard to format them all universally and give them a standard relative max-width and height. I had to roughly crop some of them to get them to fit better. Part of my solution was how wide I would let the whole section of cards get when the number of columns first decreased. Another solution  was just cropping them so they were roughly the same dimensions.

4. QAing in Firefox and Safari as well as Chrome added an extra level of challenges, especially when they arised. I needed to adjust my breakpoints to make the best compromise between the three,

## Acknowledgements

- My instructors - Casey DallaValle, Scott Ertmer, and Hannah Hudson for lectures on basic HTML, CSS and wireframing, and the independent lesson plans they provided for Flexbox and Grid displays.
- My mentors - Isaac Chabon, Kristen Cabrera, and David Becker - Who helped with me better understand the concepts of flexbox and grids styling displays in CSS.
- Other members of my cohort at Turing for providing an inclusive but creative atmosphere that allowed for free and open advice.
