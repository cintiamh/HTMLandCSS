# Lists

## Ordered Lists

### `<ol>`

The ordered list is created with the `<ol>` element. The ordered lists use numbers.

## Unordered lists

### `<ul>`

The unordered list is created with the `<ul>` element. The unordered lists use bullet points.

### `<li>` - list item

Each item in the list is placed in a `<li>` element. Used for `<ol>` and `<ul>`.

## Definition lists

### `<dl>` - definition list

The definition list usually consists of a series of terms and their definitions. Inside the `<dl>` element
you will usually see pairs of `<dt>` and `<dd>` elements.

### `<dt>` - definition term

Contains the term being defined.

### `<dd>` - definition

Contains the definition.

Sometimes you might see a list where there are two terms used for the same definition or two different
definitions for the same term.

```html
<dl>
    <dt>Sashimi</dt>
    <dd>Sliced raw fish that is served with condiments such as shredded daikon radish or ginger root,
    wasabi and soy sauce.</dd>
    <dt>Scale</dt>
    <dd>A device used to accurately measure the weight of ingredients.</dd>
    <dd>A technique by which the scales are removed from the skin of a fish.</dd>
    <dt>Scamorze</dt>
    <dt>Scamorzo</dt>
    <dd>An Italian cheese usually made from whole cow's milk.</dd>
</dl>
```

## Nested Lists

You can put a second list inside an `<li>` element to create a sub-list or nested list.