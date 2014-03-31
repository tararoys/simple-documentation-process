---
layout: post
title:  "Simple Documentation Setup"
date:   2014-03-30 18:32:40
categories: jekyll update
---


Writing good directions with microsoft word is like having to take all of the water out of a swimming pool with a drinking glass. The process of writing good directions is hard.  When a thing is hard, you do not do it.

Writing directions is simple. A person who is able to use a keyboard is able to make good directions.

The things that are not simple are 
  1. Keeping backup copies of your work. 
  2. Making corrections to your work. 
  3. Putting your work online. 

I have a system that does all of the hard things with three commands. I do not spend hours making backup copies, making corrections, or puting my work online. I spend 10 seconds.  

#This is how my process works:

1. I make a set of directions using my special template.  
2. I put my new set of directions in a the 'Articles' folder in my "blog" file. 
3. I go to the command line. I type
     
     git add .  && git commit -v 

4. I type git push

If I do steps 2 through 4, my process makes automatic backups, saves everything, and publishes it to my blog on the web. This turns an hours-long process into something that takes 30 seconds. 

#What the steps in the process do

1. The template is important because if I use this template, I am able to publish my blog in seconds. I will not have to make changes to the format. I do not have to take hours to make changes so that I can put my directions on the internet.
2. Putting the directions in the articles folder is important so that my software knows where to go looking for new directions. 
3. The git add . && git commit- v command is important because it saves and backs up your work. This command is like a better version of saving a Microsoft word document. When you go to save a Microsoft Word document, it saves over your old set of directions.  If you make a mistake, you are not able to go back to the old version.  If you save with this command, however, it saves a new copy of your directions, and keeps all of the old versions.  it's like the computer keeps every draft of you directions in a stack of papers. The oldest version is on the bottom of the stack of papers. When you save a new version, you stick it on the top of the stack.  You are able to always go back to the old versions because they are still there, under the new version.  

4. Now, for the final part. 
    
    git push 

This command does two things for me. It saves a backup copy of my directions to a place called Github.  I have a system set up so that this command also sends a copy to my public blog.  My blog is smart and knows that if I send it a new set of directions that were made with my special template, I want those directions to be a new post on my website. So it posts those directions. Five seconds after I say 'git push,'' I have a new post on my website.

#How to set up this process

1. Let us get the blog software.  Go to [General Blog](https://github.com/tararoys/General_Blog). This is the same blog software I use for my website, (tararoys.com)[http://tararoys.com/].  This general blog is a blank blog that we are going to use to start a new blog project. 

2. You will need to copy this blog. I am going to assume that you have some knowlege of the command line and of git.  If you are do not know these things, please contact me and I will take the time to make instructions that people who don't use git are able to follow. 
   1. fork the repository.  (To make this tutorial easier on yourself, you MUST fork it.)
   2. clone down the repository. 

3. Now you have the program. In this program, go to the articles folder.  Make a new file.  This file has to have a name like this: my-new-post.markdown.  The important parts are that each word is lower case, each word is separated by dashes, and it ends with .markdown.

 Now you need to start writing an article. Below is the template.  Use this template to write the article. As you write the article, make sure to save your article into the articles folder.  

### Article Template

Every article is a markdown file with some meta-data at the top of the file.

    Title: Control Flow in Node Part II
    Author: Tim Caswell
    Date: Thu Feb 04 2010 02:24:35 GMT-0600 (CST)
    Node: v0.1.91

    I had so much fun writing the last article on control flow, that I decided to...

    ## First section: Display JavaScript files

    * display contents of external JavaScript file (path is relative to .markdown file)
    <test-code/test-file.js>

    * display contents of external JavaScript file and evaluate its contents
    <test-code/evaluate-file.js*>

    More content goes here.

Use this article template.  This makes putting the article on the web very easy.  
The article is written in markdown.  Markdown is very simple, and you are able to see how to use it [here](http://chronicle.com/blogs/profhacker/markdown-the-syntax-you-probably-already-know/35295)  

### Author format

Every author has a markdown file located in `authors` folder. You should name this file by your name and surname `Name Surname.markdown`.

    Github:   your_github_account
    Email:    your_email@domain.com
    Homepage: http://yourhomepage.com
    Twitter:  your_twitter_account
    Location: City, State, Country

    A few words about you.

4. Now that you made a draft of an article, we are going to save it. Because you cloned the repository, the folder General Blog is 'under version control.' Being under version control is like having every file you see be the top paper on a stack of papers.  The papers lower on the stack are old versions of that file.  With version control, you can go through the stack, see old versions, and go back to them. 

Because you made a new article, we need to make a new space for a stack so that our 'version control system' can start keeping track each draft of this article as we stick it on the stack.  This new article is going to be the first 'piece of paper' on that stack. So the first thing we need to do is tell git, our version control manager, to stick the new article on the new stack.  We do this with the command 

   git add . && git commit -m 'NOTE ABOUT WHAT I WAS WRITING'

A note about the command: The words in capital letters between the ' ' are a place where you can write a note about the draft you are saving. I like to make good notes because in the future it will help  me look for the draft I need days or weeks from now.

After you do this command, you now have put the draft on the top of your stack of drafts. 

5. 

