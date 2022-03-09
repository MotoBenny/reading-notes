class-13.md

## **Table Of Contents**

Read: 13 - Local Storage

Reading

[“The Past, Present, and Future of Local Storage for Web Applications”](http://diveinto.html5doctor.com/storage.html)

## **“The Past, Present, and Future of Local Storage for Web Applications”**

- cookies are included with every Http request, they slow your web application, and send unencrypted data over the internet
- limited to 4kb.

- early Internet explore worked to solve this problem by creating userData. which allowed 64kb of data stored per domain.

## HTML5 Storage

- specifically named Web Storage also referred to as local storage or DOM storage
- html 5 storage is simply a way for web pages to store data in key/value pairs.

### Using HTML5 Storage

- Using the key/value pairs you store data based on a named key. That key is a string, and supports strings booleans integers and floats. IMPORTANTLY all data is stored as a string, so type methods will need to be used when accessing the data.
- `parseInt() parseFloat()`
- `setItem(keyvalue)` will overwrite the value in that key location.
- you can similarly use event listeners to check for changes in the local storage