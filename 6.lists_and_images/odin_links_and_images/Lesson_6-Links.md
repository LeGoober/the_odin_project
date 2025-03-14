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
>Through adding more attributes to the anchor elements we are then able to change the link to 'taret a new page'. By default, our anchor tags pen the webpaage on the same page.

>By adding the attribute `target="_blank"`