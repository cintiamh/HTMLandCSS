# Images

## Choosing images for your site

Images should:

* Be relevant
* Convey information
* Convey the right mood
* Be instantly recognisable
* Fit the color palette

### Stock Photos

There are companies that sell stock images (images you pay to use).

* http://www.istockphoto.com/
* http://www.gettyimages.com/
* http://www.freeimages.com/
* https://us.fotolia.com/

## Storing images on your site

It's a good practice to keep all images in a separated folder.

## Adding images

### `<img>`

Use `<img>` element to add an image into the page.

#### `src`

This can be a relative URL pointing to an image on your own site or an external URL.

#### `alt`

The alt text provides a text description for the image, it is the fallback text for 
the image and will also be used by screen readers.

#### `title`

Most browsers will display the content of `title` in a tooltip when the user hovers 
over the image.

#### `height`

Image height in pixels.

#### `width`

Image width in pixels.

It is a good idea to specify the image size so when loading the page you don't have the
jump in size. You can also specify the image size using CSS.


#### `align` (old code)

The `align` attribute is not used in HTML5. It was used to indicate how the page should
flow around the image. Possible values are `right` or `left` for horizontal and `top`, 
`middle` or `bottom` for vertical alignment.

You can get the same effect nowadays using CSS `float` property.

## Three rules for creating images

### 1. Save images in the right format

jpeg, gif or png.

### 2. Save images at the right size
 
If the image size is smaller, it can get distorted and streched, if bigger, it can take
longer than necessary to load.

### 3. Use the correct resolution

Most computers: 72 pixels per inch. If bigger, it can take longer to load.

## Tools to edit and save images

### Online Editors

* http://www.photoshop.com/
* https://pixlr.com/
* http://ipiccy.com/

Whenever you have many different colors in a picture you should use a JPEG.

Use GIF or PNG format when saving images with few colors or large areas of the same color.

When a picture has an area that is filled with exactly the same color, it is known as
flat color.

## Image dimensions

It's ok to reduce the image size, but increasing the size of photos affects the image
quality.

## Cropping images

Cropping images can make you loose valuable information.

## Image resolution

Desired resolution: 72 ppi.

JPGs, GIFs, and PNGs have bitmap format.

## Vector images

Vector images differ from bitmap images and are resolution-independent.

Tool: Adobe Illustrator.

Scalable Vector Graphics (SVG) are a relatively new format used to display vector images
directly on the web.

## Animated GIFs

Animated GIFs show several frames of an image in sequence and therefore can be used to
create simple animations.

Tool: Adobe Photoshop, some online tools.

## Transparency

### Transparent GIF

For images with straight edges and 100% transparent.

### PNG

For images with diagonal or rounded edges, or semi-opaque transparency, or drop shadow.

## HTML5: Figure and Figure Caption

### `<figure>`

HTML5 introduced the `<figure>` element to contain images and their caption so that the
two are associated.

You can have more than one image inside the `<figure>` element as long as they all 
share the same caption.

### `<figcaption>`

Adds caption to an image.

```html
<figure>
    <img src="http://static.tvtropes.org/pmwiki/pub/images/Hello_Kitty_Pink_2981.jpg" alt="Hello Kitty">
    <figcaption>This is just an image with Hello Kitty.</figcaption>
</figure>
```

Older browsers that do not understand HTML5 elements simply ignore the new elements and 
display the content of them.
