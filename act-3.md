---
layout: default
title: 3 - Adding CSS
nav_order: 4
parent: Workshop Activities
---

# Adding CSS

An introduction to CSS, adding color and a little bit of style to your web pages. If you and your group have any questions, or get stuck as you work through this in-class exercise, please ask the instructor for assistance.  Have fun!

1.  If you haven’t already completed the previous exercise, please start [here](https://richmccue.github.io/html-css/act-1.html){:target="_blank"}, as this part builds on the topics from the previous section.
2.  So far, you should have **AT LEAST? AT MOST?** two html pages, some with text and one with text and images. They all should have at least one link to another page. Even with all this lovely text your pages probably look quite plain. That’s where CSS (which stands for Cascading Style Sheets) comes into play.

    <img src="images/act-3/example.png" alt="recap of previous acts" style="width:720px;">

3.  CSS is a different language than html and has different rules and structure. It is used to alter the presentation of a website and doesn’t hold any new content to the web. This means that the same html file can appear dramatically different depending on how CSS is used.
4.  **Linking CSS Stylesheet**
    -   Let's start off by creating a separate folder inside our “html-workshop” folder called “hello-css”. This can be done in Atom by right clicking html_workshop in the project tab and clicking “New Folder”. Make a new file in Atom by right clicking on our new folder in the project tab and select “New File”. Save this file as “styling.css”.
    -   In order for a CSS file to have any effect on an html file it needs to be linked. This is done in the html file by using a link tag. Link tags are placed within the head tags and are self closing tags. Within the tag we need to have two values; rel (which stands for relation and is required for all “link” tags) and href (which behaves like the href in our “a” tags and it shows the path to the CSS file). 
<link rel = “stylesheet” href=”hello-css/styling.css”>
Save the changes to your html file.
    -   Make sure that the link tag is in the head part of the html file.
    -   Once our style sheet is linked, refreshing our html file in the browser will fetch the CSS file. To see changes save your CSS file and refresh the browser.
    -   CSS code can be used within an html file, but to keep things simple we will only use CSS code in our CSS file.
5.  **CSS Format**
    
    <img src="images/act-3/color.png" alt="CSS block" style="width:720px;">
    
    -   In the code extract above we see a snippet of CSS code. The example is called a block. It holds the changes we want to make to a specific component. Each part is explained below. Note that the colors may differ depending on the type
        -   The p in this case, is the selector. It states which elements we want to style.
        -   color in our example, is the property. It states which component of the element we want to change.
        -   blue, is the value. This is what we want to appear on the page.
        -   The open and closed curly brackets, these things {}, behave in a similar manner as the open and closed tags do in html. In the example case it states that between these brackets are all the values we want p to have.
        -   The semicolon on line 2 signifies the ending of a rule.
    -   Each block can hold multiple properties. Each property should be on its own line because it makes the block easy to read. Don’t forget to add the semicolon at the end of each rule. Let’s add the following properties:
        -   background-color:
        -   text-decoration:
    -   Your CSS file should have something like this. Save it and refresh your index.html page. You should see the changes you’ve made.
    
        <img src="images/act-3/format.png" alt="block with formatting" style="width:720px;">
    
    -   Note: Not every single color has been made available in word form. You can look up those that are available here. For colors not available, we can use its hexadecimal code. You’re probably familiar with decimal numbers: 0, 1, 2, 3, 4, 5, 6, 7, 8, and 9. Hexadecimal works the same except it has 16 unique numbers; 0, 1, 2, 3, 4, 5, 6, 7, 8, 9. A, B, C, D, E, and F. The hexadecimal numbers for colors have 6 digits, divided into three sections. 000000. The first 2 numbers represent how much red goes into the color, the middle two represents how much green is in the color, and the last 2 are how much blue. If you’re interested in playing around with hexadecimal numbers, start by replacing “blue” with “#0000FF” and you’ll get the same result. Then change the hexadecimal number as you see fit. (#000000 is black, no color, and #FFFFFF is white, all colors.)
6.  There are a lot of different properties that we can change. Each element has a selection of what can be changed, but there are many shared between elements. No one is expected to memorise all of them, but it’s good to know the main ones and the rest you can always look up. Here are a few to start playing with:
    -   font-style:
    -   font-size: (For now use px as the value, eg: 30px)
    -   Text-align:
7.  Now add more blocks for different types of tags. Here are some suggestions:
    -   body
    -   h1 (you can assign multiple tags to the same block and have a tag in multiple blocks.)
    -   a
    -   ol
    -   ul
    -   li

    <img src="images/act-3/further-format.png" alt="block with more formatting" style="width:720px;">

8.  Some properties you can change are the following:
    -   color: #012345;
    -   background-color: #6789AB;
    -   font-size: 10px;
    -   text-align: center;
        -   right
        -   left
    -   text-transform: uppercase;
        -   lowercase
        -   capitalize
    -   letter-spacing: 10px;
        -   Can be negative
    -   font-style: italic;
        -   normal
        -   oblique
    -   list-style-type: circle; (only works for lists)
        -   square
        -   lower-alpha
        -   Upper-roman
9.  CSS files can be used for multiple html pages and a single html page can have multiple CSS stylesheets.
10.  Try adding your new CSS file to other HTML files.
11.  Below is an example for the Zuko about me page:

     <img src="images/act-3/zuko-format.png" alt="block of formatting for Zuko" style="width:720px;">

[NEXT STEP: Using CSS to Change Layout](act-4.html){: .btn .btn-blue }
