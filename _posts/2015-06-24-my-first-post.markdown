---
layout:     post
title:      "Making a GitHub Website 101"
subtitle:   "By a scrub, for scrubs"
date:       2015-06-24 13:40:00
author:     "Dylan Franco"
header-img: "img/img2-2.jpg"
---

<p>Aloha! If you are reading this, you are most likely having a hard time making a website on GitHub, and that makes me sad :(. You are, however, in the right place to learn how to be able to set up a basic blog website! This tutorial was written by a scrub, for scrubs. Note that during the tutorial, when I type two different lines of code make sure you type each of them in correctly and in order.</p>

<h2 class="section-heading">Step 1: Gather Materials</h2>

<p>Before you start, you're going to need a few materials:</p>
<p>Ruby Interpretor Dev Kit: <a href="https://www.ruby-lang.org/en/installation/" target="_blank">Ruby-lang.org</a></p>
<p>GitHub account: <a href="http://www.github.com" target="_blank">GitHub.com</a></p>
<p>GitHub for Windows/Mac: We'll get to this later</p>
<p>Free Editor: <a href="http://www.sublimetext.com" target="_blank">Sublime Text 2</a></p>
<h2 class="section-heading">Step 2: Get Set Up!</h2>
<p>Alright, so you just installed all of this stuff, but what does it have to do with the website? Don't worry about it. You'll figure this stuff out as we go along with the tutorial.</p>
<p>So what you should do now (if you haven't already) is set your email and name in Git. Open "Git Bash" and type in:</p>
<p>git config --global user.name "Your Name"</p>
<p>user.name should say user.name, and "Your Name" is not your GitHub username. Now type this:</p>
<p>git config --global user.email "your_email@whatever.com"</p>
<p>Next, Mac users will type in:</p>
<p>git config --global core.autocrlf input</p>
<p>git config --global core.safecrlf true</p>
<p>Next for Windows users:</p>
<p>git config --global core.autocrlf true</p>
<p>git config --global core.safecrlf true</p>
<p>This is just setting some background stuff up that you don't have to worry about anymore. Next thing we're going to do is set up a repository in GitHub.</p>
<p>Open up GitHub.com in your favorite browser and log into your account. In the top right corner there's a little plus sign next to a down arrow. Click on it and select "New Repository." When asked to name your repository (THIS IS REALLY IMPORTANT) name it:</p>
<p>UserName.github.io</p>
<p>Now here is where you replace "Username" with your actual GitHub username instead. This tells GitHub that you're gonna be using this repository as a free GitHub website. Everybody gets one (but you knew that already, that's why you're here). Now we're ready to</p>

<h2 class="section-heading">Step 3: The Clone Wars</h2>

<p>Now that you've made this repository, we need to make a repository on your computer. There are two ways to do this: Cloning is the easier way, but if you want to learn something you'll do it manually. If you're lazy you can skip to "Step 3b: Cloning." Now that the weaklings are gone, it's time for</p>

<h2 class="section-heading">Step 3a: Setting up a local repository</h2>
<p>Go into Explorer (Or Finder for Mac) and make a folder in your Desktop folder called "websiterepo" (no space or caps, it'll make it easier on you). Now go into Git Bash and type "ls" and hit enter.</p>
<h2 class="section-heading">What's this list?</h2>
<p>What it is happens to be a list of all the folders on your user account. Reading through these you'll see one that says "Desktop." What we're going to type in now is "cd Desktop" and hit enter. Try that "ls" again.</p>
<h2 class="section-heading">WOW!</h2>
<p>Hopefully your desktop isn't too cluttered, otherwise that may have been a long list. Looking through this list we see "websiterepo."  This time, we're going to type in "cd webs" and then before pushing enter we're gonna hit the TAB button. You'll see that it fills in the rest for you! Programmers are lazy people, so this one comes in handy.</p>
<p>What you're gonna do next is type in "git status" and notice that I lied to you. This isn't a repository... Yet. Type in "git init" and watch git magically turn this folder into a repository. Next (in your browser) open the website's repository on GitHub.</p>
<h2 class"section-heading"> Setting an Origin (Last step)</h2>
<p>If you look at the top of the screen next to the "Set up in Desktop" button there is a url in a box. It should say "https://github.com/Username/Username.github.io.git" in it. In Git Bash, type "git remote add origin https://github.com/Username/Username.github.io.git" and hit enter. Now type "git remote -v" and make sure that the url next to origin is the correct one. Now type in the following two lines. Note that while typing in your GitHub Password you will not be able to see what you are typing.</p>
<p>git commit -m "first commit"</p>
<p>git push -u origin master</p>
<p>All done! You're now ready to move onto the next step! Note: From Step 4 onwards, I will assume you know how to reach your repo on your computer by yourself.</p>
<h2 class="section-heading">Step 3b: Cloning"</h2>
<p>Cloning is just a fancy way of saying we're copying this repository onto our own computers. In your repo in the browser, there should be a button that says "Quick setup in Desktop." Click on it, and it will ask you to install GitHub for your OS (I recommend doing so). After installing it, open the GitHub.exe that was put on your Desktop.</p>
<p>After signing in, there should be a list of your GitHub repositories on the left side, but you don't have any cloned yet. There should also be a familiar plus sign with a downwards arrow at the top of the screen. Click on it and push "Clone" and select the repository that we made. Select "Desktop" and begin cloning your repo! The process should only take a few seconds. After, the repo list to the left will show the name of your repo! Also, there should be a folder on your desktop named how your repo is. Open up "Git Bash" and type in the following:</p>
<p>cd Desktop</p>
<p>Now type in "cd Username" and push TAB. Make sure that where I put Username you put your actual userame. It will fill in the rest of the name and then you press enter. Congratulations! You cloned a repo from GitHub! Now type in the following two lines. Note that while typing in your GitHub Password you will not be able to see what you are typing.</p>
<p>git commit -m "first commit"</p>
<p>git push -u origin master</p>
<p>All done!</p>
<h2 class="selection-heading">Step 4: Making a Commit</h2>
<p>Open up Sublime Text 2 and save this empty document as "index.html" into your repository folder. In Sublime Text 2, enter the following into your index.html file:</p>
<p><textarea><h1>Hello World!</h1></textarea></p>
<p>Now save the document and return to Git Bash. While in your repository (in Git Bash) type "ls" and hit enter, you should see your index.html file there! Now what we're going to type into Bash is VERY important.</p>
<p>git status</p>
<p>What that did was allow us to see what needs to be "added" in order to be "pushed" to GitHub. Don't worry what those terms mean for now if you don't already. I'll show you how to do this all very easily. Type the following.
<p>git add index.html</p>
<p>If you do another "git status" you will notice that the status of your index.html has changed to "added." In Windows the color changes from red to green. Now that we have "added" index.html, we need to "commit" it and "push" it to our online repository. Type the following:</p>
<p>git commit -m "Type a message here"</p>
<p>git push origin</p>
<p>Refresh your Internet Browser window and you should see that you have added your index.html to your new website! You wanna see what it looks like so far? Open a new tab in your browser and in the address bar type in "Username.github.io" and hit enter. There's your new site! Though, there isn't much here. Let's change that.</p>
<h2 class="selection-heading">Adding a Template</h2>
<p>Close up Git Bash and reopen it to quickly get back to the first directory (or type "cd .." and hit enter until it no longer shows desktop/reponame). After opening it type in the following:</p>
<p>gem install jekyll</p>
<p>Jekyll is a GitHub based website builder that will run in the background while we make this site. It may take a while to download but don't worry, I'll be here for you. If you skipped it, you may want to go back and read Step 3a. Jekyll's done? yay! Time to download a template.</p>
<p>Head over to <a href="http://startbootstrap.com/template-overviews/clean-blog/" target="_blank">startbootstrap</a> and scroll down to the "Jekyll Version" and click the link. This will bring you to someone else's repository on GitHub with a lot of files in it. We need them all, so what we're gonna do is select the "Clone to Desktop" option on the right. The GitHub you downloaded should open and ask you where to save this new repository. Select the same one as your own repository and hit save.</p>
<p>After all of the files download, we're going to open up this new repository in our explorer (finder) and copy/paste all of these files into our own repository EXCEPT for the README. Once that is done, navigate your way back to your own repo in Git Bash and do a "git status". You'll notice that there's a lot of stuff that needs adding, but we don't have time for all of that. Instead, we're going to do the lazy thing and type in the following:</p>
<p>git add --all</p>
<p>Doing another status check shows that everything's green and ready for commit. Type the following:</p>
<p>git commit -m "We added a template!"</p>
<p>git push origin</p>
<p>This may take a little while to push, but there's a lot of stuff you just added! After the push is done, go back into your browser and type in your url again (or refresh the page if it's still open) and marvel at your new website!
<a href="#">
    <img src="{{ site.baseurl }}/img/img1.jpg" alt="Hunter Titan and Warlock">
</a>
<span class="caption text-muted">I like to play Destiny.</span>