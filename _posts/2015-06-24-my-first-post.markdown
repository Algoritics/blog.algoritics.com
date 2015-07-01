---
layout:     post
title:      "Making a GitHub Website 101"
subtitle:   "By a scrub, for scrubs"
date:       2015-06-30 19:45:00
author:     "Dylan Franco"
header-img: "img/img2-2.jpg"
---
<h2 class="selection-heading">Aloha!</h2>

<p>If you are reading this, you are most likely having a hard time making a website on GitHub, and that makes me sad :(. You are, however, in the right place to learn how to be able to set up a basic blog website! This tutorial was written by a scrub, for scrubs. Note that during the tutorial, when I type two different lines of code make sure you type each of them in correctly and in order.</p>

<h2 class="section-heading">Step 1: Gather Materials</h2>

<p>Before you start, you're going to need a few materials:</p>
<p>Ruby Interpretor Dev Kit: <a href="https://www.ruby-lang.org/en/installation/" target="_blank">Ruby-lang.org</a></p>
<p>GitHub account: <a href="http://www.github.com" target="_blank">GitHub.com</a></p>
<p>GitHub for Windows/Mac: We'll get to this later</p>
<p>Free Editor: <a href="http://www.sublimetext.com" target="_blank">Sublime Text 2</a></p>
<h2 class="section-heading">Step 2: Get Set Up!</h2>
<p>Alright, so you just installed all of this stuff, but what does it have to do with the website? Don't worry about it. You'll figure this stuff out as we go along with the tutorial.</p>
<p>So what you should do now (if you haven't already) is set your email and name in Git. Open "Git Bash" and type in:</p>
<p><i>git config --global user.name "Your Name"</i></p>
<p>user.name should say user.name, and "Your Name" is not your GitHub username. Now type this:</p>
<p><i>git config --global user.email "your_email@whatever.com"</i></p>
<p>Next, Mac users will type in:</p>
<p><i>git config --global core.autocrlf input</i></p>
<p><i>git config --global core.safecrlf true</i></p>
<p>Next for Windows users:</p>
<p><i>git config --global core.autocrlf true</i></p>
<p><i>git config --global core.safecrlf true</i></p>
<p>This is just setting some background stuff up that you don't have to worry about anymore. Next thing we're going to do is set up a repository in GitHub.</p>
<p>Now type in the following:</p>
<p><i>gem install jekyll</i></p>
<p>Jekyll is a GitHub based website builder that will run in the background while we make this site. It may take a while to download but don't worry, I'll be here for you.</p>
<p>Open up GitHub.com in your favorite browser and log into your account. In the top right corner there's a little plus sign next to a down arrow. Click on it and select "New Repository." When asked to name your repository (THIS IS REALLY IMPORTANT) name it:</p>
<p><i>UserName.github.io</i></p>
<p>Now here is where you replace "Username" with your actual GitHub username instead. Make sure that you spell it exactly how you spelt it during signup. This tells GitHub that you're gonna be using this repository as a free GitHub website. Everybody gets one (but you knew that already, that's why you're here). Now we're ready to</p>

<h2 class="section-heading">Step 3: Cloning</h2>

<p>Now that you've made this repository, we need to make a repository on your computer. There are two ways to do this: Cloning is the easier way, but if you want to learn something you'll do it manually. If you're lazy you can skip to "Step 3b: Cloning." Now it's time for</p>

<h2 class="section-heading">Step 3a: Setting up a local repository</h2>
<p>Go into Explorer (Or Finder for Mac) and make a folder in your Desktop folder called "websiterepo" (no space or caps, it'll make it easier on you). Now go into Git Bash and type "<i>ls</i>" and hit enter.</p>
<h2 class="section-heading">What's this list?</h2>
<p>What it is happens to be a list of all the folders on your user account. Reading through these you'll see one that says "<i>Desktop</i>." What we're going to type in now is "<i>cd Desktop</i>" and hit enter. Try that "<i>ls</i>" again.</p>
<h2 class="section-heading">WOW!</h2>
<p>Hopefully your desktop isn't too cluttered, otherwise that may have been a long list. Looking through this list we see "<i>websiterepo</i>."  This time, we're going to type in "<i>cd webs</i>" and then before pushing enter we're gonna hit the <i>TAB</i> button. You'll see that it fills in the rest for you! Programmers are lazy people, so this one comes in handy.</p>
<p>What you're gonna do next is type in "<i>git status</i>" and notice that I lied to you. This isn't a repository... Yet. Type in "<i>git init</i>" and watch git magically turn this folder into a repository. Next (in your browser) open the website's repository on GitHub.</p>
<h2 class="section-heading"> Setting an Origin (Last step)</h2>
<p>If you look at the top of the screen next to the "<i>Set up in Desktop</i>" button there is a url in a box. It should say "<i>https://github.com/Username/Username.github.io.git</i>" in it. In Git Bash, type "<i>git remote add origin https://github.com/Username/Username.github.io.git</i>" and hit enter. Now type "<i>git remote -v</i>" and make sure that the url next to origin is the correct one. Now type in the following two lines. Note that while typing in your GitHub Password you will not be able to see what you are typing.</p>
<p><i>git commit -m "first commit"</i></p>
<p><i>git push -u origin master</i></p>
<p>All done! You're now ready to move onto the next step! Note: From Step 4 onwards, I will assume you know how to reach your repo on your computer by yourself. This just means using the "<i>cd</i>" command in Git Bash like we did before.</p>
<h2 class="section-heading">Step 3b: Cloning"</h2>
<p>Cloning is just a fancy way of saying we're copying this repository onto our own computers. In your repo in the browser, there should be a button that says "<i>Quick setup in Desktop</i>." Click on it, and it will ask you to install GitHub for your OS (I recommend doing so). After installing it, open the <i>GitHub.exe</i> that was put on your Desktop.</p>
<p>After signing in, there should be a list of your GitHub repositories on the left side, but you don't have any cloned yet. There should also be a familiar plus sign with a downwards arrow at the top of the screen. Click on it and push "<i>Clone</i>" and select the repository that we made. Select "<i>Desktop</i>" and begin cloning your repo! The process should only take a few seconds. After, the repo list to the left will show the name of your repo! Also, there should be a folder on your desktop named how your repo is. Open up "<i>Git Bash</i>" and type in the following:</p>
<p><i>cd Desktop</i></p>
<p>Now type in "<i>cd Username</i>" and push TAB. Make sure that where I put Username you put your actual userame. It will fill in the rest of the name and then you press enter. Congratulations! You cloned a repo from GitHub! Now type in the following two lines. Note that while typing in your GitHub Password you will not be able to see what you are typing.</p>
<p><i>git commit -m "first commit"</i></p>
<p><i>git push -u origin master</i></p>
<p>All done!</p>
<h2 class="selection-heading">Step 4: Making a Commit</h2>
<p>Open up Sublime Text 2 and save this empty document as "index.html" into your repository folder. In Sublime Text 2, enter the following into your index.html file:</p>
<p><textarea><h1>Hello World!</h1></textarea></p>
<p>Now save the document and return to Git Bash. While in your repository (in Git Bash) type "ls" and hit enter, you should see your index.html file there! Now what we're going to type into Bash is VERY important.</p>
<p><i>git status</i></p>
<p>What that did was allow us to see what needs to be "added" in order to be "pushed" to GitHub. Don't worry what those terms mean for now if you don't already. I'll show you how to do this all very easily. Type the following.
<p><i>git add index.html</i></p>
<p>If you do another "<i>git status</i>" you will notice that the status of your index.html has changed to "added." In Windows the color changes from red to green. Now that we have "added" index.html, we need to "commit" it and "push" it to our online repository. Type the following:</p>
<p><i>git commit -m "Type a message here"</i></p>
<p><i>git push origin</i></p>
<p>Refresh your Internet Browser window and you should see that you have added your index.html to your new website! You wanna see what it looks like so far? Open a new tab in your browser and in the address bar type in "<i>Username.github.io</i>" and hit enter. There's your new site! Though, there isn't much here. Let's change that.</p>
<h2 class="selection-heading">Adding a Template</h2>
	<p>Close up Git Bash and reopen it to quickly get back to the first directory (or type "<i>cd ..</i>" and hit enter until it no longer shows desktop/reponame). Now it's time to download a template.</p>
				<p>Head over to <a href="http://startbootstrap.com/template-overviews/clean-blog/" target="_blank">startbootstrap</a> and scroll down to the "<i>Jekyll Version</i>" and click the link. This will bring you to someone else's repository on GitHub with a lot of files in it. We need them all, so what we're gonna do is select the "<i>Clone to Desktop</i>" option on the right. The GitHub you downloaded should open and ask you where to save this new repository. Select the desktop and hit save.</p>
					<p>After all of the files download, we're going to open up this new repository in our explorer (finder) and copy/paste all of these files into our own repository EXCEPT for the README. Once that is done, navigate your way back to your own repo in Git Bash and do a "<i>git status</i>". You'll notice that there's a lot of stuff that needs adding, but we don't have time for all of that. Instead, we're going to do the lazy thing and type in the following:</p>
						<p><i>git add --all</i></p>
							<p>Doing another status check shows that everything's green and ready for commit. Type the following:</p>
								<p><i>git commit -m "We added a template!"</i></p>
									<p><i>git push origin</i></p>
										<p>This may take a little while to push, but there's a lot of stuff you just added! After the push is done, go back into your browser and type in your url again (or refresh the page if it's still open) and marvel at your new website!
	<h2 class="selection-heading">You're Done!</h2>
<p>Congrats! You made a random blog about nothing! Now it's time to make it your own. Here are some tips:</p>
<p>Read the README in the repo you downloaded from startbootstrap</p>
<p>The folder titled "img" in your repo is where to place all of your images that you would like to be on the website! If you want to put them in the middle of the page like the example below, you must type in the following:</p>
<p><textarea><a href="#">
    <img src="{{ site.baseurl }}/img/nameoftheimage.jpg" alt="Description of the image">
</a>
</textarea></p>
<p>To add a little flavor text underneath type this:</p>
<p><textarea><span class="caption text-muted">Place your text here!</span></textarea></p>
<a href="#">
    <img src="{{ site.baseurl }}/img/img1.jpg" alt="Hunter Titan and Warlock">
</a>
<span class="caption text-muted">I like to play Destiny, so here's a pic of the new DLC.</span>
<p>That's all for this tutorial. If you would like to learn more about Git and GitHub you can checkout this other tutorial by <a href="http://www.google.com/url?q=http%3A%2F%2Fgitimmersion.com%2Flab_01.html&sa=D&sntz=1&usg=AFQjCNEWqtc2edE91VozYDHSMzsRsc3FYA">Git Immersion</a> or one of the many resources at <a href="https://www.google.com/url?q=https%3A%2F%2Fhelp.github.com%2Farticles%2Fgood-resources-for-learning-git-and-github%2F&sa=D&sntz=1&usg=AFQjCNG3a55_gzsUmW5srX-ktUBfgyWr-w">GitHub.com</a>.</p>