## W5D1 AJAX and jQuery

Hey gang, great work yesterday!

We did a good review of jQuery, and you can find the notes for these in Week 4 for reference.

### HTTP

Http is the underlying way that different computers talk to each other over the internet. It works off of the basic idea:

1. I (the client) asks for information
2. You (the server) gives me information

### CRUD

CRUD stands for the four actions that we can trigger in a database:

- Create
- Read
- Update
- Delete

### AJAX

AJAX stands for Asynchronous Javascript and XML
This allows us to talk to our database and get data back without having to refresh our page

### JSON

Javascript Object Notation!
This is the format that we expect to get data back from an HTTP request:
[Here's](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Objects/JSON) a link to the MDN docs on JSON

Here's an example of JSON:

```JSON
{
 "horoscope":"lorem ipsum dolor sit amet.",
  "date":"Thursday, February 1, 2018",
  "sign":"scorpio"
}
```

### PARAMS

Short for query parameters which lets you narrow down a 'search'. These are separated by `&` in your url.

### Get Request with jQuery

To 'get' information with jQuery, we use a get request:

```JavaScript
$.get('https://myfakestocks.com/stocks?stock=AAPL&range=year', function(data) {
  console.log(data);
});
```
