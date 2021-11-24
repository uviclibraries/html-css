---
layout: default
title: 4 - Changing Layout
nav_order: 5
parent: Workshop Activities
---

# Using CSS to Change Layout

Using CSS to change the positioning and layout of your page. If you and your group have any questions, or get stuck as you work through this in-class exercise, please ask the instructor for assistance.  Have fun!

1.  If you haven’t already completed the previous exercise, please start [here](https://richmccue.github.io/html-css/act-1.html){:target="_blank"}, as this part builds on the topics from the previous section.
2.  Let’s recap what we’ve gone through thus far.
    -   Create html pages
    -   Add headings, text and lists
    -   Have images on our pages
    -   Links to other pages on our site and links to other sites
    -   Link a css stylesheet
    -   Add some css styling
    Your page should look something like this:
    
    <img src="/images/act-4/example.png" alt="recap of activities" style="width:720px;">
    
3.  You may have noticed that all of our content is stacked like a list. This is the default layout of html files. Although our information is clear and orderly, it is also static and not very exciting. Flex boxes can be used to arrange content in a simple way.
4.  **CSS and Classes**
    -   Classes can be used in CSS to define specific html tags and alter properties and values for elements for that specific class.
    -   On the Zuko about page I want to increase the size of text in my paragraph tags. However, I want my upper paragraph tag to be a different size than my other paragraph tags.
    -   In the html file, I can give a tag a class. This class can then be referred to as its own block in the CSS file.
    -   I'm going to add a class to my top paragraph tag as follows:<br>
        **&lt;p class=”about-title”&gt;**Hello, Zuko here**&lt;/p&gt;**
    -   In CSS, class blocks are written with a full stop in front of them.
        
	```
	    .about-title{
	        font-size:150%;
	        Font-weight: bold;
            }
	```
	
    -   Notice how only the paragraph with the “about-title” class has been affected by the changes.
    -   You may have the same property in the class block and the tag block with different values. This is where precedence comes into play. Whichever block has higher precedence is the value the browser will assign. A simple way to think about it is the more specific the selector the higher the precedence.

        <img src="/images/act-4/css-class.png" alt="css class" style="width:720px;">

5.  **HTML and Divisions**
    -   The “div” tag, written in html as **<div></div>**, stands for division. All it does is defines sections within our code. Alone, it doesn’t do much. However, with CSS it helps organize our content into groups
    -   By applying a class to division tags we can change a section of code that can apply to everything between the opening and closing tag.
    -   In the Zuko example I’ve added a div class to my nested list. This way, I can change the items in my list without affecting the main list or even other lists I may have.
    -   The top image is from the html code and the bottom is the corresponding CSS code. The text is now bold and not italicized.
    
        <img src="/images/act-4/div.png" alt="div example" style="width:720px;">
    
    -   Division tags can also take advantage of precedence, A division tag enclosed within another division tag has higher precedence than the outside division tag.
6.  **CSS Flexible Boxes**
    -   Despite all the changes we’ve made, nothing has really moved around yet. This is where flexible boxes or flexbox comes in.
    -   Flexbox is a simple and powerful way to organize a webpage.
    -   Flexbox works by separating each item into their own box. These boxes can then be told how to behave and organize themselves even when viewed from different screen sizes (think a computer screen compared to a smartphone screen).
    -   HTML defaults to listing everything, one below the other. Like so:
    -   Let's start by adding a flex container to our body tag in CSS.
        
	    <img src="/images/act-4/flex.png" alt="flex container" style="width:720px;">
	
	Add the following in your CSS file: 
        ```
	    body{
	        display: flex;
            }
	```
    -   Refresh your html page and you should get each item line up horizontally.
    
        <img src="/images/act-4/flex2.png" alt="more flex containers" style="width:720px;">
    
    -   I don’t want my page to look like this either. Here is where I can use division tags to organize it further. First get rid of the display:flex in we just added in our body tag.
    -   I want my list to be horizontal to the image of Zuko. I’m going to add my opening divisions tag above the image tag and the closing division tag below the closing unordered list tag. Make the opening division tag look like this:<br>
	**&lt;div class = “bio”&gt;**
        -   Note: You can highlight everything between the opening and closing division tags and click the tab key. This indents all the highlighted items, helping to keep you code legible. Holding the shift key then clicking the tab key does the opposite and moves the text closer to the margin.
    -   Go to your CSS file and create a block for the bio class and add the display flex property.
        ```
	    .bio{
                display:flex;
            }
	```
    -   Your list should now be to the right of the image of Zuko!
    -   If you’d like to have the list on the left, there are a few ways to do this.
        -   Move the list in your html code to be above the image tag.
        -   Use the flex-direction property in CSS. Flex direction changes the order the items are displayed in. Check out how it works by adding the following to the bio block in your CSS file. 
        <flex-direction: row-reverse;>
    -   Where flex boxes can start to get complicated is with nested flex boxes. It is important to plan out how you want your content laid out. This way when adding your division tags, you know where the opening and closing tags should be.
7.  There are many different ways to manipulate flex boxes with built in properties. [Here](https://www.google.com/url?q=https://www.w3schools.com/css/css3_flexbox_container.asp&sa=D&source=editors&ust=1637785562991000&usg=AOvVaw0dVdgDERpGsMzoVn0GAyuI){:target="_blank"} and [here](https://www.google.com/url?q=https://css-tricks.com/snippets/css/a-guide-to-flexbox/&sa=D&source=editors&ust=1637785562991000&usg=AOvVaw2yQ3MsixSAmSJrJtymwNpw){:target="_blank"} are helpful pages on flex properties. The following is a list of a few you can try to add.
    -   flex-direction: (row / column / row-reversed / column-reversed);
        -   This affects how the boxes are organized. If you’d like them to stack vertically, use the value: column;
        -   Note: column-reverse & row-reverse but using them is not advised as it may cause a conflict with how you indent your page to be viewed and how users utilizing assistive technology view your page.
    -   flex-wrap: (wrap / nowrap);
        -   Should your flexbox items extend past the width of the page and you do not want users to side scroll, wrap will stack the following content below. In the example below, without wrap the purple item would be off of the display screen (orange box). With wrap, the purple box goes down

            <img src="/images/act-4/flex3.png" alt="flex container wrap" style="width:720px;">

    -   [justify-content](https://css-tricks.com/almanac/properties/j/justify-content/#:~:text=The%20justify%2Dcontent%20property%20is,have%20reached%20their%20maximum%20size.){:target="_blank"}: (flex-start(default) / flex-end / center / space-between / space-around);
        -   This property changes how the flex boxes are spaced between other flexboxes. This can be a fun one to play around with as it can dramatically change the layout of a page.
    -   [align-items](https://css-tricks.com/almanac/properties/a/align-items/){:target="_blank"}: (flex-start / flex-end / center / stretch);
        -   This property dictates how flex boxes are aligned vertically. Flex-start makes them all start at the top, flex-end makes them all end at the bottom, center makes their center sit in the center, stretch forces all items to cover the entirety of the flex box.
        -   For having items in the center of your flex box, apply both of the following:
            -   justify-content : center;
            -   align-items : center;

[NEXT STEP: Next Steps](act-5.html){: .btn .btn-blue }
