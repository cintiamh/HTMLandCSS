# Forms

## Form Controls

### Adding text

* Text input (single-line)
* Password input
* Text area (multi-line)

### Making choices

* Radio buttons
* Checkboxes
* Drop-down boxes

### Submitting forms

* Submit buttons
* Image buttons

### Uploading files

* File upload

## How forms work

A user fills in a form and then press a button to submit the information to the server.

A form may have several form controls. To differentiate between various pieces of inputed data, information
is sent from the browser to the server using name/value pairs.

## Form structure

### `<form>` element

Form controls live inside a `<form>` element. This element should always carry the `action` attribute and 
will usually have an `id` attribute.

### `action` attribute

The `action` value is the URL for the page on the server that will receive the information in the form when
it is submitted.

### `method` attribute

Possible values: (the default value is `get`)

* `get` : this method add the form values to the end of the URL in `action`. 
* `post` : this method send the form values in HTTP headers. This method is most used (it's safer). 

### `id` attribute

The `id` attribute is important in forms to identify it inside the page, for input validation and such.

```html
<form action="http://www.example.com/subscribe.php" method="get"></form>
```

## Text input

### `<input type="text">` element

Use the `<input>` element with the `type` set to `text`.

### `name` attribute

The name attribute will used to identify the form control when the information is sent to the server with its value.

### `maxlength` attribute

This will limit the number of characters a user may enter into the text field.

### `size` attribute (deprecated)

This attribute will adjust the input width to accommodate the specified number of characters. You should use CSS instead.

```html
Username: <input type="text" name="username" size="15" maxlength="30" />
```

## Password input

### `<input type="password>` element

Use the `<input>` element with the `type` set to `password`. This will show blocked characters instead of what the user 
is actually typing.

### `name` attribute

The name attribute will used to identify the form control when the information is sent to the server with its value.

### `maxlength` attribute

This will limit the number of characters a user may enter into the field.

### `size` attribute (deprecated)

This attribute will adjust the input width to accommodate the specified number of characters. You should use CSS instead.

```html
Password: <input type="password" name="username" size="15" maxlength="30" />
```

## Text Area

### `<textarea>` element

The text area creates a multi-line text input. This is not an empty element, it needs a opening and a closing tag.

Any text in between the opening and closing tags will appear in the text box when the page loads.

You might find older code that uses `cols` and `rows` attributes to define the `textarea`'s width and height. You
should prefer to do it with CSS.

### `name` attribute

The name attribute will used to identify the form control when the information is sent to the server with its value.

```html
Some comments:
<textarea name="comments" cols="20" rows="4">
    Enter your comments...
</textarea>
```

## Radio Button

### `<input type="radio">` element

Use the `<input>` element with the `type` attribute set to `radio`. Radio buttons allows users to pick just one of a 
number of options.

### `name` attribute

The `name` attribute will used to identify the form control when the information is sent to the server with its value.
When you have multiple options for a specific question, you should set the same `name` for all options.

### `value` attribute

The value that is sent to the server in case the field in question is checked.

### `checked` attribute

You can force one of the options to be set before the user chooses, like the default value. Once one option in a radio
button group is selected, there is no way to unselect it. There is always one option selected.

```html
Favorite Genre:
<input type="radio" name="genre" value="rock" checked="checked" /> Rock
<input type="radio" name="genre" value="pop" checked="checked" /> Pop
<input type="radio" name="genre" value="jazz" checked="checked" /> Jazz
```

## Checkbox

### `<input type="checkbox">` element

Use the `<input>` element with the `type` attribute set to `checkbox`. You can choose multiple or none of the options 
with checkbox.

### `name` attribute

The `name` attribute will used to identify the form control when the information is sent to the server with its value.
When you have multiple options for a specific question, you should set the same `name` for all options.

### `value` attribute

The value that is sent to the server in case the field in question is checked.

### `checked` attribute

This will show the box checked when the page loads.

```html
Favorite music services:
<input type="checkbox" name="service" value="itunes" checked="checked" /> iTunes
<input type="checkbox" name="service" value="lastfm" /> Last.fm
<input type="checkbox" name="service" value="spotify" /> Spotify
```

## Drop down list box

### `<select>` element

The `<select>` element is used to create a drop down list box containing two or more `<option>` elements.

### `name` attribute

The `name` attribute will used to identify the form control when the information is sent to the server with its value.

### `<option>` element

The `<option>` element is used to specify the options to select from. The string between the open and close tags will 
be shown.

### `value` attribute

The `value` attribute associated with the `<option>` tag. The `value` is sent to the server associated with the 
`<select>` 's `name`.

### `selected` attribute

The `selected` attribute set to `selected` string can be used in the `<option>` tag that should be selected when the 
page loads. If no `<option>` is set to `selected`, the first option is set by default.

```html
What device do you use to listen to music?
<select name="devices">
    <option value="ipod">iPod</option>
    <option value="radio">Radio</option>
    <option value="computer" selected="selected">Computer</option>
</select>
```
