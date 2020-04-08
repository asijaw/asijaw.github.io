---
layout: post
title:      "MVC in Sinatra"
date:       2020-04-08 02:26:13 +0000
permalink:  mvc_in_sinatra
---


For my sinatra project I created a movie application that implements a Model Views Controller. This application allows the users to add their favorite movies to a database and access a list of all the users favorite movies . Sinatra is a Ruby framework that aids in the creation of simple web applications with help of some HTML, CSS, and Javascript. This is possible with the use of Model Views Controller or MVC. Each component of the MVC is essential in ensuring that the correct information is dissplayed to the user and well as any request from the user are processed and rendered correctly. 

In order to get started, the use of Corneal, a Ruby Gem designed to give the skeletal structure of a Sinatra web app, was installed to set up the environment needed for the app. This Gem was installed using the *gem install corneal* command followed by the *run corneal new APP-Name* command. Running * bundle install* installed all of the gem dependencies needed for this application and for corneal to run. Once this gem was up and running, the shotgun command and following the link, http://127.0.0.1:9393/ allowed me to track the visual progression of my web application. 

**MODELS**
Models held all the classes that managed my databases and any logic needed in my application. Models are aided with ActiveRecord macros that allow object relationships and associations. These associations such as has_many, belongs_to, has_many_through, etc. were defined in my models classes. Any attributes that needed to be define were created in database tables and migrated for use using rake. 

**VIEWS**
Views acesses your embedded ruby or erb templetes to display information, as well as collect user information to be processed. This was done with the help of HTML tags and forms, as well as CSS for styling and creating a better user experience. Because I didn't want the user to be able to directly manipulate my data, controllers were used to validate and manipulate data.

**CONTROLLERS**
Controllers processed all of the data in my application. Once the information was feed into the controllers, the information was validated and then passed to the models to update the database. This updated data was then feed back to the controller which then rendered the correct views pages. Controllers are resposible for which erb pages are displayed according to user input. This was done with the use of RESTful Routes. Restful Routes are routes that use HTTP verbs such as get, post, patch, and delete and map them to the controller create, read, update, and delete action or CRUD. 

Using MVC in Sinatra was a simple and popular way of implementing separation of concerns, where groups of files have specific jobs and work together in defined ways for desired output. Using this framework allowed a better understanding of web applications are setup and how data is passed back and forth between the user and a database. Though this project presented many challenges, I am grateful for this experience. 




