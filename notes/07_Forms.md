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