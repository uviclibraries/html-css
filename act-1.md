---
layout: default
title: 1 - Getting Started
nav_order: 2
parent: Workshop Activities
customjs: http://code.jquery.com/jquery-1.4.2.min.js
---

# Getting Started With HTML

To start, we will be learning about adding basic components to an about me page like text. If you and your group have any questions, or get stuck as you work through this in-class exercise, please ask the instructor for assistance. This exercise will be for creating an about me page, it doesn’t have to be about yourself. Mine will be about Zuko, a character from a cartoon show. Have fun!

If you haven’t already, **please install [Visual Code Studio text editor](https://code.visualstudio.com/) on your computer**. You are welcome to use any text editor you like, but our workshop examples use VCS. We use this editor becasue it has some smart features that help to prevent code errors.


## Create a directory and your first HTML file

- Open VCS.
- When you open VCS for the first time you will see a "Get Started" window, which you can close.
- We are going to create a new project in VCS by clicking in the main menu on **File** > **Open Folder**. A Dialogue box will appear. 
- Navigate to your **Desktop** and then click on the **New Folder** button.
- Name your folder, or directory, `html_workshop`. 
- Once back in VCS, you will see a navigation pane on the lefthand side of the VCS window. We will use this navigation pane to create our first file.
- To the right of your directory name (html_workshop), click on the "New file" button. 

<img src="images/act-1/vcs-new-file-button.png" alt="New file button">

- You will see a text field appear below the directory name. Now, we will add our file name. 
- Name your file exactly like this: `about.html`. 
- VCS will know that this new file is an HTML file becasue you used the `.html` extension, or suffix.
- We now have our first HTML file. VCS will now be able to provide some HTML features, such as autocompletes, suggestions, and colour themse to make your code easier to read.
    <!-- <button onclick="toggle('gif1')">Show/Hide Animation</button> -->
<!-- <div id="gif1">
    <img src="images/act-1/save-as.gif" alt="save as" style="width:720px;">
    </div> -->
    - To test VCS's autocomplete feature, type the letter “**h**”. VCS has a dropdown list of suggested items, selecting one of these will autocomplete the line for you. Like autocomplete with texting, it is easy to make a mistake, so make sure you are selecting the right one. 

<img src="images/act-1/vcs-autocomplete.png" alt="autocomplete example">

## Introducing HTML "tags"

- HTML uses tags to tell the browser how to interpret text.
- HTML involves three basic components: 
    - (1) the opening tag, which has a descriptor symbol such as `h1` between two pointy brackets: `<` and `>`; 
    - (2) the closing tag, which has the same symbols as the opening tag, with a forward slash _before_ the descriptor (there are some tags that don’t need a closing bracket and these are called "self-closing" tags); 
    - (3) finally, we have the content (everything between the opening bracket and the closing bracket).

## Essential HTML 

- The HTML <!DOCTYPE> declaration is not an HTML element or tag, exactly, but an instruction that tells your browser what type of document to expect, so that your browser knows how to render it properly.
- Next, we need to tell the browser where our HTML code will go. On a new line (press the enter key) and type `<html>` (this is the "open" tag because there is no forward slash before `html`). 
- Go down to a new line and type a closed `</html>` (this is the "closed" tag because there is a forward slash before `html`).
- When the browser opens this file it now knows how to deal with what is between these tags as it’s a recognized tag. There are many kinds of tags and you’ll be introduced to some of them.
- The next part will be within our tags. Underneath the opening tag click the tab key once. Then type `<head>`. Your text editor may automatically indents tags by default. Indenting tags, especially within other tags, makes code more readable and orderly. Similarly, we want to have our closing head tag (`</head>`) indented the same amount, still in between the HTML tags. The head tag holds metadata (data about data) on our file, things like styling and  title, but we’ll get to that later.
- Next, we want to create the `<body>` tags. This is where the content of the website is held. Underneath the closing head tag, but still within the HTML tags, add an open `<body>` and closed `</body>` tag. You can also indent both of these tags. 
- Here is what your `about.html` page should look like so far: 
    
    <img src="images/act-1/vcs-basic-tags.png" alt="tag examples">

- Have you saved your file yet? Now is the time: in VCS's main menu, click on **File > Save As...** or hit **CTRL (or Command for Mac users) + S** on your keyboard.

<!-- <button onclick="toggle('gif2')">Show/Hide Animation</button> -->
<!-- <div id="gif2">
    <img src="images/act-1/save-tags.gif" alt="save present tags" style="width:720px;">
    </div> -->

### Title Tags
    
- The title tag goes within the head tag and is the title of our webpage. You may notice our current file name is `about.html`, but we want to add a different title to our page. Since it is within the head tags, we indent one space and add `<title></title>` and then add text between these two tags.
- This will always be one line, so leaving the closing tag on the same line will make it more legible than splitting it up. Between the title tags, type `About Me` and save your file.
- We will now look at our page in a browser. 
- Navigate to your **Desktop** and go into your `html_workshop` folder and click on the `about.html` file. Your `about.html` file will open in whatever browser is the default on your computer. In the following example, I have opened my file in Chrome: 

    <img src="images/act-1/view-page-title.png" alt="page title test">

Looking good! Let's move on to adding content to our `about.html` page...

### Headings Tags
    
<!-- <button onclick="toggle('gif3')">Show/Hide Animation</button>-->
<!-- <div id="gif3">
    <img src="images/act-1/h-and-p.gif" alt="h and p tags" style="width:720px;">
    </div> -->
- Let’s move on to writing code and content between the `<body></body>` tags.
- We are going to start with heaging or `<h>` tags are HTML heading tags.
- There are 6 types of heading tags: `h1`, `h2`, `h3`, `h4`, `h5`, and `h6`. Heading tags range from biggest text size, with `h1`, to the smallest text size, with `h6`.
- Heading tags are written as follows:<br>
`<h1></h1>`
- We are going to add the following heading tags (between the `<body></body>` tags) and content to our page:
`<h2>Hello, Zuko here.</h2>`<br>
`<h3>About Me</h3>`
- Here is an example of what we have, so far: 

<img src="images/act-1/first-content.png" alt="adding first content">

- As you did before, **Save** your file and open it in your browser. Be sure to [hard refresh (↪)](https://www.howtogeek.com/672607/how-to-hard-refresh-your-web-browser-to-bypass-your-cache/) your browser if you do not see the changes you expect. 
- Feel free to try different heading tags to see the differences between them.

### Paragraph Tag

- The `p` tag is used for paragraphs. 
- The content you want in a paragraph would go between the open and closed paragraph tags, as in the following example:<br>
    `<p>Your paragraph content would go here.</p>`
- We are going to add a couple of `p` tags and some content within them:<br>
        `<h2>Hello, Zuko here.</h2>`<br>
        `<p>Prince of the Fire Nation</p>`<br>
        `<h3>About Me</h3>`<br>
        `<p>Zuko is the son of the current Fire Lord of the Fire Nation, making him a prince of the fire nation. However, at 13 Zuko was scarred and subsequently banished by his father for disrespecting his authority. Zuko now roams the world searching for the Avatar as his father has deemed it the only way for Zuko to redeem himself.</p>`<br>
- <mark>Note</mark>: The paragraph content about Zuko is longer than anything we have added so far, and it could be that our text exceeds the width of the VCS window, depending on how wide you have made it on your computer. If your text is disappearing off to the right of the VCS window, we can enable "Word Wrap" so that you can always see your text, not matter what size you make your VCS window. 
  - To enable word wrap in VCS, click on **View > Word Wrap**. 
- Let's add another paragraph beneath the first paragraph:<br>
`<p>Zuko is joined on his journey for redemption by his paternal uncle, Iroh. Iroh is a retired army general, who mentors Zuko by helping him improve his fire bending and keeping him on the right path. His love of tea often gets on Zuko’s nerves.</p>`

<!-- <button onclick="toggle('gif4')">Show/Hide Animation</button>-->
<!-- <div id="gif4">
    <img src="images/act-1/end-of-6.gif" alt="body paragraph" style="width:720px;">
    </div> -->
    
### List Tags
    
- You can use HTML markup to create two kinds of lists: ordered lists and unordered lists. Use an ordered list if you want to display content in a particular order. Use an unordered list if the order of the list items does not matter. 
- Ordered lists use an `<ol>` tag and display in a browser as a numbered list. Here’s an example of an ordered list:  
> Frodo’s top three traveling essentials, in order of importance: 
> 1. The One Ring
> 2. Sting (the sword, not the musician)
> 3. Samwise Gamgee
- Unordered lists use a `<ul>` tag and display in a browser as a bulleted list. Here’s an example of an unordered list: 
> Frodo’s shopping list for Bree Market: 
> - Pipe weed
> - Craft beer
> - Even more lembas bread?
- Both ordered (`<ol>`) and unordered (`<ul>`) contain list items, which are indicated with an `<li>`, or list item, tag. 
- It is considered best markup practice to indent your `<li>` tags within the `<ol>` or `<ul>` tags. 
- In the following examples, I use unordered lists, since the list (`<li>`) items do not need to be in any particular order. Note that the lists in both examples are nested inside paragraph (`<p>`) tags. 
- I have added a list of some of Zuko's attributes on my `about.html` page. I used an unordered list, since these details are not in any particular order.
- Here is an example of what we have, so far:

<img src="images/act-1/example-page-with-list.png" alt="example page with list">

<!-- <button onclick="toggle('gif5')">Show/Hide Animation</button> -->
    
<!-- <div id="gif5">
    <img src="images/act-1/list-tag.gif" alt="list tags animated" style="width:720px;">
    </div> -->

<!-- <img src="images/act-1/list-tag.jpg" alt="list tags" style="width:720px;"> -->

### Text Tags
    
- Applying style to your HTML code should be done in CSS files, but sometimes making changes in the HTML file can be helpful. For example, the `<del></del>` and `<ins></ins>` tags can be helpful to highlight specific text. The `<del>` tag puts a line through the text and the `<ins>` tag underlines text.
- HTML tags can be put around any text that shows up in the browser. These tags don't have to encompass the whole text, it doesn't even have to cover a whole word. Say I wanted the following text to be typed out in a paragraph:
- This is <strong>important</strong>. This is <strong><ins>very</ins> important.</strong> Thank <ins>you!</ins>
    - We have 2 words in bold, 1 word underlined, and 1 word underlined and in bold. Let’s look at what that would look like in HTML, with tags: 
    -   `<p>This is <strong>important</strong>. This is <strong><ins>very</ins>important.</strong> Thank <ins>you!</ins></p>`
- Notice where the spaces and full stops are. With so many tags, it can be easy to forget to add important content in the right places.
- On your `about.html` page, play around with some of the following tags, saving your file(!), and looking at it in your browser as you go:
  - `<strong>` = important
  - `<i>` = italic
  - `<em>` = emphasized
  - `<mark>` = marked, or <mark>highlighted</mark>
  - `<small>` = smaller
  - `<sub>` = subscript
  - `<sup>` = superscript
- Remember that there is no right or wrong with our growing `about.html` page. 
- We are taking this time to play around and, often, the best learning happens when we break things! 
- Let's move on the next section in our workshop... 

<script>  

    function toggle(input) {
        var x = document.getElementById(input);
        if (x.style.display === "none") {
            x.style.display = "block";
        } else {
            x.style.display = "none";
        }
    }
</script>

[NEXT STEP: Adding Images and Links in HTML](act-2.html){: .btn .btn-blue }
