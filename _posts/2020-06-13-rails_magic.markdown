---
layout: post
title:      "Rails Magic"
date:       2020-06-13 23:42:10 +0000
permalink:  rails_magic
---


Working on this Rails project for the past two weeks was very challenging. A lot of the features used in rails mimic those used in Sinatra, but a lot of things suddenly became automatic with rails magic. One of my favorite feautes of this rails magic was generators. Generators allow you to building out databses, models, views, controllers, or even all of the above, with a few terminal commands. This saved a lot of time and unnecesaary errors in the beginning stages of building out my program. Although generators can be super helpful, they can also cause your program to be cluttered with unnecessary files if not careful. These extra files do not neccessarily harm the development process of your code, but it can get complicated when others want to contribute to your code and aren't sure which files are actaully needed for the program to run and which files are just junk files from various generator commands. While making this program I was sure to research exactly whcih files would be created from each generator and only used those which created the files I would need for development as to not clutter my program. 

Another feature of rails magic was rails routes. In Sinatra, a lot of the RESTful routes had to be manually typed as get, post, or delete paths. With rails, a lot of these path were automatically added with simple lines like ***resource :user***. This created paths for all of the RESTful methods defined in the controller. Only custom routes have to be explicitly defined in the routes file. This way of defining routes cleaned up the controller in a way that made to code more readable. Rails also provides route helpers that allow the programmer to redirect and render different routes without hardcoding the URL. For example, instead of typing ***redirect_to /users/#{@user.id}*** you’re allowed to simply type ***redirect_to user_path(@user)***. This prevents any changes in the URL or route from effecting the code. This concept got even more interesting with nested routes. Nested routes allow you to type things like ***user_posts_path(@post.user)*** to access all of the posts of a user. This allowed the URL in the browser to be more cleaned up and practical for the route. 

Overall, I enjoyed this project and I earned a lot while developing it. I’m excited to learn more tricks of Ruby magic as a become more advanced as a Ruby developer. 
