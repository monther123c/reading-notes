1.	What does REST stand for?
REpresentational State Transfer
2.	REST APIs are designed around a resources

3.	What is an identifier of a resource? Give an example.
a URI that uniquely identifies that resource. For example, the URI for a particular customer order might be: https://adventure-works.com/orders/1
4.	What are the most common HTTP verbs?
The primary or most-commonly-used HTTP verbs (or methods, as they are properly called) are POST, GET, PUT, PATCH, and DELETE. These correspond to create, read, update, and delete (or CRUD) operations, respectively. There are a number of other verbs, too, but are utilized less frequently.
5.	What should the URIs be based on?
The URI should not rely on information that is not important to the content or the user. A common example of this is using the database ID as the URI, as in /products/23. The end user does not care that the product is database record number 23, so a URI like /products/ballpoint-pen is much better.
6.	Give an example of a good URI.
products/ballpoint-pen
7.	What does it mean to have a ‘chatty’ web API? Is this a good or a bad thing?
A chatty API, as defined by Reese, is any API that requires consumer to do more than a single call to perform a single, common operation. The details of what constitutes chatty, of course, depend on what people might reasonably want to do with the API. A good API thinks through its developer experience, providing complete, accurate, and easy-to-digest documentation. It also helps its developers by thinking through common use cases, the sort of things the real user of the API will want.
8.	What status code does a successful GET request return?
A successful GET method typically returns HTTP status code 200 (OK)
9.	What status code does an unsuccessful GET request return?
If the resource cannot be found, the method should return 404 (Not Found).
10.	What status code does a successful POST request return?
If the method does some processing but does not create a new resource, the method can return HTTP status code 200 and include the result of the operation in the response body.
11.	What status code does a successful DELETE request return?
If the delete operation is successful, the web server should respond with HTTP status code 204 (No Content), indicating that the process has been successfully handled
## Things I want to know more about
all api things is not ok with me  i will  serch more on the weekend
