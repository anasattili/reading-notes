# Read: 13 - Local Storage

## THE PAST, PRESENT & FUTURE OF LOCAL STORAGE FOR WEB APPLICATIONS
local storage is one of the areas where native client applications have held an advantage over web applications. For native applications, the operating system typically provides an abstraction layer for storing and retrieving application-specific data like preferences or runtime state. These values may be stored in the registry, INI files, XML files, or some other place according to platform convention. If your native client application needs local storage beyond key/value pairs, you can embed your own database, invent your own file format, or any number of other solutions.

* Cookies are included with every HTTP request, thereby slowing down your web application by needlessly transmitting the same data over and over
* Cookies are included with every HTTP request, thereby sending data unencrypted over the internet (unless your entire web application is served over SSL)
* Cookies are limited to about 4 KB of data — enough to slow down your application (see above), but not enough to be terribly useful

**HTML Web Storage**

> With web storage, web applications can store data locally within the user's browser.
Before HTML5, application data had to be stored in cookies, included in every server request. Web storage is more secure, and large amounts of data can be stored locally, without affecting website performance.
Unlike cookies, the storage limit is far larger (at least 5MB) and information is never transferred to the server.
Web storage is per origin (per domain and protocol). All pages, from one origin, can store and access the same data.

![HTML Local Storage](https://www.codeproject.com/KB/HTML/Web-Storage-In-Essence/localStorageShare.jpg)


## HTML Web Storage Objects
HTML web storage provides two objects for storing data on the client:
* `window.localStorage - stores data with no expiration date`
* `window.sessionStorage - stores data for one session (data is lost when the browser tab is closed)`
* `Before using web storage, check browser support for localStorage and sessionStorage:`
* `if (typeof(Storage) !== "undefined") {`
*  `// Code for localStorage/sessionStorage.`
* `} else {`
*  `// Sorry! No Web Storage support..`
* `}`

## The localStorage Object
The localStorage object stores the data with no expiration date. The data will not be deleted when the browser is closed, and will be available the next day, week, or year.
* `Example`
* `// Store`
* `localStorage.setItem("lastname", "Smith");`
* `// Retrieve`
* `document.getElementById("result").innerHTML = localStorage.getItem("lastname");`

> Create a localStorage name/value pair with name="lastname" and value="Smith". Retrieve the value of "lastname" and insert it into the element with id="result".

> The syntax for removing the "lastname" localStorage item is as follows:
`localStorage.removeItem("lastname");`

## The sessionStorage Object
The sessionStorage object is equal to the localStorage object, except that it stores the data for only one session. The data is deleted when the user closes the specific browser tab.
The following example counts the number of times a user has clicked a button, in the current session:

* `Example`
* `if (sessionStorage.clickcount) {`
*  `sessionStorage.clickcount = Number(sessionStorage.clickcount) + 1;`
* `} else {`
*  `sessionStorage.clickcount = 1;`
* `}`
* `document.getElementById("result").innerHTML = "You have clicked the button " +`
* `sessionStorage.clickcount + " time(s) in this session.";`




