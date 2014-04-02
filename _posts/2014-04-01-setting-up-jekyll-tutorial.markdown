---
layout: post
title:  "Setting Up Jekyll Tutorial"
date:   2014-04-01 18:32:40
categories: jekyll update
---

Writing good documentation for a project with microsoft word is like having to take all of the water out of a swimming pool with a drinking glass. The process of writing good documentation is hard.  When a thing is hard, you do not do it.

Writing good documentation is simple. A person who is able to use a keyboard is able to and is able to take some time to write down what they are doing as they do it is able to make good documentation.

The things that are not simple are 
  1. Keeping backup copies of your log.  
  2. Putting your log online. 
  3. formating your log so that it is easy to read

I have a system that does the first tow things all of the hard things with three commands. I do not spend hours making backup copies or puting my work online. I spend 10 seconds. I also have techniquest to make the third thing much more simple. 

#This is how my process works:

1. I make a set of directions using my special log template.  
2. I put my new set of directions in a the '_posts' folder in my blog file. 
3. I go to the command line. I type
     
     git add .  && git commit -v 

4. I type 

    git push

If I do steps 2 through 4, my process makes automatic backups, saves everything, and publishes it to my blog on the web. This turns an hours-long process into something that takes 30 seconds. 

##What the steps in the process do

1. The template is important because if I use this template, I am able to publish my blog in seconds. I will not have to make changes to the format. I do not have to take hours to make changes so that I can put my directions on the internet.
2. Putting the directions in the articles folder is important so that my software knows where to go looking for new directions. 
3. The git add . && git commit- v command is important because it saves and backs up your work. This command is like a better version of saving a Microsoft word document. When you go to save a Microsoft Word document, it saves over your old set of directions.  If you make a mistake, you are not able to go back to the old version.  If you save with this command, however, it saves a new copy of your directions, and keeps all of the old versions.  it's like the computer keeps every draft of you directions in a stack of papers. The oldest version is on the bottom of the stack of papers. When you save a new version, you stick it on the top of the stack.  You are able to always go back to the old versions because they are still there, under the new version.  

4. Now, for the final part. 
    
    git push 

This command does two things for me. It saves a backup copy of my directions to a place with the name of Github. Github has a service called Github Pages that lets me publish simple blog pages. If I use my special template to make a log and put it in the right folder, github will make a nice-looking webpage for me. Five seconds after I say 'git push,'' I have a new post on my project's website. 

##How I set up a simple documentation process with Git and Jekyll

This is how I take easy notes: I go to a webpage. When I see a part of the webpage that has valuable information, I use the web inspector in Google Chrome to change the background of that part to orange.  Then I save that webpage to my computer with a number and a name. 

The website below is my copy of the jekyll main page.  It is numbered 001-follow-main-page-instructions.html because it is the first website I saw when I googled Jekyll. I name follow-main-page-instructions because that is what I did on this page.  

[Tara's higlighted copy of the Jekyll Website](/GettingStartedWithJekyllWebsites/001-follow-main-page-instructions.html/) 

[Actual Jekyll main page](http://jekyllrb.com/)

I do what the page says to install jekyll. The install process takes about half an hour. 

{%raw%}
```bash
    Last login: Sun Mar 30 18:07:00 on ttys000
    Taras-MacBook-Air:~ tlroys$ cd ~/Desktop
    ruby-2.0.0-p247 is not installed.
    To install do: 'rvm install ruby-2.0.0-p247'
    Taras-MacBook-Air:Desktop tlroys$ script jekyll_start.log
    Script started, output file is jekyll_start.log
    bash-3.2$ gem install jekyll
    Fetching: liquid-2.5.5.gem (100%)
    Successfully installed liquid-2.5.5
    Fetching: fast-stemmer-1.0.2.gem (100%)
    Building native extensions.  This could take a while...
    Successfully installed fast-stemmer-1.0.2
    Fetching: classifier-1.3.4.gem (100%)
    Successfully installed classifier-1.3.4
    Fetching: rb-kqueue-0.2.2.gem (100%)
    Successfully installed rb-kqueue-0.2.2
    Fetching: listen-1.3.1.gem (100%)
    Successfully installed listen-1.3.1
    Fetching: maruku-0.7.0.gem (100%)
    Successfully installed maruku-0.7.0
    Fetching: posix-spawn-0.3.8.gem (100%)
    Building native extensions.  This could take a while...
    Successfully installed posix-spawn-0.3.8
    Fetching: yajl-ruby-1.1.0.gem (100%)
    Building native extensions.  This could take a while...
    Successfully installed yajl-ruby-1.1.0
    Fetching: pygments.rb-0.5.4.gem (100%)
    Successfully installed pygments.rb-0.5.4
    Fetching: highline-1.6.21.gem (100%)Fetching: highline-1.6.21.gem
    Successfully installed highline-1.6.21
    Fetching: commander-4.1.6.gem (100%)
    Successfully installed commander-4.1.6
    Fetching: safe_yaml-1.0.1.gem (100%)
    Successfully installed safe_yaml-1.0.1
    Fetching: colorator-0.1.gem (100%)
    Successfully installed colorator-0.1
    Fetching: redcarpet-2.3.0.gem (100%)
    Building native extensions.  This could take a while...
    Successfully installed redcarpet-2.3.0
    Fetching: blankslate-2.1.2.4.gem (100%)
    Successfully installed blankslate-2.1.2.4
    Fetching: parslet-1.5.0.gem (100%)
    Successfully installed parslet-1.5.0
    Fetching: toml-0.1.1.gem (100%)
    Successfully installed toml-0.1.1
    Fetching: jekyll-1.5.1.gem (100%)
    Successfully installed jekyll-1.5.1
    18 gems installed
```
 {%endraw%} 
 
 Jekyll install took what seemed like half an hour.  This made me lose my momentum. I continue following the instructions. 

 {%raw%} 

```bash

    bash-3.2$ jekyll new documentation-made-painless
    New jekyll site installed in /Users/tlroys/Desktop/documentation-made-painless.
    bash-3.2$ cd documentation-made-painless/
    bash-3.2$ ls
    _config.yml _layouts  _posts    css   index.html
    bash-3.2$ jekyll serve
    Configuration file: /Users/tlroys/Desktop/documentation-made-painless/_config.yml
                Source: /Users/tlroys/Desktop/documentation-made-painless
           Destination: /Users/tlroys/Desktop/documentation-made-painless/_site
          Generating... done.
        Server address: http://0.0.0.0:4000
      Server running... press ctrl-c to stop.
    ^Cbash-3.2$ jekyll serve &
    [1] 7451
    bash-3.2$ Configuration file: /Users/tlroys/Desktop/documentation-made-painless/_config.yml
                Source: /Users/tlroys/Desktop/documentation-made-painless
           Destination: /Users/tlroys/Desktop/documentation-made-painless/_site
          Generating... done.
        Server address: http://0.0.0.0:4000
      Server running... press ctrl-c to stop.

```
I start the server, go to google, and type in http://0.0.0.0:4000. I see [a jekyll blog that looks like this](/GettingStartedWithJekyllWebsites/002my-new-jekyll-site.html)
I click on the post.  I see a link to a post called [Welcome to Jekyll!](/GettingStartedWithJekyllWebsites/003post-on-jekyll.html). If you click on it, you see an example post.  

 {%endraw%} 

 ## Adding a new post to Jekyll and creating a Github Repository

 In this section, I fail to do and test just one thing at a time. I create a new post and at the same time put this blog under version control. 

 I have read the example post.  I am now going to take my how to set up easy documentation post and copy it into a jekyll blog. 
 {%raw%} 

```bash

    bash-3.2$ ls
    _config.yml _posts    css
    _layouts  _site   index.html
    bash-3.2$ subl .
```

 {%endraw%} 
 
Using Sublime, I copy my 'how to set up easy documentation' post from my failed attempt to set up a node.js wheat blog into this new jekyll blog. Since I put a new post in the posts directory. Do I have to kill the server and restart it? 
 
 {%raw%} 

```bash
    bash-3.2$ jekyll -w
    invalid option: -w
    bash-3.2$ jekyll --help
      NAME:

        jekyll

      DESCRIPTION:

        Jekyll is a blog-aware, static site generator in Ruby

      COMMANDS:
            
        build                Build your site                
        default                             
        docs                 Launch local server with docs for Jekyll v1.5.1        
        doctor               Search site and print specific deprecation
    warnings                
        help                 Display global or [command] help documentation.        
        import               Import your old blog to Jekyll         
        new                  Creates a new Jekyll site scaffold in PATH             
        serve                Serve your site locally                

      ALIASES:
      
        hyde                 doctor   
    bash-3.2$ jekyll build -w
    Configuration file: /Users/tlroys/Desktop/documentation-made-painless/_config.yml
                Source: /Users/tlroys/Desktop/documentation-made-painless
           Destination: /Users/tlroys/Desktop/documentation-made-painless/_site
          Generating... done.
     Auto-regeneration: enabled
     
    ^Cerror: can't be called from trap context. Use --trace to view backtrace
```
{%endraw%}

The jekyll example blog post assumes that you know about hte build command.  I did not know about the build command.  I had to guess using --help.  So here is what the example post should have said.      

    jekyll build -w
     
This turns the markdown post into a static website. 

Type 

    jekyll serve. 

This starts your local server. You can go to your browser and type 

    localhost:4000

This will take you to your main page.  It will show you the list of posts, and you can click on this post to see your changes.

I wonder if simply typing jekyll build will update the site? 

{%raw%} 

```bash

    bash-3.2$ jekyll build
    Configuration file: /Users/tlroys/Desktop/documentation-made-painless/_config.yml
                Source: /Users/tlroys/Desktop/documentation-made-painless
           Destination: /Users/tlroys/Desktop/documentation-made-painless/_site
          Generating... done.
    bash-3.2$ git add -p
    fatal: Not a git repository (or any of the parent directories): .git
    bash-3.2$ ls
    _config.yml _posts    css
    _layouts  _site   index.html
    bash-3.2$ git init
    Initialized empty Git repository in /Users/tlroys/Desktop/documentation-made-painless/.git/
    bash-3.2$ git add _layouts/
    bash-3.2$ git add _site/
    bash-3.2$ git add css/
    bash-3.2$ git ad _config.yml 
    git: 'ad' is not a git command. See 'git --help'.

    Did you mean one of these?
      add
      am
    bash-3.2$ git add _config.yml 
    bash-3.2$ git add index.html 
    bash-3.2$ git add .gitignore 
    bash-3.2$ git add _posts/2014-03-30-welcome-to-jekyll.markdown 
    bash-3.2$ git commit
    Aborting commit due to empty commit message.
    bash-3.2$ git add _posts/2014-03-30-welcome-to-jekyll.markdown 
    bash-3.2$ git commit -v
    [master (root-commit) 4d25aa0] created jekyll blog and uploaded a change to the default post
     8 files changed, 332 insertions(+)
     create mode 100644 .gitignore
     create mode 100644 _config.yml
     create mode 100644 _layouts/default.html
     create mode 100644 _layouts/post.html
     create mode 100644 _posts/2014-03-30-welcome-to-jekyll.markdown
     create mode 100755 css/main.css
     create mode 100644 css/syntax.css
     create mode 100644 index.html
    bash-3.2$ git status
    On branch master
    Untracked files:
      (use "git add <file>..." to include in what will be committed)

      _posts/2014-03-30-simpler-documentation.markdown

    nothing added to commit but untracked files present (use "git add" to track)
    bash-3.2$ git commit _posts/2014-03-30-simpler-documentation.markdown 
    error: pathspec '_posts/2014-03-30-simpler-documentation.markdown' did not match any file(s) known to git.
    bash-3.2$ git add _posts/2014-03-30-simpler-documentation.markdown 
    bash-3.2$ git commit
    [master 037b40c] New Post: Simpler documentation
     1 file changed, 103 insertions(+)
     create mode 100644 _posts/2014-03-30-simpler-documentation.markdown
```

 {%endraw%} 
 I want to put this on github.  If I simply push it to github, do magic good things happen?  Specifically, does it create a github pages website for me automatically? 
 {%raw%} 

```bash

    bash-3.2$ git status
    On branch master
    nothing to commit, working directory clean
    bash-3.2$ git remote add origin https://github.com/tararoys/simple-documentation-process.git
    bash-3.2$ git push -u origin master
    Username for 'https://github.com': tararoys
    Password for 'https://tararoys@github.com': 
    Counting objects: 17, done.
    Delta compression using up to 2 threads.
    Compressing objects: 100% (16/16), done.
    Writing objects: 100% (17/17), 7.13 KiB | 0 bytes/s, done.
    Total 17 (delta 1), reused 0 (delta 0)
    To https://github.com/tararoys/simple-documentation-process.git
     * [new branch]      master -> master
    Branch master set up to track remote branch master from origin.
    bash-3.2$ echo 'remember to delete that password from the log , you fool.'
    remember to delete that password from the log , you fool.
    bash-3.2$ echo 'to answer the previous question, no, magic does not just happen if you push to github.  You need to create a branch called github pages and push to that.'
    to answer the previous question, no, magic does not just happen if you push to github.  You need to create a branch called github pages and push to that.
    bash-3.2$ git checkout -b gh-pages
    Switched to a new branch 'gh-pages'
    bash-3.2$ git push origin gh-pages
    Username for 'https://github.com': tararoys
    Password for 'https://tararoys@github.com': 
    Total 0 (delta 0), reused 0 (delta 0)
    To https://github.com/tararoys/simple-documentation-process.git
     * [new branch]      gh-pages -> gh-pages
```

 {%endraw%} 
 and delete that password from the log file too, you fool. 
 My website is now published at http://tararoys.github.io/simple-documentation-process/ 
 {%raw%} 

```bash
    bash-3.2$ git status
    On branch gh-pages
    nothing to commit, working directory clean
    bash-3.2$ git checkout master
    Switched to branch 'master'
    Your branch is up-to-date with 'origin/master'.
    bash-3.2$ git status
    On branch master
    Your branch is up-to-date with 'origin/master'.

    nothing to commit, working directory clean
    bash-3.2$ jekyll build
    Configuration file: /Users/tlroys/Desktop/documentation-made-painless/_config.yml
                Source: /Users/tlroys/Desktop/documentation-made-painless
           Destination: /Users/tlroys/Desktop/documentation-made-painless/_site
          Generating... done.
    bash-3.2$ jekyll update
    Invalid command. Use --help for more information 
    bash-3.2$ jekyll --help
      NAME:

        jekyll

      DESCRIPTION:

        Jekyll is a blog-aware, static site generator in Ruby

      COMMANDS:
            
        build                Build your site                
        default                             
        docs                 Launch local server with docs for Jekyll v1.5.1        
        doctor               Search site and print specific deprecation
    warnings                
        help                 Display global or [command] help documentation.        
        import               Import your old blog to Jekyll         
        new                  Creates a new Jekyll site scaffold in PATH             
        serve                Serve your site locally                

      ALIASES:
      
        hyde                 doctor   
    bash-3.2$ jekyll build -w
    Configuration file: /Users/tlroys/Desktop/documentation-made-painless/_config.yml
                Source: /Users/tlroys/Desktop/documentation-made-painless
           Destination: /Users/tlroys/Desktop/documentation-made-painless/_site
          Generating... done.
     Auto-regeneration: enabled

    ^Cerror: can't be called from trap context. Use --trace to view backtrace
```

 {%endraw%} 
 I do not know what -w does. 
 {%raw%} 

```bash
    bash-3.2$ git status
    On branch master
    Your branch is up-to-date with 'origin/master'.

    nothing to commit, working directory clean
    bash-3.2$ git checkout gh-pages
    Switched to branch 'gh-pages'
```

 {%endraw%} 
 according to http://stackoverflow.com/questions/12000316/jekyll-and-github-how-to-update-the-blog-post I ought to delete my site directory and regenerate my blog. I am going to try that. 
 {%raw%} 

```bash
    bash-3.2$ ls
    _config.yml _posts    css
    _layouts  _site   index.html
    bash-3.2$ git rm -r _site/
    fatal: pathspec '_site/' did not match any files
    bash-3.2$ ls
    _config.yml _posts    css
    _layouts  _site   index.html
    bash-3.2$ git rm _site/
    fatal: pathspec '_site/' did not match any files
```

 {%endraw%} 
 Why does the git rm command not work? 
 {%raw%} 

```bash

    bash-3.2$ git rm -rf _site/
    fatal: pathspec '_site/' did not match any files
```

 {%endraw%} 
 Because _site is apparently in the .gitignore.  Why is _site in the .gitignfore file? 

 https://help.github.com/articles/using-jekyll-with-pages this page looks like the goldmine I need. 
 {%raw%} 

```bash
    https://help.github.com/articles/using-jekyll-with-pages this page looks like the goldmine I need.
```

 {%endraw%} 
 To ensure your local development environment is using the same version of Jekyll and its dependencies as GitHub Pages, you can periodically run the command gem update github-pages (or bundle update github-pages if using Bundler) once Jekyll is installed. 
 {%raw%} 

```bash
    bash-3.2$ bundle update githup-pages
    Could not locate Gemfile
    bash-3.2$ gem update githup-pages
    Updating installed gems
    Nothing to update
    bash-3.2$ gem update github-pages
    Updating installed gems
    Nothing to update
    bash-3.2$ gem update github-pages
    Updating installed gems
    Nothing to update
    bash-3.2$ echo 'nothing is updated. Does that mean I can assume my local development environment is using the same version of jekyll and its dependancies?'
    nothing is updated. Does that mean I can assume my local development environment is using the same version of jekyll and its dependancies?
```
{%endraw%} 
 
The Pages don't build" thingy doesn't seem to be telling me anything useful.  https://help.github.com/articles/pages-don-t-build-unable-to-run-jekyll I don't get any page not building errors. INstead I just get 404 pages on blogs. 

I need some in-person help.  https://www.java.com/en/download/mac_download.jsp But in order to do that, I need to get on irc.  In order to get on irc, I need to be in this page: http://en.irc2go.com/webchat/?net=freenode&room=jekyll&nick=tara  In order to get in this page, I need to download the above java applet.  In order to get that applet, I need to be in a 64 bit browser such as safari or chrome.  I went to safari and apparently safari has no place to type in urls at the top of the browser.  WTF safari.  So I went to firefox.  

Getting help should not be this hard.  I hereby resolve to make it easier. 

In order to start the download, I need to hang around for 15 minutes. 

an 'easy blog' should not be this hard. 

put in a github issue, asked that lovely scottish Mike github evangelist I met today for help, and am trying to figure out how IRC works for the first time in my life so i can ask the Jekyll irc chat what is going on. 

I have to install bloody java in order to run irc? 

I now want to kill firefox.  I just want to see the add-ons I have installed, firefox! 

restarting firefox allowed the plugin to load.  Now java is blocking it due to mismatched security.

I found the java control panel and added an exception for the irc chat. 
 {%raw%}  

```bash
    -----------made new shell because I froze the old one---------------------

    Last login: Sun Mar 30 20:50:28 on ttys000
    Taras-MacBook-Air:~ tlroys$ script jekyl-log-2.log
    Script started, output file is jekyl-log-2.log
    bash-3.2$ ls
    7357584         blog_setup.log
    Desktop         chaotica
    Desktops        code
    Documents       flashcard.rb
    Downloads       fractals
    Dropbox         gisttest
    Finances        inkscapeStuff
    HorrificallyCreativeUsesOfMummies.pdf jekyl-log-2.log
    Library         jekyllstart.log
    Movies          local
    Music         names.rb
    OpenSource        pear
    Passwordless-Loggin-to-a-Server.md  public_vs_private
    Personal        root@tararoys.com~
    Pictures        ruby_flashcards
    Plain_svg.svg       src
    Public          tara
    Random params 1.chaos     temp
    Random params 2.chaos     the_self_keyword
    Salamanders       tmp
    Screencasts       twilio-research.log
    Socrates        typescript
    TarasBlog       writing
    bin
    bash-3.2$ cd ~/Desktop
    bash-3.2$ ls
    documentation-made-painless node_blog_debugging
    jekyll_start.log    untitled folder
    bash-3.2$ cd documentation-made-painless/
    bash-3.2$ ls
    _config.yml     css
    _layouts      index.html
    _posts        jekyll_install_pretty_log.log
    _site
    bash-3.2$ jekyll build
    Configuration file: /Users/tlroys/Desktop/documentation-made-painless/_config.yml
                Source: /Users/tlroys/Desktop/documentation-made-painless
           Destination: /Users/tlroys/Desktop/documentation-made-painless/_site
          Generating... done.
    bash-3.2$ jekyll serve
    Configuration file: /Users/tlroys/Desktop/documentation-made-painless/_config.yml
                Source: /Users/tlroys/Desktop/documentation-made-painless
           Destination: /Users/tlroys/Desktop/documentation-made-painless/_site
          Generating... done.
        Server address: http://0.0.0.0:4000
      Server running... press ctrl-c to stop.
    ^Cbash-3.2$ git branch
    * gh-pages
      master
    bash-3.2$ git push origin gh-pages
    Username for 'https://github.com': tararoys
    Password for 'https://tararoys@github.com': 
    Everything up-to-date
```

 {%endraw%} 
 You will need to setup your baseurl so that it knows everything lives in the "simple-documentation-process 
 {%raw%} 

```bash 
url. You can do this by adding baseurl: /simple-documentation-process to your 'config.yml' file. And then in your templates you will need to include {{ site.baseurl }} before the links to your posts.
    > 
    > This article should also help explain more about how to setup the baseurl."
    You will need to setup your baseurl so that it knows everything lives in the simple-documentation-process url. You can do this by adding baseurl: /simple-documentation-process to your 'config.yml' file. And then in your templates you will need to include {{ site.baseurl }} before the links to your posts.

    This article should also help explain more about how to setup the baseurl.
    bash-3.2$ subl .
```

 {%endraw%} 
 let us try this out. On the jekyll website is a Project Pages URl Structure section. http://jekyllrb.com/docs/github-pages/  It is similar to the comment on the issue that I posted. https://github.com/jekyll/jekyll/issues/2182  Let us see if we can kludge these two things together to get a working produect. 
 {%raw%} 

```bash

    bash-3.2$ jekyll serve --baseurl ''
    Configuration file: /Users/tlroys/Desktop/documentation-made-painless/_config.yml
                Source: /Users/tlroys/Desktop/documentation-made-painless
           Destination: /Users/tlroys/Desktop/documentation-made-painless/_site
          Generating... done.
        Server address: http://0.0.0.0:4000
      Server running... press ctrl-c to stop.
    ^Cbash-3.2$ git branch
    * gh-pages
      master
    bash-3.2$ git add .
    bash-3.2$ git commit -v
    Aborting commit due to empty commit message.
    bash-3.2$ git reset
    Unstaged changes after reset:
    M _config.yml
    M index.html
    bash-3.2$ git add -p
    diff --git a/_config.yml b/_config.yml
    index 85daa77..a4fe4c4 100644
    --- a/_config.yml
    +++ b/_config.yml
    @@ -1,3 +1,4 @@
     name: Your New Jekyll Site
     markdown: redcarpet
     pygments: true
    +baseurl: /simple-documentation-process
    Stage this hunk [y,n,q,a,d,/,e,?]? y

    diff --git a/index.html b/index.html
    index c726819..42df5fd 100644
    --- a/index.html
    +++ b/index.html
    @@ -7,7 +7,7 @@ title: Your New Jekyll Site
       <h1>Blog Posts</h1>
       <ul class="posts">
         {% for post in site.posts %}
    -      <li><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ post.url }}">{{ post.title }}</a></li>
    +      <li><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></li>
         {% endfor %}
       </ul>
     </div>
    \ No newline at end of file
    Stage this hunk [y,n,q,a,d,/,s,e,?]? y

    bash-3.2$ git commit
    [gh-pages 2693c8a] Bugfix attempt for github pages 404 error
     2 files changed, 2 insertions(+), 1 deletion(-)
    bash-3.2$ git push origin gh-pages
    Username for 'https://github.com': tararoys
    Password for 'https://tararoys@github.com': 
    Counting objects: 7, done.
    Delta compression using up to 2 threads.
    Compressing objects: 100% (4/4), done.
    Writing objects: 100% (4/4), 1.31 KiB | 0 bytes/s, done.
    Total 4 (delta 2), reused 0 (delta 0)
    To https://github.com/tararoys/simple-documentation-process.git
       037b40c..2693c8a  gh-pages -> gh-pages
    bash-3.2$ echo 'and adding the baseurl stuff fixed the issue.'
    and adding the baseurl stuff fixed the issue.
    bash-3.2$ echo 'now let us pull those changes into the master branch.'
    now let us pull those changes into the master branch.
    bash-3.2$ git checkout master
    Switched to branch 'master'
    Your branch is up-to-date with 'origin/master'.
    bash-3.2$ git pull origin master
    remote: Counting objects: 1, done.
    remote: Total 1 (delta 0), reused 0 (delta 0)
    Unpacking objects: 100% (1/1), done.
    From https://github.com/tararoys/simple-documentation-process
     * branch            master     -> FETCH_HEAD
       037b40c..eac30ad  master     -> origin/master
    Updating 037b40c..eac30ad
    Fast-forward
     _config.yml | 1 +
     index.html  | 2 +-
     2 files changed, 2 insertions(+), 1 deletion(-)
```

 {%endraw%} 
 I captured a lot of documentation.  Let's see how easy it is to translate a shell script log into a blog post. 

 That may be tomorrow's task, because I am dog tired tonight. 
 {%raw%} 

```bash
    bash-3.2$ 
    bash-3.2$ subl .
    bash-3.2$ cd ..
    bash-3.2$ cd ~/Downloads/
    bash-3.2$ ls
    12-secret-messages.md
    2013-07-24 16.46.16.jpg
    2013-07-24 16.46.29.jpg
    2013-07-24 17.23.10.jpg
    2013-07-24 17.23.24.jpg
    2013-08-26.svg
    20130913SavingImageFreezesChaotica.txt
    2013_08_28-master
    2013_08_28-master.zip
    279aa1cfa0fe4f446c658ed6286e815d.pdf
    512px-Cave_painting,_Anthropos_(1).jpeg
    5SecondsApp.gif
    9604628703-265122221-ticket.pdf
    9924646886-243338515-tickets.pdf
    <flam3_IFS name="Terdragon">
    About Downloads.lpdf
    Adium_1.5.7.dmg
    AdobeFlashPlayerInstaller_11_ltrosxd_aaa_aih.dmg
    Alfred_2.0.7_205.zip
    Ali and Lizzy Final Paper.doc
    Apo_Plugins__Hexes_And_Crackle_by_slobo777
    Apo_Plugins__Hexes_And_Crackle_by_slobo777.zip
    Apo_Simplified.pdf
    Blender
    Boot Tea Finances - Sheet1.csv
    BümBöx.html
    BümBöx_files
    CJ_Julia_Uncovered_2_2
    CJ_Julia_Uncovered_2_2 2
    CaptureIt!.app
    CaptureIt!.zip
    Cave_painting,_Anthropos_(1).jpeg
    Chaotica_1.0.2 (1).pkg
    Chaotica_1.0.2.pkg
    Chaotica_1.1 (1).pkg
    Chaotica_1.1 (2).pkg
    Chaotica_1.1 (3).pkg
    Chaotica_1.1 (4).pkg
    Chaotica_1.1 (5).pkg
    Chaotica_1.1.1.pkg
    Chaotica_1.1.pkg
    Chaotica_1.1_tara.pkg
    Chaotica_1.5.pkg
    Couch (1).alfredworkflow
    Couch.alfredworkflow
    CreativeCloudInstaller.dmg
    CrimWks5-7R (1).doc
    CrimWks5-7R (2).doc
    CrimWks5-7R.doc
    DSC03606.jpg
    DeleteIteratorsError.mov
    DockSpaces(406) 2.dmg
    DockSpaces(406).dmg
    DockSpaces(406).zip
    Dragon_Dictate_EN_3.0.4.dmg
    Dreamforce_Conference_Proposal.rtf
    Dropbox 2.0.26 (1).dmg
    Dropbox 2.0.26.dmg
    EligibilityNotice.pdf
    Firefox 27.0.1 (1).dmg
    Firefox 27.0.1.dmg
    Flux.app
    Flux.zip
    GMStudio-Installer.exe
    GettingStartedWithJekyll
    Gimp-2.8.10-SL-Lion-ML-x64.dmg
    GoogleVoiceAndVideoSetup (1).dmg
    GoogleVoiceAndVideoSetup (2).dmg
    GoogleVoiceAndVideoSetup.dmg
    IMG_20140320_080441.jpg
    IMG_20140320_093423.jpg
    IMG_20140320_135353.jpg
    Inkscape-0.48.2-1-SNOWLEOPARD.dmg
    Install Spotify.app
    IntelligensiaOnBroadway.html
    IntelligensiaOnBroadway_files
    Invitation.docx
    JFLAP.jar
    Julia_Uncovered_v_2_2_by_ClaireJones.zip
    MATH IS ART.docx
    Office Lunchtime Foodstuffs Survey.txt
    Paintbrush-2.1.1.zip
    Photo Jul 24, 3 21 51 PM.jpg
    Photo Jun 04, 5 43 48 PM.jpg
    ProjectDesktops.app
    ProjectDesktops_1.0_trial.zip
    Quick REnder 2.jpg
    RailsInstaller-1.0.4-osx-10.7 2.app
    RailsInstaller-1.0.4-osx-10.7 3.app
    RailsInstaller-1.0.4-osx-10.7 4.app
    RailsInstaller-1.0.4-osx-10.7.app
    RailsInstaller-1.0.4-osx-10.7.app (1).tgz
    RailsInstaller-1.0.4-osx-10.7.app.tgz
    SBU V3 Manual 1-3-13
    SBU V3 Manual 1-3-13 2
    SBUV3Manual1-3-13 (1).zip
    SBUV3Manual1-3-13 (2).zip
    SBUV3Manual1-3-13 (3).zip
    SBUV3Manual1-3-13.zip
    SORI CD Release.tiff
    Salamander_names
    Salamander_names.zip
    SamsApplication.pdf
    SciFiAndStirFry - Google Drive.pdf
    Shopify Theme 2.app
    Shopify Theme.app
    ShopifyTheme_1.0.3.zip
    Silverlight.dmg
    Skype_6.6.60.467.dmg
    Spectacle+0.8.4.zip
    Spectacle.app
    SpotifyInstaller (1).zip
    SpotifyInstaller.zip
    Sublime Text 2.0.2.dmg
    The Aposhack Plugin Pack
    The Aposhack Plugin Pack.zip
    To Dropbox.alfredworkflow
    Twilio User - Account.html
    Twilio User - Account_files
    TwilloNumbers.html
    TwilloNumbers_files
    Workflow Lab (1).alfredworkflow
    Workflow Lab.alfredworkflow
    ar_todos
    ar_todos_20130308.gz
    bar-triangles-002.pdf.pdf
    bernies_big_mistake (1).zip
    bernies_big_mistake.zip
    blender-2.68a-OSX_10.6-i386.zip
    bootstrap
    bootstrap 2
    bootstrap 3
    bootstrap.zip
    bowling_game
    bowling_game.zip
    chaotica1_0_264bitmacbug2programfreezeswhentryin.zip
    chaotica_1.1_beta3.4_x64.exe
    chaotica_parameter_pack_1_by_tatasz-d5uyla2.chaos
    chaoticax264-muxed (1).mkv
    chaoticax264-muxed.mkv
    command_line_tools_os_x_mountain_lion_for_xcode__october_2013.dmg
    countdown.rb
    countdown_spec.rb
    deaf_grandma_skeleton 2
    deaf_grandma_skeleton 3
    deaf_grandma_skeleton.zip
    decrypter.rb
    exercism
    exercism 2
    exercism 3
    exercism-darwin-386 (1).tgz
    exercism-darwin-386.tgz
    exercism-darwin-amd64.tgz
    finalpaper.tex
    fleurs_mecanique.zip
    gist6180526-231f00084463eaf3ff8f0d6451d97d62d77ed181
    gist6180526-231f00084463eaf3ff8f0d6451d97d62d77ed181 2
    gist6180526-231f00084463eaf3ff8f0d6451d97d62d77ed181.tar.gz
    gist714ce5beb0d74b361c80-b13883c966fb7f70a7be6dee20b802b57c07dd61
    gist714ce5beb0d74b361c80-b13883c966fb7f70a7be6dee20b802b57c07dd61.tar.gz
    gista0eb698f06327688264d-b13f45ef04b5a7ae88633631731345aeb7a7acdd.tar.gz
    gistc9e6e271521155b79d3b-38b234f53158c9a1e384c14f3a83c46defe6742c
    gistc9e6e271521155b79d3b-38b234f53158c9a1e384c14f3a83c46defe6742c (1).tar.gz
    gistc9e6e271521155b79d3b-38b234f53158c9a1e384c14f3a83c46defe6742c.tar.gz
    googlechrome.dmg
    heroku-toolbelt (1).pkg
    heroku-toolbelt.pkg
    ical.ics
    jQuery_ajax (1).zip
    jQuery_ajax.zip
    jasmine-standalone-2.0.0
    jasmine-standalone-2.0.0 (1).zip
    jasmine-standalone-2.0.0.zip
    join.me (1).zip
    join.me.zip
    jquery.scrollTo-1.4.11.zip
    jre-7u51-macosx-x64(1).dmg
    jre-7u51-macosx-x64.dmg
    learn-to-program_p2_0.pdf
    licence (1).sig
    licence.sig
    longwall-ada-triangles-002 (1).pdf
    longwall-ada-triangles-002.pdf
    longwall-group-triangles (1).pdf
    longwall-group-triangles (2).pdf
    longwall-group-triangles (3).pdf
    longwall-group-triangles (4).pdf
    longwall-group-triangles (5).pdf
    longwall-group-triangles (6).pdf
    longwall-group-triangles.pdf
    longwall-hopper-source.psd
    longwall-hopper-triangles (1).pdf
    longwall-hopper-triangles (1).png
    longwall-hopper-triangles.pdf
    longwall-jennings-triangles.pdf
    longwall-mask (1).psd
    longwall-mask.psd
    lpmacosx.dmg
    lucky_ajax.zip
    mactex-additions (1).pkg
    mactex-basic.pkg
    mrd.vcf
    ngrok
    ngrok.zip
    node-v0.10.20.pkg
    output1a.txt
    output1a.zip
    padder (1).rb
    padder.rb
    pandoc-1.11.1 (1).dmg
    pandoc-1.11.1.dmg
    pandoc-1.12.1-1 (1).dmg
    pandoc-1.12.1-1.dmg
    photo (1).JPG
    photo (2).JPG
    photo (3).JPG
    photo (4).JPG
    photo.JPG
    racw.zip
    s1eTAwoNhhTlOa9AmRqluLQ (1).png
    s1eTAwoNhhTlOa9AmRqluLQ.png
    samblackmanapp (1).JPG
    samblackmanapp.JPG
    showdown-master
    showdown-master.zip
    sinatra_skeleton (1).zip
    sinatra_skeleton (2)
    sinatra_skeleton (2) 2
    sinatra_skeleton (2).zip
    sinatra_skeleton (3)
    sinatra_skeleton (3).zip
    sinatra_skeleton (4)
    sinatra_skeleton (4) 2
    sinatra_skeleton (4).zip
    sinatra_skeleton.zip
    sinatra_skills
    sinatra_skills (1).zip
    sinatra_skills (2).zip
    sinatra_skills (3).zip
    sinatra_skills.zip
    starter-kit-1.0.0-rc.6.1
    starter-kit-1.0.0-rc.6.1.zip
    test.db
    twilio-twilio-php-3.12.1-0-gd3cc7ab.zip
    twitter_oauth (1).zip
    twitter_oauth.zip
    vlc-2.0.8-intel64.dmg
    vlc-2.1.0.dmg
    walden (1).svg
    walden.svg
    xcode462_cltools_10_76938260a.dmg
    xcode_5.0.2.dmg
    汤玛斯.路德维格.wma
    bash-3.2$ mv GettingStartedWithJekyll/ ~/Desktop
    bash-3.2$ cd ~/Desktop
    bash-3.2$ mv documentation-made-painless/
    .git/                          _site/
    .gitignore                     css/
    _config.yml                    index.html
    _layouts/                      jekyll_install_pretty_log.log
    _posts/                        
    bash-3.2$ mv documentation-made-painless/jekyll_install_pretty_log.log .
    bash-3.2$ 
    bash-3.2$ logout
    bash: logout: not login shell: use `exit'
    bash-3.2$ exit
    exit

    Script done, output file is jekyl-log-2.log
    Taras-MacBook-Air:~ tlroys$ mv jekyl-log-2.log ~/Desktop
    Taras-MacBook-Air:~ tlroys$ ls
    7357584         bin
    Desktop         blog_setup.log
    Desktops        chaotica
    Documents       code
    Downloads       flashcard.rb
    Dropbox         fractals
    Finances        gisttest
    HorrificallyCreativeUsesOfMummies.pdf inkscapeStuff
    Library         jekyllstart.log
    Movies          local
    Music         names.rb
    OpenSource        pear
    Passwordless-Loggin-to-a-Server.md  public_vs_private
    Personal        root@tararoys.com~
    Pictures        ruby_flashcards
    Plain_svg.svg       src
    Public          tara
    Random params 1.chaos     temp
    Random params 2.chaos     the_self_keyword
    Salamanders       tmp
    Screencasts       twilio-research.log
    Socrates        typescript
    TarasBlog       writing

    -----------------------fixing badly-linked css style sheet-------------------------------

    Last login: Sun Mar 30 20:50:42 on ttys001
    Taras-MacBook-Air:~ tlroys$ script ~/Desktop/jekyll_fix_css.log
    Script started, output file is /Users/tlroys/Desktop/jekyll_fix_css.log
    bash-3.2$ cd ~/Desktop
    bash-3.2$ cd documentation-made-painless/
    bash-3.2$ ls
    _config.yml _posts    css
    _layouts  _site   index.html
    bash-3.2$ mkdir _includes
    bash-3.2$ cd _includes/
    bash-3.2$ touch head.html
    bash-3.2$ touch foot.html
```

 {%endraw%} 
 It’s always useful to be able to pull in snippets of content onto pages, such as the header and footer, so they only need to be updated in one place. That’s what an _includes folder is for in Jekyll. Create a folder in the root called _includes, and within it add two files: head.html and foot.html. 

 this info is from the tutorial I copied here: /Users/tlroys/Desktop/GettingStartedWithJekyll/013-help-from-the-issue-tracker/03-wish-I-had-seen-this-before.html  

 That tutorial lives here on the internets: http://24ways.org/2013/get-started-with-github-pages/ 

 Now it is time to make the head 

'In head.html, paste the following:
 {%raw%} 

```html
     <!DOCTYPE html>
     <html>
         <head>
             <meta charset="utf-8">
             <title>{{ page.title }}</title>
             <link rel="stylesheet" href="{{ site.baseurl }}/css/main.css" >
         </head>
         <body>
     '
```

{%endraw%} 


echo "and in foot.html:
 

{%raw%} 
```bash 
    > </body>
    > </html>"
    > 
```
{%endraw%} 

bash-3.2$ echo "Whenever we want to pull in something from the _includes folder, we can use the liquid {%raw%} {% include filename.html %}{%endraw%}  in the layout file — I’ll show you how to set that up in next step."

In our directory, there’s a folder called _layouts and this lets us create a reusable template for pages. Inside that is a default.html file. Delete everything in default.html and paste in this instead:

{%raw%} 
```bash   
 {% include head.html %}
    > 
    >     <h1>{{ page.title }}</h1>
    > 
    >     {{ content }}
    > 
    > {% include foot.html %}"
    {% include head.html %}

        <h1>{{ page.title }}</h1>

        {{ content }}

    {% include foot.html %}
```
{%endraw%}

That’s a very basic page with a header, footer, page title and some content. To apply this template to a page, go back into the index.html page and add this snippet to the very top of the file:

{%raw%} 
```bash 

    > ---
    > layout: default
    > title: Home
    > ---"

```
{%endraw%}

"Now save the index.html file and hit Refresh in the browser. We should see a heading where {{ page.title }} was in the layout, which matches what comes after title: on the page itself (in this case, Home). So, if we wanted a subheading to appear on every page, we could add {{ page.subheading }} to where we want it to appear in our layout file, and a line that says subheading: This is a subheading in between the dashes at the top of the page itself.

{%raw%} 

```bash 

    bash-3.2$ ls
    foot.html head.html
    bash-3.2$ cd ..
    bash-3.2$ ls
    _config.yml _layouts  _site   index.html
    _includes _posts    css
    bash-3.2$ jekyll serve --baseurl ''
    Configuration file: /Users/tlroys/Desktop/documentation-made-painless/_config.yml
                Source: /Users/tlroys/Desktop/documentation-made-painless
           Destination: /Users/tlroys/Desktop/documentation-made-painless/_site
          Generating... done.
        Server address: http://0.0.0.0:4000
      Server running... press ctrl-c to stop.
 ```

 {%endraw%} 
 this for some reason centers the text on the page. I do not li this." 

 I bet it is because something is wrong with the css." 

 At the moment I do not care. I want a css stylesheet linked on gh-pages. I do not care if it looks pretty yet." 
 {%raw%} 

```bash    

    bash-3.2$ git status
    On branch master
    Your branch is up-to-date with 'origin/master'.

    Changes not staged for commit:
      (use "git add <file>..." to update what will be committed)
      (use "git checkout -- <file>..." to discard changes in working directory)

      modified:   _layouts/default.html
      modified:   index.html

    Untracked files:
      (use "git add <file>..." to include in what will be committed)

      _includes/

    no changes added to commit (use "git add" and/or "git commit -a")
    bash-3.2$ jekyll serve --baseurl ''Configuration file: /Users/tlroys/Desktop/documentation-made-painless/_config.yml
                Source: /Users/tlroys/Desktop/documentation-made-painless
           Destination: /Users/tlroys/Desktop/documentation-made-painless/_site
          Generating... done.
        Server address: http://0.0.0.0:4000
      Server running... press ctrl-c to stop.
    ^Cbash-3.2$ git add .
    bash-3.2$ git commit
    [master 64d2231] Attempt to attach css stylesheet using a baseurl
     4 files changed, 18 insertions(+), 45 deletions(-)
     create mode 100644 _includes/foot.html
     create mode 100644 _includes/head.html
     rewrite _layouts/default.html (99%)
    bash-3.2$ git branch
      gh-pages
    * master
    bash-3.2$ git checkout gh-pages
    Switched to branch 'gh-pages'
    bash-3.2$ git merge master
    Updating 2693c8a..64d2231
    Fast-forward
     _includes/foot.html   |  2 ++
     _includes/head.html   |  8 ++++++++
     _layouts/default.html | 45 ++++-----------------------------------------
     index.html            |  2 +-
     4 files changed, 15 insertions(+), 42 deletions(-)
     create mode 100644 _includes/foot.html
     create mode 100644 _includes/head.html
    bash-3.2$ git push origin gh-pages
    Username for 'https://github.com': tararoys
    Password for 'https://tararoys@github.com': 
    Counting objects: 12, done.
    Delta compression using up to 2 threads.
    Compressing objects: 100% (7/7), done.
    Writing objects: 100% (8/8), 1.06 KiB | 0 bytes/s, done.
    Total 8 (delta 3), reused 0 (delta 0)
    To https://github.com/tararoys/simple-documentation-process.git
       2693c8a..64d2231  gh-pages -> gh-pages
 ```

 {%endraw%} 
 remember to delete that password from the script log, and set up that ssh stuff so you don't have to remember to delete the password, you fool.

 And everything on http://tararoys.github.io/simple-documentation-process/jekyll/update/2014/03/30/welcome-to-jekyll.html is now center-justified. Yay!  Therefore it worked.  Next task: fix the center-justification." 
 
 {%raw%} 

```bash


    ------------------Responsive CSS and rendering Console Logs----------------
    Taras-MacBook-Air:JekyllBlogSetup tlroys$ cd documentation-made-painless/
    Taras-MacBook-Air:documentation-made-painless tlroys$ ls
    _config.yml _layouts    _site       index.html
    _includes   _posts      css
    Taras-MacBook-Air:documentation-made-painless tlroys$ subl .
    Taras-MacBook-Air:documentation-made-painless tlroys$ script ~/Desktop/jekyl_debugging_css.log
    Script started, output file is /Users/tlroys/Desktop/jekyl_debugging_css.log
    bash-3.2$ jekyll serve -baseurl ''
    Configuration file: /Users/tlroys/Desktop/JekyllBlogSetup/documentation-made-painless/_config.yml
                Source: /Users/tlroys/Desktop/JekyllBlogSetup/documentation-made-painless
           Destination: /Users/tlroys/Desktop/JekyllBlogSetup/documentation-made-painless/_site
          Generating...   Liquid Exception: Included file '/Users/tlroys/Desktop/JekyllBlogSetup/documentation-made-painless/_includes/filename.html' not found in _posts/2014-03-31-simpler-documentation-with-a-jekyll-blog.markdown
    error: Included file '/Users/tlroys/Desktop/JekyllBlogSetup/documentation-made-painless/_includes/filename.html' not found. Use --trace to view backtrace
    bash-3.2$ mv _posts/2014-03-31-simpler-documentation-with-a-jekyll-blog.markdown ~/Desktop
    bash-3.2$ echo 'I will debug th markdown of that post later'
    I will debug th markdown of that post later
    bash-3.2$ jekyll serve -baseurl ''Configuration file: /Users/tlroys/Desktop/JekyllBlogSetup/documentation-made-painless/_config.yml
                Source: /Users/tlroys/Desktop/JekyllBlogSetup/documentation-made-painless
           Destination: /Users/tlroys/Desktop/JekyllBlogSetup/documentation-made-painless/_site
          Generating... done.
        Server address: http://0.0.0.0:4000
      Server running... press ctrl-c to stop.
    ^Cbash-3.2$ jekyll build
    Configuration file: /Users/tlroys/Desktop/JekyllBlogSetup/documentation-made-painless/_config.yml
                Source: /Users/tlroys/Desktop/JekyllBlogSetup/documentation-made-painless
           Destination: /Users/tlroys/Desktop/JekyllBlogSetup/documentation-made-painless/_site
          Generating... done.
    bash-3.2$ jekyll serve --baseurl ''
    Configuration file: /Users/tlroys/Desktop/JekyllBlogSetup/documentation-made-painless/_config.yml
                Source: /Users/tlroys/Desktop/JekyllBlogSetup/documentation-made-painless
           Destination: /Users/tlroys/Desktop/JekyllBlogSetup/documentation-made-painless/_site
          Generating... done.
        Server address: http://0.0.0.0:4000
      Server running... press ctrl-c to stop.
    ^Cbash-3.2$ jekyll serve --baseurl ''
    Configuration file: /Users/tlroys/Desktop/JekyllBlogSetup/documentation-made-painless/_config.yml
                Source: /Users/tlroys/Desktop/JekyllBlogSetup/documentation-made-painless
           Destination: /Users/tlroys/Desktop/JekyllBlogSetup/documentation-made-painless/_site
          Generating... done.
        Server address: http://0.0.0.0:4000
      Server running... press ctrl-c to stop.
 ```

 {%endraw%} 
 I am going to borrow the css from http://tararoys.github.io/AdnturesInDns/ to see if I can make this blog look better.  I would like to have a responsive website without having to learn how to write my own css, and this seesm like a good way to do it." 
 {%raw%} 

```bash

    bash-3.2$ jekyll serve --baseurl ''Configuration file: /Users/tlroys/Desktop/JekyllBlogSetup/documentation-made-painless/_config.yml            Source: /Users/tlroys/Desktop/JekyllBlogSetup/documentation-made-painless
           Destination: /Users/tlroys/Desktop/JekyllBlogSetup/documentation-made-painless/_site
          Generating... done.
        Server address: http://0.0.0.0:4000
      Server running... press ctrl-c to stop.
    ^Cbash-3.2$ git rm css/main.css 
    error: the following file has local modifications:
        css/main.css
    (use --cached to keep the file, or -f to force removal)
    bash-3.2$ git status
    On branch gh-pages
    Changes not staged for commit:
      (use "git add/rm <file>..." to update what will be committed)
      (use "git checkout -- <file>..." to discard changes in working directory)

        modified:   _includes/head.html
        modified:   _layouts/default.html
        deleted:    _posts/2014-03-31-simpler-documentation-with-a-jekyll-blog.markdown
        modified:   css/main.css

    Untracked files:
      (use "git add <file>..." to include in what will be committed)

        css/stylesheet.css

    no changes added to commit (use "git add" and/or "git commit -a")
    bash-3.2$ git add .
    warning: You ran 'git add' with neither '-A (--all)' or '--ignore-removal',
    whose behaviour will change in Git 2.0 with respect to paths you removed.
    Paths like '_posts/2014-03-31-simpler-documentation-with-a-jekyll-blog.markdown' that are
    removed from your working tree are ignored with this version of Git.

    * 'git add --ignore-removal <pathspec>', which is the current default,
      ignores paths you removed from your working tree.

    * 'git add --all <pathspec>' will let you also record the removals.

    Run 'git status' to check the paths you removed from your working tree.

    bash-3.2$ git status
    On branch gh-pages
    Changes to be committed:
      (use "git reset HEAD <file>..." to unstage)

        modified:   _includes/head.html
        modified:   _layouts/default.html
        modified:   css/main.css
        new file:   css/stylesheet.css

    Changes not staged for commit:
      (use "git add/rm <file>..." to update what will be committed)
      (use "git checkout -- <file>..." to discard changes in working directory)

        deleted:    _posts/2014-03-31-simpler-documentation-with-a-jekyll-blog.markdown

    bash-3.2$ git add -u
    bash-3.2$ git status
    On branch gh-pages
    Changes to be committed:
      (use "git reset HEAD <file>..." to unstage)

        modified:   _includes/head.html
        modified:   _layouts/default.html
        deleted:    _posts/2014-03-31-simpler-documentation-with-a-jekyll-blog.markdown
        modified:   css/main.css
        new file:   css/stylesheet.css

    bash-3.2$ git commit
    [gh-pages 7b2fc0a] Made blog look prettier
     5 files changed, 440 insertions(+), 980 deletions(-)
     delete mode 100644 _posts/2014-03-31-simpler-documentation-with-a-jekyll-blog.markdown
     create mode 100644 css/stylesheet.css
    bash-3.2$ git push origin gh-pages
    Username for 'https://github.com': tararoys
    Password for 'https://tararoys@github.com': 
    Counting objects: 24, done.
    Delta compression using up to 2 threads.
    Compressing objects: 100% (13/13), done.
    Writing objects: 100% (13/13), 14.14 KiB | 0 bytes/s, done.
    Total 13 (delta 4), reused 0 (delta 0)
    To https://github.com/tararoys/simple-documentation-process.git
       64d2231..7b2fc0a  gh-pages -> gh-pages
    bash-3.2$ git status
    On branch gh-pages
    nothing to commit, working directory clean
    bash-3.2$ mv ~/Desktop/
    .DS_Store
    .gitignore
    .localized
    .rspec
    .ruby-version
    .swp
    2014-03-31-simpler-documentation-with-a-jekyll-blog.markdown
    FoxJobHunting/
    JekyllBlogSetup/
    Linked-In-Profile/
    alan_interview/
    jekyl_debugging_css.log
    node_blog_debugging/
    bash-3.2$ mv ~/Desktop/
    .DS_Store
    .gitignore
    .localized
    .rspec
    .ruby-version
    .swp
    2014-03-31-simpler-documentation-with-a-jekyll-blog.markdown
    FoxJobHunting/
    JekyllBlogSetup/
    Linked-In-Profile/
    alan_interview/
    jekyl_debugging_css.log
    node_blog_debugging/
    bash-3.2$ mv ~/Desktop/2014-03-31-simpler-documentation-with-a-jekyll-blog.markdown _posts/
    bash-3.2$ ls
    _config.yml _layouts    _site       index.html
    _includes   _posts      css
 ```

 {%endraw%} 

 Now that css is fixed to my satisfaction, I am going to create a blog that is just a log of all of the shell commands I used to learn how to create a jekyll blog."

 If I recall correctly, when I try to run this blog with this post, it will give me a markdown error. 
 {%raw%} 

```bash
bash-3.2$ jekyll serve --baseurl ''Configuration file: /Users/tlroys/Desktop/JekyllBlogSetup/documentation-made-painless/_config.yml
            Source: /Users/tlroys/Desktop/JekyllBlogSetup/documentation-made-painless
       Destination: /Users/tlroys/Desktop/JekyllBlogSetup/documentation-made-painless/_site
      Generating...   Liquid Exception: Included file '/Users/tlroys/Desktop/JekyllBlogSetup/documentation-made-painless/_includes/filename.html' not found in _posts/2014-03-31-simpler-documentation-with-a-jekyll-blog.markdown
error: Included file '/Users/tlroys/Desktop/JekyllBlogSetup/documentation-made-painless/_includes/filename.html' not found. Use --trace to view backtrace
bash-3.2$ jekyll serve --baseurl '' --trace
Configuration file: /Users/tlroys/Desktop/JekyllBlogSetup/documentation-made-painless/_config.yml
            Source: /Users/tlroys/Desktop/JekyllBlogSetup/documentation-made-painless
       Destination: /Users/tlroys/Desktop/JekyllBlogSetup/documentation-made-painless/_site
      Generating...   Liquid Exception: Included file '/Users/tlroys/Desktop/JekyllBlogSetup/documentation-made-painless/_includes/filename.html' not found in _posts/2014-03-31-simpler-documentation-with-a-jekyll-blog.markdown
/Users/tlroys/.rvm/gems/ruby-2.0.0-p353/gems/jekyll-1.5.1/lib/jekyll/tags/include.rb:114:in `validate_path': Included file '/Users/tlroys/Desktop/JekyllBlogSetup/documentation-made-painless/_includes/filename.html' not found (IOError)
    from /Users/tlroys/.rvm/gems/ruby-2.0.0-p353/gems/jekyll-1.5.1/lib/jekyll/tags/include.rb:96:in `render'
    from /Users/tlroys/.rvm/gems/ruby-2.0.0-p353/gems/liquid-2.5.5/lib/liquid/block.rb:106:in `block in render_all'
    from /Users/tlroys/.rvm/gems/ruby-2.0.0-p353/gems/liquid-2.5.5/lib/liquid/block.rb:93:in `each'
    from /Users/tlroys/.rvm/gems/ruby-2.0.0-p353/gems/liquid-2.5.5/lib/liquid/block.rb:93:in `render_all'
    from /Users/tlroys/.rvm/gems/ruby-2.0.0-p353/gems/liquid-2.5.5/lib/liquid/block.rb:82:in `render'
    from /Users/tlroys/.rvm/gems/ruby-2.0.0-p353/gems/liquid-2.5.5/lib/liquid/template.rb:124:in `render'
    from /Users/tlroys/.rvm/gems/ruby-2.0.0-p353/gems/liquid-2.5.5/lib/liquid/template.rb:132:in `render!'
    from /Users/tlroys/.rvm/gems/ruby-2.0.0-p353/gems/jekyll-1.5.1/lib/jekyll/convertible.rb:88:in `render_liquid'
    from /Users/tlroys/.rvm/gems/ruby-2.0.0-p353/gems/jekyll-1.5.1/lib/jekyll/convertible.rb:150:in `do_layout'
    from /Users/tlroys/.rvm/gems/ruby-2.0.0-p353/gems/jekyll-1.5.1/lib/jekyll/post.rb:259:in `render'
    from /Users/tlroys/.rvm/gems/ruby-2.0.0-p353/gems/jekyll-1.5.1/lib/jekyll/site.rb:239:in `block in render'
    from /Users/tlroys/.rvm/gems/ruby-2.0.0-p353/gems/jekyll-1.5.1/lib/jekyll/site.rb:238:in `each'
    from /Users/tlroys/.rvm/gems/ruby-2.0.0-p353/gems/jekyll-1.5.1/lib/jekyll/site.rb:238:in `render'
    from /Users/tlroys/.rvm/gems/ruby-2.0.0-p353/gems/jekyll-1.5.1/lib/jekyll/site.rb:39:in `process'
    from /Users/tlroys/.rvm/gems/ruby-2.0.0-p353/gems/jekyll-1.5.1/lib/jekyll/command.rb:18:in `process_site'
    from /Users/tlroys/.rvm/gems/ruby-2.0.0-p353/gems/jekyll-1.5.1/lib/jekyll/commands/build.rb:23:in `build'
    from /Users/tlroys/.rvm/gems/ruby-2.0.0-p353/gems/jekyll-1.5.1/lib/jekyll/commands/build.rb:7:in `process'
    from /Users/tlroys/.rvm/gems/ruby-2.0.0-p353/gems/jekyll-1.5.1/bin/jekyll:97:in `block (2 levels) in <top (required)>'
    from /Users/tlroys/.rvm/gems/ruby-2.0.0-p353/gems/commander-4.1.6/lib/commander/command.rb:180:in `call'
    from /Users/tlroys/.rvm/gems/ruby-2.0.0-p353/gems/commander-4.1.6/lib/commander/command.rb:180:in `call'
    from /Users/tlroys/.rvm/gems/ruby-2.0.0-p353/gems/commander-4.1.6/lib/commander/command.rb:155:in `run'
    from /Users/tlroys/.rvm/gems/ruby-2.0.0-p353/gems/commander-4.1.6/lib/commander/runner.rb:422:in `run_active_command'
    from /Users/tlroys/.rvm/gems/ruby-2.0.0-p353/gems/commander-4.1.6/lib/commander/runner.rb:82:in `run!'
    from /Users/tlroys/.rvm/gems/ruby-2.0.0-p353/gems/commander-4.1.6/lib/commander/delegates.rb:8:in `run!'
    from /Users/tlroys/.rvm/gems/ruby-2.0.0-p353/gems/commander-4.1.6/lib/commander/import.rb:10:in `block in <top (required)>'
2044488/jekyll-code-in-jekyll" be solved by http://stackoverflow.com/questions/2 

```
{%endraw%} 

This error can be solved by http://stackoverflow.com/questions/22044488/jekyll-code-in-jekyll
The {%raw%}{%...%}{%endraw%} 
 syntax used by Jekyll is part of the Liquid templating engine. To escape these tags, and so show them literally, you should use the raw tag.

You will probably want to combine this with the markdown syntax for code blocks. With Redcarpet you can use the triple backtick syntax. It doesn’t matter if you put the backticks inside the raw tags or the other way round.

NOTE: had pasted code from stack overflow into this log.  This was a bad idea, because jekyll interpreted the liquid tags in the code snippit as liquid tags and not as a code snippet precisely because I was using the liquid raw and end raw tags in the code snippet. So visit the stack overflow to see the snippet in it's full glory. 

You will probably want to combine this with the markdown syntax for code blocks. With Redcarpet you can use the triple backtick syntax. It doesn’t matter if you put the backticks inside the raw tags or the other way round:
{%raw%}

```bash
bash-3.2$ jekyll server --baseurl ''
Configuration file: /Users/tlroys/Desktop/JekyllBlogSetup/documentation-made-painless/_config.yml
            Source: /Users/tlroys/Desktop/JekyllBlogSetup/documentation-made-painless
       Destination: /Users/tlroys/Desktop/JekyllBlogSetup/documentation-made-painless/_site
      Generating... done.
    Server address: http://0.0.0.0:4000
  Server running... press ctrl-c to stop.
^Cbash-3.2$ jekyll server --baseurl '' -w
Configuration file: /Users/tlroys/Desktop/JekyllBlogSetup/documentation-made-painless/_config.yml
            Source: /Users/tlroys/Desktop/JekyllBlogSetup/documentation-made-painless
       Destination: /Users/tlroys/Desktop/JekyllBlogSetup/documentation-made-painless/_site
      Generating...   Liquid Exception: Tag '{%' was not properly terminated with regexp: /\%\}/ in _posts/2014-03-31-simpler-documentation-with-a-jekyll-blog.markdown
error: Tag '{%' was not properly terminated with regexp: /\%\}/ . Use --trace to view backtrace
bash-3.2$ git status
On branch gh-pages
Untracked files:
  (use "git add <file>..." to include in what will be committed)

    _posts/2014-03-31-simpler-documentation-with-a-jekyll-blog.markdown

nothing added to commit but untracked files present (use "git add" to track)
bash-3.2$ jekyll server --baseurl '' -w
Configuration file: /Users/tlroys/Desktop/JekyllBlogSetup/documentation-made-painless/_config.yml
            Source: /Users/tlroys/Desktop/JekyllBlogSetup/documentation-made-painless
       Destination: /Users/tlroys/Desktop/JekyllBlogSetup/documentation-made-painless/_site
      Generating... done.
 Auto-regeneration: enabled
    Server address: http://0.0.0.0:4000
  Server running... press ctrl-c to stop.
      Regenerating: 1 files at 2014-04-01 07:33:22 ...done.
      Regenerating: 1 files at 2014-04-01 07:33:53 ...done.
      Regenerating: 1 files at 2014-04-01 07:34:07 ...done.
      Regenerating: 1 files at 2014-04-01 07:34:22 ...done.
      Regenerating: 1 files at 2014-04-01 07:35:23 ...done.
```
{%endraw%}


And I now have a raw log. With the caveat that I can't paste liquid raw tags into the echo output and expect jekyll to process it correctly.  

I used the regex 
```regex
       \^Cbash-3.2\$ echo "(.*)\n
```
to find all of the echos in this log, and replaced them with markdown and liquid tags that I can't right down right now because this log interprets them as actual markdown and liquid tags.  Things suddenly got very meta.

