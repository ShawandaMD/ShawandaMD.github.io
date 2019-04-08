---
layout: post
title:      "Hats Off To Sinatra"
date:       2019-04-08 01:11:36 +0000
permalink:  hats_off_to_sinatra
---

### What is Sinatra?

Sinatra is a free software library and **DSL**(Domain Specific Language) that allows users to create web applications easily. Sinatra is written in ruby and is a quick alternative to **Ruby on Rails** for simple web applications.

#### My Experience with Sinatra…

A few hours shy of this post, I completed my first ever Sinatra project! I don’t much to compare it to besides my first CLI project and I will say that it erased my fear of creating dynamic applications.

Everything had it’s place and worked together efficiently, the set up was a breeze with the **corneal gem** and viewing changes were as easy as refreshing your server. The only real challenges I had was ensuring my routes, erb files and ruby logic were accurate.

#### My Project…

It’s a simple travel journal website that allows users to create an account and write journal entries from their travel experiences. The user can view, edit and delete their entries and also have the option to view other users entries. [Check it out](https://github.com/ShawandaMD/sinatra-wanderlust-app).

### How to get started!

**Step 1: What kind of app do you want to build?**
*Obvious, no?*
Think of what you want your app to do… does your app have users? Do they need to be able to log in? Are there forms involved? Do you have multiple models and if so how do they interact with each other?
Write it out! Create a map of your site. Here is an example of a model map I created before actually coding…


	MODEL-
		~JournalEntry

	ATTRIBUTES-
		~Title
		~Content 
		~date
		USER_ID
		COUNTRY_ID

	ASSOCIATIONS-
		belongs_to :user
		belongs_to :country
	
	
**Step 2: Setting up a Sinatra Framework (Local Environment)**

You want to load the Sinatra file through the corneal gem.

1.   Open up your terminal and type ‘gem install corneal’

2.   then run ‘corneal new *name-of-project*'

3.   Open up file in your text editor and you will see your Sinatra file structure(*Remove the files you don’t need*).

4.   Create a git repository for your new project.

5.   Connect your project to *github*.

**Step 3: Create your database and Models**

1.   Create a migration file through your terminal with rake.

2.   Create tables(tables should always be plural) through the migration file and rake commands.

3.   Create accompanying models for your tables(Model names should be singular and match table names).

**Step 4: Controllers and Inheritance**

When creating your controllers keep your initial Application controller simple. Any other controllers that will be used for the app must...

1.   Be inherited from the main controller 

      ```
		class  UserController < ApplicationController
		end
			```

2.   Must be added to config.ru file above the Application Controller
       ```
			 use UserController
			 run ApplicationController
			 ```
			 
**You’re ready to start building your app and functionality!**

*Now go young grasshopper and build something great.*

Happy coding!

**-S**
