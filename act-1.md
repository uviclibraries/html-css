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


1. When you open VCS for the first time you will see a "Get Started" window, which you can close.
2.  **Coding Time:**
    -   We are going to create a new project in VCS by clicking in the main menu on **File** > **Open Folder**. A Dialogue box will appear. 
    -   Navigate to your **Desktop** and then click on the **New Folder** button.
    -   Name your folder, or directory, `html_workshop`. 
    -   Once back in VCS, you will see a navigation pane on the lefthand side of the VCS window. We will use this navigation pane to create our first file.
        -   To the right of your directory name (html_workshop), click on the "New file" button. 
        -   <img src="images/act-1/vcs-new-file-button.png" alt="New file button">
        -   You will see a text field appear below the directory name. Now, we will add our file name. 
        -   Name your file exactly like this: `about.html`. 
        -   VCS will know that this new file is an HTML file becasue you used the `.html` extension, or suffix.
        -   We now have our first HTML file. VCS will now be able to provide some HTML features, such as autocompletes, suggestions, and colour themse to make your code easier to read.
    <!-- <button onclick="toggle('gif1')">Show/Hide Animation</button> -->
<!-- <div id="gif1">
    <img src="images/act-1/save-as.gif" alt="save as" style="width:720px;">
    </div> -->
   -   To test VCS's autocomplete feature, type the letter “**h**”. VCS has a dropdown list of suggested items, selecting one of these will autocomplete the line for you. Like autocomplete with texting, it is easy to make a mistake. So make sure you are selecting the right one. 
    -  <img src="images/act-1/vcs-autocomplete.png" alt="autocomplete example">
     
- Now it’s time to get to the actual coding portion.
- HTML uses tags to tell the browser how to interpret text. Tags are built with three components: (1) the opening tag, which has a descriptor symbol such as `h1` between two pointy brackets: `<` and `>`; (2) the closing bracket, which has the same symbols as the opening bracket, with a forward slash before the descriptor (there are some tags that don’t need a closing bracket. They are called self-closing tags); (3) finally, the content (everything between the opening bracket and the closing bracket).
- The first thing needed at the very top of the page is an HTML declaration: `<!DOCTYPE html>`
- This is not an HTML tag, but a "declaration" for the browser. When opened in a browser, this file it reads, or declares itself, as an HTML document. 
- Next, we need to tell the browser where our HTML code will go. On a new line (press the enter key) and type `<html>` (this is the "open" tag because there is no forward slash before `html`). 
- Go down to a new line and type a closed `</html>` (this is the "closed" tag because there is a forward slash before `html`).
- When the browser opens this file it now knows how to deal with what is between these tags as it’s a recognized tag. There are many kinds of tags and you’ll be introduced to some of them.
- The next part will be within our tags. Underneath the opening tag click the tab key once. Then type `<head>`. Your text editor may automatically indents tags by default. Indenting tags, especially within other tags, makes code more readable and orderly. Similarly, we want to have our closing head tag (`</head>`) indented the same amount, still in between the HTML tags. The head tag holds metadata (data about data) on our file, things like styling and  title, but we’ll get to that later.
- Next, we want to create the `<body>` tags. This is where the content of the website is held. Underneath the closing head tag, but still within the HTML tags, `<body>` and `</body>` should both be indented once, similar to head.
- Here is what your `about.html` page should look like so far: 
    
    <img src="images/act-1/vcs-basic-tags.png" alt="tag examples">
    
- Note that HTML is not case sensitive. You could write the body tag as **<BODY>** or even **<BoDy>** and it would work. However, it’s best practice to keep to the same pattern, so if you choose to capitalize, capitalize uniformly.
- Although our page is empty we can still open it in our browser. First thing we need to do is save the changes we’ve made. Under “**File**”, click “**Save**”. Now open the file by double clicking “**about.html**” in your “**html_workshop**” folder. This should open a browser with nothing on the page.

    <button onclick="toggle('gif2')">Show/Hide Animation</button>
    
<div id="gif2">
    <img src="images/act-1/save-tags.gif" alt="save present tags" style="width:720px;">
    </div>


5.  **Title Tag**
    
- The title tag goes within the head tag and is the title of our webpage. You may notice our current title is “about.html”, but we want to change this. Since it is within the head tags we indent one space and add `<title></title>` and then add your own text between these two tags.
- This will always be one line, so leaving the closing tag on the same line will make it more legible than splitting it up. Between the title tags, type “About Me”. Save your file and refresh your browser.

    <img src="images/act-1/example.png" alt="webpage" style="width:720px;">

6.  **Headings and Paragraph Tags**
    
    <button onclick="toggle('gif3')">Show/Hide Animation</button>
    
<div id="gif3">
    <img src="images/act-1/h-and-p.gif" alt="h and p tags" style="width:720px;">
    </div>

- Let’s move onto the body part of our code. `<h>` tags are HTML heading tags. There are 6 types: “h1”, “h2, “h3”, “h4”, “h5”, and “h6”. Inherently, h1 gives the largest text and h6 the smallest. The tags are written like so:<br>
`<h1></h1>`
- Put text within the above header tags to make a header.
- Like the title tags they can go on the same line. Don’t forget to indent from the body. I'm going to write two tags, h2 and h3:<br>
`<h2>Hello, Zuko here.</h2>`<br>
`<h3>About Me</h3>`
- See the changes you’ve made by saving and refreshing your webpage. Feel free to try different heading tags to see the difference between them and find what works best for you.
- The `p` tag is used for paragraphs. The content you want in a paragraph would go between the open and closed paragraph tags, as in the following example:<br>
    `<p>Your paragraph content would go here.</p>`
- Underneath each `h` tag, add a paragraph tag. If you are following along you can add the following in the `p` tags, if not add what is appropriate to your page:<br>
        `<h2>Hello, Zuko here.</h2>`<br>
        `<p>Prince of the Fire Nation</p>`<br>
        `<h3>About Me</h3>`<br>
        `<p>Zuko is the son of the current Fire Lord of the Fire Nation, making him a prince of the fire nation. However, at 13 Zuko was scarred and subsequently banished by his father for disrespecting his authority. Zuko now roams the world searching for the Avatar as his father has deemed it the only way for Zuko to redeem himself.</p>`<br>
    -   Atom has a helpful feature to make your file more readable. If your text exceeds the width of Atom you can compress it instead of having to scroll sideways. Under **View** click **Toggle Soft Wrap**.
    -   I’m going to add another paragraph beneath the last `p` tag. This will still be in the "about me" section. Separating items in different tags can be helpful when you want them to appear or behave in different ways when it comes to changing layout. For the Zuko page I’m adding the following:<br>
        `<p>Zuko is joined on his journey for redemption by his paternal uncle, Iroh. Iroh is a retired army general, who mentors Zuko by helping him improve his fire bending and keeping him on the right path. His love of tea often gets on Zuko’s nerves.</p>`

<button onclick="toggle('gif4')">Show/Hide Animation</button>
    
<div id="gif4">
    <img src="images/act-1/end-of-6.gif" alt="body paragraph" style="width:720px;">
    </div>
    
7.  **List Tag**
    
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
- It's best markup practice to indent your `<li>` tags within the `<ol>` or `<ul>` tags. 
- In the following examples, I use unordered lists, since the list (`<li>`) items do not need to be in any particular order. Note that the lists in both examples are nested inside paragraph (`<p>`) tags. 
- I want to add a list of attributes on my about page. I’ll make a list underneath the paragraph tags with “Prince of the Fire Nation”. I used an unordered list since these details are not in any particular order.

<button onclick="toggle('gif5')">Show/Hide Animation</button>
    
<div id="gif5">
    <img src="images/act-1/list-tag.gif" alt="list tags animated" style="width:720px;">
    </div>

    

<img src="images/act-1/list-tag.jpg" alt="list tags" style="width:720px;">

8.  **Text Tags**
    -   Applying style to your HTML code should be done in CSS files, but sometimes making changes in the HTML file can be helpful. For example, the `<del></del>` and `<ins></ins>` tags can be helpful to highlight specific text. The `<del>` tag puts a line through the text and the `<ins>` tag underlines text.
    -   HTML tags can be put around any text that shows up in the browser. These tags don't have to encompass the whole text, it doesn't even have to cover a whole word. Say I wanted the following text to be typed out in a paragraph:
    -   This is <strong>important</strong>. This is <strong><ins>very</ins> important.</strong> Thank <ins>you!</ins>
        -   We have 2 words in bold, 1 word underlined, and 1 word underlined and in bold. Let’s look at what that would look like in HTML, with tags: 
    -   `<p>This is <strong>important</strong>. This is <strong><ins>very</ins>important.</strong> Thank <ins>you!</ins></p>`
        -   Notice where the spaces and full stops are. With so many tags, it can be easy to forget to add important content in the right places.
    -   Try some more tags that alter HTML text in the following ways:
        -   `<strong>` = important
        -   `<i>` = italic
        -   `<em>` = emphasized
        -   `<mark>` = marked, or <mark>highlighted</mark>
        -   `<small>` = smaller
        -   `<sub>` = subscript
        -   `<sup>` = superscript


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
