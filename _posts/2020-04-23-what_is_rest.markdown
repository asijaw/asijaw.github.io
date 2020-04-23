---
layout: post
title:      "What is REST?"
date:       2020-04-23 16:54:08 +0000
permalink:  what_is_rest
---


When creating a web-based application, we want to be able to send request to our server and we except the server to send us back a response based on that request. To do this we would have to know exactly how to server takes in a request. Subsequently, a server would have to remember information about a client and send back a response based on that stored information. In order to make this interaction simplier, Universal Resource Identifiers or URIs are used to provide unique addresses that allow this communication. Having this interface allows each request-response to be independent of one another, making our interactions stateless. 

In order to maintain separate of concerns we use RESTful routes, or simply REST. REST is a client-server architecture that provide mapping between HTTP verbs (get, post, put, delete and patch) and the CRUD (create, read, update, and delete) controller actions. These routes allow us to read from and write to our database. When an HTTP request is sent through an application, that request is matched with a corresponding controller action. That action is executed and processed, then determines which response is sent back to the client.


