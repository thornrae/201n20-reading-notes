# Read: 13 Local Storage
http://diveinto.html5doctor.com/storage.html

http://diveinto.html5doctor.com/ 

What we want from local storage is: 
- a lot of storage space
- on the client 
- that persists beyond a refresh page
- and isn't transmitted to the server

HTML5 Storage (aka local storage or DOM storage) is a way for web pages to store key/value pairs locally within the client web browser. 

Similar to cookies, this data persists even after you navigate from the page or close the browser. But, unlike cookies the data is never transferred to a remote web server (though that is within the realm of possibility if that is part of your code).

We access local storage using the localStorage object in JavaScript code.

Using Local Storage: 
- store data based on a named key (use same key to retrieve)
- the named key is a string, the data can be any type of data that JS supports BUT the data is stored as a string WHICH MEANS
- use functions like parseInt() or parseFloat() to coerce your retrived data into the expected JS datatype

Treat the localStorage object as ann associative array

If you want to keep track of when the storage area changes you can trap the event.

