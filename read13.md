 [HOME](https://mousasbbah.github.io/reading-notes/)

# Local Storage
## What is HTML Web Storage?
With web storage, web applications can store data locally within the user's browser.

Before HTML5, application data had to be stored in cookies, included in every server request. Web storage is more secure, and large amounts of data can be stored locally, without affecting website performance.

Unlike cookies, the storage limit is far larger (at least 5MB) and information is never transferred to the server.

Web storage is per origin (per domain and protocol). All pages, from one origin, can store and access the same data.


## **Old school: Cookies**
The concept of client-side storage has been around for a long time. Since the early days of the web, sites have used cookies to store information to personalize user experience on websites. They're the earliest form of client-side storage commonly used on the web.

These days, there are easier mechanisms available for storing client-side data, therefore we won't be teaching you how to use cookies in this article. However, this does not mean cookies are completely useless on the modern-day web — they are still used commonly to store data related to user personalization and state, e.g. session IDs and access tokens.

## **New school: Web Storage and IndexedDB**
The "easier" features we mentioned above are as follows:

* The Web **Storage API** provides a very simple syntax for storing and retrieving smaller, data items consisting of a name and a corresponding value. This is useful when you just need to store some simple data, like the user's name, whether they are logged in, what color to use for the background of the screen, etc.
* The **IndexedDB API** provides the browser with a complete database system for storing complex data. This can be used for things from complete sets of customer records to even complex data types like audio or video files.


## **The future: Cache API**

Some modern browsers support the new Cache API. This API is designed for storing HTTP responses to specific requests, and is very useful for doing things like storing website assets offline so the site can subsequently be used without a network connection. Cache is usually used in combination with the Service Worker API, although it doesn't have to be.


## HTML Web Storage Objects
HTML web storage provides two objects for storing data on the client:

* **`window.localStorage`** - stores data with no expiration date
* **`window.sessionStorage `**- stores data for one session (data is lost when the browser tab is closed)
Before using web storage, check browser support for localStorage and sessionStorage:
```js
if (typeof(Storage) !== "undefined") {
  // Code for localStorage/sessionStorage.
} else {
  // Sorry! No Web Storage support..
}
```

### **The localStorage Object**
The localStorage object stores the data with no expiration date. The data will not be deleted when the browser is closed, and will be available the next day, week, or year.

**Example**:
```js
// Store
localStorage.setItem("lastname", "Smith");

// Retrieve
document.getElementById("result").innerHTML = localStorage.getItem("lastname");
```

**Example explained**:

* Create a localStorage name/value pair with `name="lastname" and value="Smith"`
* Retrieve the value of "lastname" and insert it into the element with `id="result"`

### **The sessionStorage Object**
The sessionStorage object is equal to the localStorage object, except that it stores the data for only one session. The data is deleted when the user closes the specific browser tab.

 [HOME](https://mousasbbah.github.io/reading-notes/)