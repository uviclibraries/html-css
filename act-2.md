---
layout: default
title: 2 - Adding Images & Links
nav_order: 3
parent: Workshop Activities
---

# Adding Images and Links in HTML

### Before we begin...

If you haven’t already completed the first exercise, please go to [Getting Started With HTML](https://uviclibraries.github.io/html-css/act-1.html).

### Next steps: images and links!

Next, we’ll learn how to add images and links to an HTML page. If you or your group have any questions, or you get stuck as you work through this in-class exercise, please ask the instructor for assistance. Have fun!

If you completed the [Getting Started With HTML](https://uviclibraries.github.io/html-css/act-1.html) exercises, you should have an **"about.html"** page with some paragraphs, headers, and a list.

You may have added some additional content and HTML markup as well, and that's encouraged because we're here to tinker!

**Your "about.html" document should look something like this:**

<img src="images/act-2/recap.png" alt="recap of act 1" style="width:720px;">

## Adding Images

1.  **Create a folder called "images" in your “html_workshop” folder.**
    -   In your **“html_workshop”** folder create another folder called **“images”**. You can do this in Atom by right-clicking the "**Project**" tab and selecting “**New Folder**” and naming it within Atom.
    -   You can find an image on the Internet or right-click with your mouse or trackpad on the image below, and then save it to the **"images"** folder.

<img src="images/act-2/zuko.png" alt="zuko" style="width:720px;">

2. **Get to know the image `<img>` tag.**
    - `<img>` is the tag used to show images on an HTML webpage. Notice that there is no closing, or forward slash, in this tag. This is because `<img>` is what's called a self-closing tag, or a [void element (↪)](https://html.spec.whatwg.org/multipage/syntax.html#elements-2). You may see it written as `<img/>` to show that it is self-closing, but this is just for human readability. Both `<img>` and `<img/>` are valid, so the important thing is to keep it consistent.
3. **Add an `<img>` tag to your HTML page.**
    - Somewhere between the `<body></body>` tags, add `<img src="image.jpg" alt="image description">`.
    - **`src`** means "source," or the location your HTML browser will look to display the image. My image, “avaZuko.png”, is stored in the "images" folder. Between the quotation marks we put the filepath to our image file, which creates a link between our image and our HTML webpage. The path in my case is “images/avaZuko.png”. If you used another image file, then you would replace "avaZuko.png" with your file's name. **Note** that if we ever move our image file to another folder we would break the link between the image and our HTML page.
    - **`alt`** means "alternate text" for an image, if the image cannot be displayed. What you put between the quotation marks will be displayed when the image fails to load. This text is also used by people who may have visual disabilities, who use [screen reader software (↪)](https://www.cnib.ca/en/screen-readers?region=bc).
4. **Add your filepath and alternate text to your `<img>` tag.**
    - When you have added your filepath and alternate text, you should have an `<img>` tag that looks something like this: **`<img src="images/avaZuko.png" alt="Zuko headshot with a frowning expression">`**.

        <img src="images/act-2/img.jpg" alt="image tag" style="width:720px;">

    - **Note** that my image is saved as a .png file but `<img>` accepts various types, the most common other ones being .jpeg (or .jpg), .svg, and .gif.
5. **Save your HTML file and refresh your browser to see the changes.**

    - Just for practice, try adding another image to your page. You can use the fire nation image below if you don't have any images of your own.

        <img src="images/act-2/fire.png" alt="fire nation logo" style="width:720px;">

## Adding Links

### Get to know the `<a>` hyperlink tag
Here is an example of a complete [hyperlink tag (↪)](https://www.w3schools.com/tags/tag_a.asp) for an Internet URL (Uniform Resource Locator) web address: `<a href="https://www.wikipedia.org/">Wikipedia</a>`.

The content between the open and closed `<a>` tags will appear as a clickable link in your browser. In the example given, the word "Wikipedia" would appear as the clickable hyperlinked text.

The `<a>` in the hyperlink tag defines it as a hyperlink element, and the `href` is the attribute that indicates the link's destination.

**Hyperlinks come in many flavours. Here are the basic four:**
  - **"anchor links"**, or hashtag links, "jump" you to locations in the same webpage, or document. These are helpful in pages with a lot of text. You can, for example create a table of contents at the top of your HTML page that jumps to sections (or text) within that same page. **Example: `<a href="#anchor-location">clickable text</a>`**.
  - **"external links"** link you to other locations outside of your directory, such as other webpages or websites. These links always use the full URL. **Example: `<a href = http://www.wordpress.com/my-webpage.html>clickable text</a>`**.
  - **"email links"** link you to an email address. When you click on these, they tell your computer to open up whatever email program you are using. **Example: `<a href="mailto:some-email@yoursite.com">Email me</a>`**.

### Add one or more hyperlinks to your HTML page

To get a feel for how hyperlinks work, **choose one or more of the following examples to add to your "about.html" page.**

#### 1. Anchor link

This type of link jumps us to another place in the same page.

1. **Add some placeholder text of some kind** to one of your "about.html" page. You can type a few paragraphs on your own, or use placeholder text called [_lorem ipsum_ (↪)](https://en.wikipedia.org/wiki/Lorem_ipsum), which is often used by web developers for creating website examples. People like to have fun inventing their own versions of _lorem ipsum_, and my current favourite is [_The Lord of The Rings_ _lorem ipsum_ generator (↪)](https://ceheiss.github.io/LordOfTheIpsum/).
2. **Wrap a selection of text in a header tag of your choice and give it a unique `id`.** Think of this as your named anchor. The `<a>` link we eventually create will link to this unique `id` anchor. In my example, I have wrapped the heading text of "Bilbo's speech to the Council" in an `h2` tag and assigned it a unique `id` of "bilbo-speech":

>`<h2 id="bilbo-speech">Bilbo's speech to the Council</h>`
>`<p>I used to think that they were things the wonderful folk of the stories went out and looked for, because they wanted them, because they were exciting and life was a bit dull, a kind of a sport, as you might say. But that’s not the way of it with the tales that really mattered, or the ones that stay in the mind. Folk seem to have been just landed in them, usually their paths were laid that way, as you put it.</p>`

 **Note** that each anchor has to have a unique name. In my example, the anchor's `id` is "bilbo-speech". Any additional anchor on this same page would need to have a diffrent name. For example, if I wanted to link to another of Bilbo's speeches, I would change that anchor's `id` to something like "bilbo-speech-2". 
 
3. **Create an `<a>` link to your anchor's unique `id`**. This will be the clickable link that jumps you to the unique `id` you just created. You can add this link anywhere on the HTML page, but to pretend we are making a table of contents, please add your link toward the top of your HTML page, but within the `<body></body>` tags. What we are doing in my example is making my `h2` become a link that jumps us to the heading of "Bilbo's speech to the Council." Here is what my link looks like:

>`<h2 href="#bilbo-speech">Read Bilbo's speech to the Council</h2>`

4. **Save your HTML file** and look at it again, after you refresh your browser, to see if your anchor link works. In my example, the text of "Read Bilbo's speech to the Council" now jumps me to start of Biblo's speech.

**For more practice with anchor links, try [this W3Schools test-space (↪)](https://www.w3schools.com/tags/tryit.asp?filename=tryhtml5_a_href_anchor).**

#### 2. Internal link

This type of link jumps us to another HTML page in our directory. So, **we need to create another HTML page to jump to.**

1. **In your "html_workshop" folder, create a new HTML page called "index.html"**. This is the file to where we are going to link from our **"about.html"** page. If you are using Atom, choose **"File"** and select **“New File."** Once saved you should see the **"index.html"** file appear in Atom's project tab, on the left of the Atom window.

<img src="images/act-2/links.gif" alt="adding links animated" style="width:720px;">

<img src="images/act-2/links.jpg" alt="adding links" style="width:720px;">

As with any new HTML page, we need to add at least `<!DOCTYPE html>` at the top of the page and some other tags to get us started. **Copy/paste the following into your "index.html" page (and be sure save the file afterwards):**  

 ```
<!DOCTYPE html>
<html>
<head>
    <title>Your page title here</title>
</head>
  <body>
    <h1>Your heading here</h1>
    <p>Your paragraph of text here.</p>
  </body>
</html>

```

2. **Go back to your "about.html" page and add an internal link to your "index.html" file.** In your **"about.html"** file, select some text to turn into a link and wrap that text in the following tags:

`<a href="index.html">your link text here</a>`

We only need to link to another location within the same directory, so notice that we do not need to add the full URL, as in the `https://www` part. We only add the file name between the quotation marks.

In my example, I want my readers to know that I have another webpage on my website that they can read:

`Be sure to check out <a href="index.html">my Index page</a> for more reading!`

3. **Save your "about.html" file** and refresh your browser to see if your new link works.

#### 3. External link

This type of link takes you to somewhere outside of your website, to another website or webpage on the Internet. The process to create an external link is identical to an internal link, except that the external link requires a full URL, the whole `https://www` part. This type of full URL is known as an ["absolute" URL (↪)](https://www.w3schools.com/tags/att_link_href.asp).  

1. **In either your "index.html" or "about.html" file, choose some text to turn into a link.**
2. **Wrap your selection of text in the following tags:**

 `<a href="your web URL here">your link text here</a>`

3. **Add your full URL between the quotation marks,** which includes the whole `https://www` part. **Make sure that you do not add any accidental spaces before or after your URL.** Here's my example:

`<a href="https://www.w3schools.com/tags/att_a_href.asp">your link text here</a>`

4. **Save your HTML file** and refresh your browser to see if your new link works.

🎉 **Congratulations!** You now know how to add images and links to a webpage!

[NEXT STEP: Adding CSS](act-3.html)
