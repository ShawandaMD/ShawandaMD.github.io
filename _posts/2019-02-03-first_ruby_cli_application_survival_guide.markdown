---
layout: post
title:      "First Ruby CLI Application Survival Guide"
date:       2019-02-03 08:54:24 -0500
permalink:  first_ruby_cli_application_survival_guide
---


A survival guide is essientially a guide helping someone manage to **continue** or **exist** in spite of difficult circumstances. Managing to simply **EXIST** is how I felt about my first project, but I can also be a drama queen so there's that.

I had this irrational fear of just not being able to do it. As if my brain would compute "INFORMATION OVERLOAD" and implode, but I stand before you today with a completed project and a sigh of relief.


## Here is how I survived my first project!
		 
1. 		 Reading ALL of the instructions or resources. 

   9/10 you will find detailed instructions of exactly where to start or how to solve a problem through the links in the project page or study groups because the ask a question techs have left the building. Being able to problem solve on your own is such a big part of this project, so get crafty!
	
2.     Start with finding a scrapable site

    This is the foundation of the project, so choose a site with clean and clear css selectors that are identical for each object you want to get information from. I've learned that sites with anything stored in individual cards (if not loaded with Javascript) are good to use. When you have found your site use this [repl.it](https://repl.it/@jenn_leigh_hansen/ScraperChecker?language=ruby) to help determine if it is scrapable. Be sure to fork the file first! Here is an example of a website I used.
	![](https://www.freedieting.com/wp/wp-content/uploads/2017/01/homechef-recipes.jpg)
	
3.    Decide what information you want to scrape 

	    Creating a plan for your project before even touching a gem is important. It allows you to structure your project so you can break it into pieces on what to scrape and what infomation is needed. For example once I knew my site was scrapable I came up with an idea of what I wanted my application to do, and then I scraped each object and potential attribute and saved the css selectors. Use the repl.it link to scrape the site and make sure it returns the data in the format you need it.
			 
4.     Build your gem! (Working locally)  

    This is where the magic happens! Start with setting up a folder for your project...perferable outside of the folder you keep your labs. Use Snake_Case to name your file and keep it consistent through out your project and github. Next you will open your terminal and type 'bundle install ***Snake_case file name***'.	Be sure to say yes to the code of conduct and license prompts because these are requirements for the project. Once you get into the actual project, name your files accordingly and set up your environment to require those files and neccessary gems. DON'T FORGET TO HIT SAVE!
			
5.      Take a nap		

		 You've done a lot kiddo... Take a break.
		 
6.     GIT involved (get it??? I couldn't help myself)

    It's time to push this new repository and changes to github! In your terminal type in 'git init' to create a new repository in git hub. Next type 'git add .' to add all of the files you've changed, then type 'git commit -m "First Commit" ' and lastly 'git push' to push those changes through. Now head over to github and create a new repository and follow the steps on how to 'push an existing repository'. To confirm this was done correctly your terminal should say (master) *file name* and your github should say 1 commit.

7.      Now it's time to code!

    At this point your environment should be set up and you have a cool new git repository. Take the time to make sure your bin folder has a file that calls your CLI class to start your program. Then go into your cli class and call a simple method that puts out a string ie...
	
		``` 
		def start
		   puts "I am a CLI Application!"
		end 
		```			
	
	Start your program in the terminal by calling ` ruby bin/***file name***`. You should see the string from the method printed!
	
8.    Tackle your project
	
	    The confirmation in step 7 allowed me to move on to coding out my scrape class (binding.pry is your best friend in this class... and pretty much through out the entire project). After this I was able to semi set up my CLI class and whatever other classes I needed. Don't be afaid to ask for help whether it's from the cohort lead, peers in your cohort or strangers on the internet! Be sure to run your program often to make sure it's working the way you intended.
			
9.     AND WE'RE DONE!

      Whew! Wasn't so bad right? There will be a lot of errors along the way but what is a program without a few errors? Proof read every single file before submitting!
			
10.   Take another nap


#### Signing off
**-S**

> [Patience is truly a virtue](https://shawandamd.github.io/patience_is_truly_a_virtue)
	
	
		


