# Links

## Writing links

```html
<a href="http://www.imdb.com">IMDB</a>
```

Clear link text can help visitors find what they want.

## Linking to other sites

### `<a>`

Links are created using the `<a>` element which has an attribute called `href`. The value of the `href`
 attribute is the page that you want people to go to when click on the link.
 
To link to a different website you need to use the absolute URL.

## Linking to other pages on the same site

Fot pages in the same site, you can use relative URLs. The relative URLs are shorthand version of absolute
URLs because you don't need to specify the domain name.

## Directory structure

Every page and every asset on a website has a URL (Uniform Resource Locator). The URL is made up of the
domain name followed by the path to that page or asset.

## Relative URLs

Relative URLs can be used when linking to pages within your own website.

* If all fo the files in your site are in one folder, you simply use the file name for that page.
* If your site is organized into separate directories, you need to tell the browser how to get from the page
it is currently on to the page that you are linking to.

You can use `/` to return the site's homepage and give the path relative to the root.

## Email links

### `mailto`

```html
<a href="mailto:jon@example.com">Email Jon</a>
```

When it is clicked on, the user's email program will open a new email message and address it to the 
person specified in the link.

## Opening links in a new window

### `target`

If you want a link to open in a new window, you can use the `target` attribute the value of this attribute
should be `_blank`.

```html
<a href="http://www.imdb.com" target="_blank">IMDB</a>
```

Generally you should avoid opening links in a new window. It's good to let your users know about it.

## Linking to a specific part of the same page

Before you can link to a specific part of a page, you need to identify the points in the page that the link
will got to. You do this using the id attribute.

Now we can link it to the id:

```html
<h1 id="top">Film Making Terms</h1>
<p><a href="#top">Top</a></p>
```

## Linking to a specific part of another page

As long as the page you are linking to has id attributes that identify parts of the page, you can simply 
add the same syntax to the end of the link for that page.

```html
<a href="http://www.htmlandcssbook.com/#bottom">Top of next page</a> 
```
