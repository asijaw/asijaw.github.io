---
layout: post
title:      "What is fetch()"
date:       2020-08-17 17:57:20 +0000
permalink:  what_is_fetch
---


In front-end development in order to make interactive webpages we tend to send lot of data across the internet. Processing this data synchronously leaves the user waiting for a response from the browser and for the page to load. To help solve this problem AJAX (Asynchronous Javascript and XML) and fetch requests were developed. An asynchronous approach allows for HTML and CSS to be rendered quickly on to the page, and then use Javascript to access the data and manipulate the DOM. 

A fetch request accepts a URL along with a request type, either a "GET", "POST", "PATCH/PUT" or "DELETE", and that URL is then matched with a route.

***fetch("http://127.0.0.1:3000/users" { method: "POST"})*  **

The fetch request always returns a what is called a promise. This promise tells the state or status of the request either it is pending, rejected, or resolved. If the promise is pending, it is can still go into a rejected or resolved state. If the promise is rejected that means an error occurred and the request could not be fufilled. If is resolved, then the promise has a reponse value. "DELETE" requests that are fulfilled are now done, but all other request have to go a step further in order to use the response data and to be able to append the DOM. Information is sent as *strings* across the internet, therefore, the body of the reponse must be jsonified. 

***.then(response => response.json())* **

The *.json()* method returns another promise, but we can now use the data to manipulate the DOM.

***.then(data => console.log(data)* **

Fetch can be confusing at first, but it is an important tool in front-end development. Being able to acess the backend and display data to the user without long wait times and without having to reload the page each time is essential to having a better user experience. 

