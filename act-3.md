---
layout: default
title: 3 - Adding CSS
nav_order: 4
parent: Workshop Activities
---

# Introducing CSS

If you haven’t already completed the previous exercise, please start [here](https://uviclibraries.github.io/html-css/act-1.html), as this part builds on the topics from the previous section.

This section of the workshop is on Cascading Style Sheets (CSS). Think of HTML as the builder and CSS as the artist. CSS is a different language than HTML and has different rules and structure. 

CSS is used to alter the presentation of a website. Bascially, it creates the rules for what your various HTML elements, like paragraphs (`p`), headings (`h1`, for example), and content will look like in a browser. CSS also controls things like the size and spacing between objects, like images, and text, and so much more. 

Getting CSS to work the way you want to can sometimes try your patience, but it is worth it when things work, so stick with it and be preared to have fun breaking things! 

If you have any questions, or get stuck as you work through this in-class exercise, please ask the instructor for assistance.  Have fun!

**On our journey, so far**, you should have a couple of HTML pages, with a list, some links, and a mix of text an images. Visually speaking, it looks fairly basic. Here's an example of what my `about.html` page looks like at this point: 

    <img src="images/act-3/img-browser-example.png" alt="example browser image">

Using CSS, we will make our growing website look a little more stylish and colourful.

## Linking CSS to your HTML content

- We are going to create new file, or "style sheet," for our CSS, and this file will also have an extension name, or suffix, of `.css`.
- The CSS "rules" for modern, complex websites can be very complicated, with multiple style sheets applying multiple rules to HTML files. We are going to keep things simple to start with and use just one style sheet.  
- In the Visual Code Studio (VCS) editor, create a new file in your `html_workshop` folder and name it exactly as follows: `style.css` 

    -   In order for a CSS file to have any effect on an HTML file, these files need to be linked to each other. This is done in the HTML file by using a link tag. Link tags are placed within the head tags and are self closing tags. Within the link tag we need to have two values: “rel” (which stands for relation and is required for all “link” tags), and “href” (which behaves like the “href” in our “a” tags, and it shows the path to the CSS file).<br>
        **&lt;link rel = "stylesheet" href="hello-css/styling.css"&gt;**
    -   Save the changes to your HTML file.
    -   Make sure that the link tag is in the head part of the HTML file.
    -   Once our style sheet is linked, refreshing our html file in the browser will fetch the CSS file. To see changes save your CSS file and refresh the browser.
    -   CSS code can be used within an HTML file, but to keep things simple we will only use CSS code in our CSS file.
5.  **CSS Format**
    
    <img src="images/act-3/color.png" alt="CSS block" style="width:720px;">
    
    -   In the code extract above we see a snippet of CSS code. The example is called a **declaration block**. It determines the changes we want to make to a specific HTML element, such as a paragraph <p>. Each part of the CSS declaration is explained below. Note that the colours may differ depending on the type.
        -   The **p** in this case, is the **selector**. It states which elements we want to style.
        -   **colour** in our example, is the **property**. It states which component of the element we want to change.
        -   **blue**, is the **value**. This is what we want to appear on the page.
        -   The open and closed curly brackets, these things **{ }**, behave in a similar manner as the open and closed tags do in HMTL. The example shows all the values we want **p** to have.
        -   The semicolon on line 2 signifies the ending of a "declaration".
    -   Each block can hold multiple properties. Each property should be on its own line because it makes the block easy to read. Don’t forget to add the semicolon at the end of each rule. Let’s add the following properties and values:
        `background-colour:grey;`
        `text-decoration:underline;`
    -   Feel free to change the values if you wish.
    -   Your CSS file should now contain something like this. Save it and go back to your browser and refresh your **index.html** page. You should see the changes you’ve made.
    
        <img src="images/act-3/format.png" alt="block with formatting" style="width:720px;">
    
    -   Note: not every single colour has been made available in word form. You can look up those that are available here. For colours not available, we can use its hexadecimal code. You’re probably familiar with decimal numbers: 0, 1, 2, 3, 4, 5, 6, 7, 8, and 9. Hexadecimal works the same except it has 16 unique numbers; 0, 1, 2, 3, 4, 5, 6, 7, 8, 9, A, B, C, D, E, and F. The hexadecimal numbers for colours have 6 digits, divided into three sections. 000000. The first 2 numbers represent how much red goes into the color, the middle two represents how much green is in the colour, and the last 2 are how much blue. If you’re interested in playing around with hexadecimal numbers, start by replacing “blue” with “#0000FF” and you’ll get the same result. Then change the hexadecimal number as you see fit. (#000000 is black, no colour, and #FFFFFF is white, all colours.)
6.  There are a lot of different properties that we can change. Each element has a selection of what can be changed, but there are many shared between elements. No one is expected to memorize all of them, but it’s good to know the main ones and the rest you can always look up. Here are a few to start playing with:
    -   font-style: can take on the values "normal", "italic", or "oblique"
    -   font-size: for now use px as the value, eg: 30px
    -   text-align: can take on the values "center", "left", or "right"
7.  Now add more blocks for different types of tags. Here are some suggestions:
    -   body
    -   h1 (you can assign multiple tags to the same block and have a tag in multiple blocks.)
    -   a
    -   ol
    -   ul
    -   li

    <img src="images/act-3/further-format.jpg" alt="block with more formatting" style="width:720px;">

8.  Some properties you can change are as follows:
    -   colour: #012345;
    -   background-colour: #6789AB;
    -   font-size: 10px;
    -   text-align: center; (or left or right)
    -   text-transform: uppercase; (or lowercase or capitalize)
    -   letter-spacing: 10px; (could also be negative eg: -10px)
    -   font-style: italic; (or normal or oblique)
    -   list-style-type: circle; (only works for lists)
        -   could also be square, lower-alpha, upper-roman
9.  CSS files can be used for multiple HTML pages and a single HTML page can have multiple CSS stylesheets.
10.  Try adding your new CSS file to other HTML files.
11.  Below is an example for the Zuko about me page:

     <img src="images/act-3/zuko-format.jpg" alt="block of formatting for Zuko" style="width:720px;">

[NEXT STEP: Using CSS to Change Layout](act-4.html){: .btn .btn-blue }
