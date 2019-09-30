---
layout: post
title:      "Welcome Back, Habit Tracker!"
date:       2019-09-29 20:29:49 -0400
permalink:  welcome_back_habit_tracker
---


Here we are once again staring each other fiercely in the face… you trying to take me down and me trying to conquer every error and bug you throw my way.

We meet under the guise of ‘adding improvements and front-end functionality’. This should be fun right???

YES! Fun beyond belief.

![](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQFcOFZkjXYk7HhDkUgDvk-rCZZtLfQWfyF3xtU3MTLMlwaZbLc)


Let's start with the basics...
## Adding Javascript to a Rails project

In order for your project to handle the functionalities that come with Javascript and jQuery we need to make sure a few things are set up…


Step 1.  Your gemfile needs to have the jQuery gem. If it is not already in the file add it, and run bundle install.

```
gem 'jquery-rails', '~> 4.3', '>= 4.3.1'
gem 'active_model_serializers' 
```
*** I'll explain the 2nd line of code later, but make sure you add it!*

Step 2.  Go over to your manifest file… if you are running Rails <= 5.0 you need to add this text  before your `//= require_tree` 

```
//= require jquery3
//= require jquery_ujs
```


Step 3.  Lets handle relationships in JSON! This is where our Active Model Serializer gem comes in handy!
And because you added it earlier, we don’t have to bundle install again, and we can start building out our serializer.

In your terminal type:

```
Rails g serializer *NAME OF MODEL*
```

Your serializer models will show up in a separate folder **/app/serializers**


Step 4.  In the serializer model add the attributes that you want JSON to have access to.
Also add the relationships for that model.

Here is an example...

![](https://imgur.com/a/YsJ6uJH)


Step 5.  Head into your controller so you have the option to render a JSON view.
You want your controller to respond to both html and JSON when necessary.

Go into your controller and choose an action where you will need access to JSON.
Use respond_to to give the action access to both views.

![](https://i.imgur.com/bnegcxt.png)

## You are ready to start coding your javascript file!

The browser's developers tool console is truly your best friend! It's good way to manipulate your DOM, analyze your code with `debugger` and to ensure that your page is loading your javascript file.

To check if your javascript is loading, you can simply add an alert message in your code or a console.log('Hello World') that will show up in your browser console when you load the page.


![](https://i.imgur.com/djSG5sb.png)


The biggest challenge I faced with this project was taking the new knowledge I had about javascript and somehow putting it together to create a robust application.

Also, knowing that there are multiple ways of doing tasks ie... jQuery functions, abstracting data and changing scope. 

With a little more practice I can learn to really love Javascript.

Happy Coding!
Patience is truly a virtue.

-S





