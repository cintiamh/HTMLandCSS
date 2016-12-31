# Tables

## What's a table?

A table represents information in a grid format.

Each block in the grid is referred to as table cell.

## Basic Table structure

### `<table>`

The contents of the table are written row by row.

### `<tr>`

The Table row.

### `<td>`

The table cell (table data).

## Table headings

### `<th>`

`<th>` is used just like `<td>`, but represents the heading for either a column or a row.

Even if the cell has no content, you should always have a empty `<th>` or `<td>`.

#### `scope`

This attribute works with `<th>` element to indicate whether it is a heading for a colomn or a row.

Possible values: `row` or `col`.

## Spanning columns - `colspan`

The `colspan` attribute can be used on `<td>` and `<th>`.

```html
<table>
    <tr>
        <th></th>
        <th>9am</th>
        <th>10am</th>
        <th>11am</th>
        <th>12am</th>
    </tr>
    <tr>
        <th>Monday</th>
        <td colspan="2">Geography</td>
        <td>Math</td>
        <td>Art</td>
    </tr>
    <tr>
        <th>Tuesday</th>
        <td colspan="3">Gym</td>
        <td>Home Ec</td>
    </tr>
</table>
```

## Spanning Rows - `rowspan`

The `rowspan` attribute can be used on `<td>` and `<th>`.

```html
<table>
    <tr>
        <th></th>
        <th>ABC</th>
        <th>BBC</th>
        <th>CNN</th>
    </tr>
    <tr>
        <th>6pm - 7pm</th>
        <td rowspan="2">Movie</td>
        <td>Comedy</td>
        <td>News</td>
    </tr>
    <tr>
        <th>7pm - 8pm</th>
        <td>Sport</td>
        <td>Current Affairs</td>
    </tr>
</table>
```

## Long Tables

If you have a table that is taller than the screen, then the browser can keep the header and footer visible
whilst the contents of the table scroll.

### `thead`

The headings of the table should sit inside `<thead>` element.

### `<tbody>`

The body should sit inside the `<tbody>` element.

### `<tfoot>`

The footer belongs inside the `<tfoot>` element.

```html
<table>
    <thead>
    <tr>
        <th>Date</th>
        <th>Income</th>
        <th>Expenditure</th>
    </tr>
    </thead>
    <tbody>
    <tr>
        <td>1st January</td>
        <td>250</td>
        <td>36</td>
    </tr>
    </tbody>
    <tfoot>
    <tr>
        <td></td>
        <td>250</td>
        <td>36</td>
    </tr>
    </tfoot>
</table>
```

## Old code

All of these attributes have been replaced by the use of CSS.

* `width` - can be used for `<table>`, `<th>`, and `<td>`.
* `cellpadding` - adds space inside each cell of the table.
* `cellspacing` - creates space between each cell of the table.
* `border` - indicates the width of the border in pixels.
* `bgcolor` - indicates the background color.
