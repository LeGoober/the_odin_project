# Lesson 6-Understanding how to Link in HTML

The entirety of Hypertext Documents is their ability to structure documents based on the manner in which we define the tags and elements that are placed within a .html file.

We are now able link to other .html documents that are stored on the web

## Preparing on Using the Hyperlink 'Anchors' and Images
>After creating a new index page on this directory, I have provided the default VSCode HTML boilerplate code using '!', and we can then start defining the following elements to define 'Anchor' elements:
>> - these are the elements that wraps text or other HTML elements with an `<a>` tag

```html
    <!DOCTYPE html>
    <html>
        <body>
            <a href="https://www.theodinproject.com/about">About the Odin Project </a>
        </body>
    </html>
```
>By introducing the `href/hypertext reference` attribute to the HTML element, we have then added additonal information about the anchor tag that allows us to define its name and value

## Allowing our Anchor Tags to open in new tabs
>Through adding more attributes to the anchor elements we are then able to change the link to 'taret a new page' and this is done through the target attribute. By default, our anchor tags pen the webpaage on the same page and the 'href' specifies the destination link and the 'target' specified the linked resouce that will be opened.

>By adding the attribute `target="_blank"` to the element, we can then get into linking to the other documents through the name. 
```html
<body>
  <h1>Homepage</h1>
  <a href="https://www.theodinproject.com/about" target="_blank" rel="noopener noreferrer">About The Odin Project</a>

  <a href="about.html">About</a>
</body>
```
>With the 'rel' attribute it describes the relationship between the current page and the linked attribute:
 - `noopener`: ensures a link opened in a new tab won't interact/access the original page, without it JavaScipt could be used to manipulate the previous page and this poses a security risk.

 - `noreferrer`: this provides both privacy and security, as it prevents new pages from knowing where the user came from (hiding the referrer), and includes the functionality of the `noopener`, as it also prevents the new page being accessed from the original page.

>Ultimately, this serves as protection from phisiing attacks, they allows for the links used from the original page to lead users to a different one to trick them.

## 2. Absolute VS Relative Links
>Within the process of creating the hyperlinks, we would use two kinds of links:
 - links to other pages on the web,
 - linking to pages stored on our own websites

 - [Absolute Links]:
 these allow us to link to pages on the internet and are known to be absolute links, and they would typically comprise of the following parts
  - `scheme://domain/path` or `https://localhost:8080/user`

 - [Relative Links]:
 on the other hand, relative links are used as a means of locating the files that are located within the directories of our pages, and easily we could link a page called `about.html` from our `index.html` page,
 - but things to keep note is with relative links, if our files are located within our project directory we can use the `./` annotation to the link will allow our code to look for the file/directory that is relative to the current directory

 ```html
    <body>
        <h1>Homepage</h1>
        <a href="./about.html">
    </body>
 ```

I can then create a subdirectory within this project,
so that when we have various pages/directories I'd know the fundamental value of finding a page in a directory:
 ```html
    <body>
        <h1>Homepage</h1>
        <a href="./pages/about.html">
    </body>
 ```

## 3. Working with Images
Within the process of working with images, I have to note that it uses the same concept of hyperlinking the source of the resource that we want to display in our project.
> The fundamental knowledge of working with images involves:
 - displaying the image using the `<img>` element,
 - understanding parent directories,
 - using the 'alt' attribute
 - the resizing of the image elements