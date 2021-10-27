# WEEK-4 HOMEWORK

This week your task is to create a multi-page website with an html structure using the appropriate semantic elements, then style your page using advanced css methods.
This site can be about any subject and can contain 'dummy' text (search lorem ipsum) and placeholder images (try https://placekitten.com/200/400).



## Multiple Pages

This site should contain at least 3 pages that can be navigated to using some kind of navbar.
To simplify the design / development: each page can have the same structure and use the same css file. The link or button that relates to the current page should be styled differently than the rest of the links. For example: If the user is on the home page, the home button should stand out in some way



## File Structure

When creating a large site with multiple pages, you should think ahead when creating the file structure. This can help you to stay organized later on.

For example:

```
> my-project-folder
    > css
        > style.css     (used for all pages usually)
        > section.css   (optional - used to style something more specific)
    > html
        > index.html    (the home page)
        > page-2.html
        > page-3.html
    > images            (optional location for saved images)
        > image-1.jpg
```


## Semantic Elements

Using semantic elements correctly guarantees that search engine crawlers can see and read your sites content, links, and headings which scores higher in search engine results

Your site should contain at least the following semantic elements:

ELEMENT                 | PURPOSE 
-|-
html                    | always used to contain the entire page
head                    | used to contain meta-data about the page
body                    | always used to contain the content of the page
nav                     | used to contain the navigation elements
main                    | should contain most content
footer                  | used to contain site-map, site info, extra links, etc.
a                       | link tags, used for navigation or external links
p                       | paragraph tags - used for text content
h1, h2, h3, ...         | headings - used to describe the entire section
img                     | image tags are used for displaying any images



## Custom Elements

Custom elements are not useful to search engines, but allow creators more control over the style and appearance of the site / elements

Your site should contain at least 3 non-semantic elements, each one styled seperately using your css file.

For example: 

```
<div id="myCustomElementOne"> ... some text or content ... </div>
```



## Responsive Design

Your site should take advantage of css media-queried to structure or style the page differently depending on the screen size - mobile/desktop. The best approach is to design for mobile devices first, then use a media query to style pages for larger screens. This is called 'mobile-first design'.

For example: 

```
/* The original styles are for small screens ---------- */
.myElements{
    width: 100%
}

/* Use media-queries for larger devices --------------- */
@media only screen and (min-width(800px)){
    .myElements{
        width: 30%
    }
}
```

Your site should contain at least one 'flex-box' for containing any content.
Flex-boxes are useful for changing the structure of content depending on the available space.

For example:

```
<div class='flexContainer'>
    <div>Flex Child One</div>
    <div>Flex Child Two</div>
    <div>Flex Child Three</div>
</div>
```



## Advanced CSS

When creating a large site, you may use colors or values many times throughout a css file and it can be difficult to find and change each value, you should define css variables so that it is easy to make theme changes later on. 

For example:

```
  /* The ':root{} selector should be placed at the top of your css file */
  /* declare a variable with `--` syntax */

:root {
  --dark: #13293d;
  --light: #fff;
  --navlink-color: #b9c6ae;
}

```

There are many ways to create interesting graphics on a page using css. You should use the following css properties to style your page in some way.

PROPERTY                | PURPOSE 
-|-
transform: skew()       | used to skew images or shapes
clip-path               | used to shape an image or object based on a path



## Requirements

- Website with at least 3 pages
- A navbar for switching pages
- Proper semantic structure
- An external CSS file
- CSS variables
- media queries
- some usage of transform / clip-path



## Extra

- Try adding and using a 'video' or 'audio' tag to a page in your site
- Experiment with flex-boxes and their different methods of alignment and spacing.
- Experiment with css transforms on some images or text content
- Use a script element on one of your pages to write some javascript and send an 'alert' to the user, 'log' to the console, or change the color of an element when a button is clicked.