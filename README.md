# fashion-test-site
Select Fashion Sample Site: A Modern Showcase of Style and Trends

1. HTML Structure (index.html)
The HTML file defines the structure of the webpage. Below is a breakdown of the key sections:

<!DOCTYPE html>: Declares the document type as HTML5.

<html lang="en">: Sets the language of the document to English.

<head>: Contains metadata about the webpage.

<meta charset="UTF-8">: Defines the character encoding for the page.
<meta name="viewport" content="width=device-width, initial-scale=1.0">: Ensures the page is responsive on different devices.
<link rel="stylesheet" href="style.css">: Links the external CSS file for styling.
<title>Document</title>: Defines the title of the webpage, which can be customized as needed.
<body>: Contains the visible content of the webpage. It's divided into several sections:

<div id="main">: The main container for the webpage layout.
<div id="left-top-left">: Contains a square graphic element.
<div id="square"></div>: Represents a small, rotated square that serves as a decorative element.
<div id="left-top-right">: Contains the navigation menu.
<h4>Menu</h4>: The title "Menu."
<h5> elements: Links for "Home Page," "Portfolio," "Fashion Week," "News/Article," and "Contact."
<h6><i class="ri-menu-line"></i></h6>: A hidden icon for smaller screens.
<div id="left-center">: Contains the main text/banner with large headings.
Four <h1> elements: Display the text "SELECT," "FASHION," "MOD.05-," and "SCENE."
<div id="left-bottom">: A text block with placeholder content (<p> element), which can be replaced with a relevant description.
<div id="right">: A section containing a video.
<video autoplay loop muted src="./video.mp4"></video>: Automatically plays a muted video on a loop.
<div id="arrow">: A large arrow button used for navigation.
<i class="ri-arrow-right-line"></i>: An arrow icon from the Remixicon library.
  
2. CSS Styling (style.css)
The CSS file is responsible for the visual styling of the webpage. Here’s an explanation of the major styles used:

General Styles:

* { margin: 0; padding: 0; box-sizing: border-box; }: Resets default margins and padding, ensuring consistent spacing.
html, body { height: 100%; width: 100%; }: Makes the page occupy the full height and width of the screen.
font-family: Sets the default fonts for text on the page.
Grid Layout (#main):

The layout is divided into three columns and three rows using grid-template-columns and grid-template-rows.
grid-template-columns: 25% 25% 50%;: Creates three columns with the last column taking up 50% of the width.
grid-template-rows: 30% 55% 15%;: Defines row heights for content distribution.
Decorative Square (#square):

height: 25px; width: 25px; rotate: 45deg;: Creates a small square rotated by 45 degrees to appear like a diamond.
background-color: black;: The square is black.
Navigation Menu (#left-top-right):

text-align: right;: Aligns the text to the right.
Hides certain elements (like h6 and h5) based on screen size using media queries.
h4, h5, h6: Defines font sizes and spacing for different headings in the menu.
Main Heading Section (#left-center):

The large headings (h1) have a font size of 6vw, ensuring they scale with the width of the viewport.
The nth-child(2n) selector centers the even-numbered headings.
Text Block (#left-bottom):

The paragraph (p) is styled with a small font size (9px) and a light gray color (#666).
Video Section (#right):

object-fit: cover;: Ensures the video scales without distortion.
The video has a border-radius: 10%, giving it rounded corners.
Arrow Button (#arrow):

Positioned at the center of the page using position: absolute and transformed for visual effect.
The arrow is styled with a bright orange background (orangered) and rounded (border-radius: 30%).
The icon inside (i) is scaled using font-size: 50px.

3. Responsive Design
The design is responsive, adapting to smaller screens using media queries (@media (max-width: 600px)).
On smaller screens, elements like the headings (h1) become larger, and the layout changes to a simpler grid structure.
Some elements, like menu options and text, are hidden or rearranged to better fit mobile devices.
