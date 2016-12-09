# Text

Adding markup to the text that appears on your page.

## Headings

### `<h1>`, `<h2>`, `<h3>`, `<h4>`, `<h5>`, and `<h6>`

HTML has 6 levels of headings. `<h1>` is used for main headings, it will usually be bigger.

## Paragraphs

### `<p>`

By default, the browser will show each paragraph on a new line with some space around.

## Bold and Italic

### `<b>`

This tag will show the text in bold. No meaning associated with its content.

### `<i>`

This tag will show the text in italic.

## Superscript and Subscript

### `<sup>`

The `<sup>` element is used to contain characters that should be superscript.

### `<sub>`

The `<sub>` element is used to contain characters that should be subscript.

```html
<p>On the 4<sup>th</sup> of September you will learn about E=MC<sup>2</sup>.</p>
<p>The amount of CO<sub>2</sub> in the atmosphere grew by 2ppm in 2009<sub>1</sub>.</p>
```

## White Space

White space collapsing - When the browser comes across two or more spaces next to each other, 
it only displays one space. It also treats a line break as a single space.

## Line breaks and horizontal rules

### `<br />`

This is used to add a break line, without any extra space.

### `<hr />`

This is used to create a break between themes. This adds a horizontal rule between sections.

## Semantic markup

Semantic markups are not intended to affect the structure of the web page, but it adds extra information.

These markups should not be used to change the way the text looks; their purpose is to describe the 
content of the page more accurately.

These are very useful for tools like screen readers.

## Strong and Emphasis

### `<strong>`

Is used to indicate the content has strong importance. By default, browsers will show the contents of 
`<strong>` element in bold.

### `<em>`

Is used to indicate emphasis that subtly changes the meaning of a sentence. By default, browsers will show
the contents of `<em>` element in italic.

## Quotations

### `<blockquote>`

Is used for longer quotes that take up an entire paragraph. Note that the `<p>` element is still used 
inside the `<blockquote>` element. Browsers tend to indent the contents of `<blockquote>` element.

### `<q>`

Is used for shorter quotes that sit within a paragraph. Browsers are supposed to put quotes around the 
`<q>` element, however IE does not.
 
Both elements may use the `cite` attribute to indicate where the quote is from (the value is the URL of 
the source).

```html
<blockquote cite="https://en.wikipedia.org/wiki/Winnie-the-Pooh">
    <p>Did you ever stop to think, and forget to start again?</p>
</blockquote>
<p>As A.A. Milne said. <q>Some people talk to animals. Not many listen 
though. That's the problem.</q></p>
```

## Abbreviations and Acronyms

### `<abbr>`

Used for abbreviations and acronyms. A `title` attribute is used to specify the full term.

```html
<p><abbr title="Professor">Prof</abbr> Stephen Hawking is a theoretical physicist and cosmologist.</p>
<p><abbr title="National Aeronautics and Space Administration">NASA</abbr> do some crazy space stuff.</p>
```

## Citations and Definitions

### `<cite>`

When referencing a piece of work such as a book, film or research paper, use the `<cite>` element to 
indicate where the citation is from.

### `<dfn>`

The first time you explain some new terminology in a document, it is known as the defining instance of it.

`<dfn>` is used to indicate the defining instance of a new term.

## Author details

### `<address>`

Contains the contact details for the author of the page.

It can contains the physical address, phone number, or e-mail address.

```html
<address>
    <p><a href="mailto:homer@example.org">homer@example.org</a></p>
    <p>742 Evergreen Terrace, Springfield</p>
</address>
```

## Changes to content

### `<ins>`

Shows content that has been inserted into a document. This is usually shown as underlined.

### `<del>`

Shows content that has been deleted from a document. This is usually shown lined through.

### `<s>`

Shows content that is no longer accurate or relevant (but should not be deleted). This is usually shown
with a line through.
