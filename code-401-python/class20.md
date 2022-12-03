# Django CRUD and Forms
---
Django provieds a framework that allows developers to create forms and their fields, so you can use them as objects that can be generated as HTML forms to handle and validate user interactions.

Forms are a flexible way to collect user input, as there are many widgets that can be used for entering many different data types, and in Django admin site they are mainly used for entering and modifying data in the database.
---
## HTML Forms:
A form may have any number of other input elements and their associated labels.

The form attributes define the HTTP method used to send the data and the destination of the data on the server (action):
- action: The resource/URL where data is to be sent for processing when the form is submitted. If this is not set (or set to an empty string), then the form will be submitted back to the current page URL.

- method: The HTTP method used to send the data: post or get.

---
## GET and POST

- GET and POST are the only HTTP methods to use when dealing with forms.
- Django’s login form is returned using the POST method, in which the browser bundles up the form data,
 . encodes it for transmission, sends it to the server, and then receives back its response.
- GET, by contrast, bundles the submitted data into a string, and uses this to compose a URL
 . The URL contains the address where the data must be sent, as well as the data keys and values.
- Any request that could be used to change the state of the system
- for example, a request that makes changes in the database - should use POST. GET should be used only for requests that do not affect the state of the system.
---

## Django form handling process

Django's form handling uses these techniques: the view gets a request, performs any actions required including reading data from the models, then generates and returns an HTML page (from a template, into which we pass a context containing the data to be displayed). What makes things more complicated is that the server also needs to be able to process data provided by the user, and redisplay the page if there are any errors.

