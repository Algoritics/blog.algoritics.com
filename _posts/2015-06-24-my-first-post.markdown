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
<p>Free Editor: <a href="http://www.sublimetext.com" target="_blank">Sublime Text</a></p>
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

<p>Now that you've made this repository, we need to clone it to your computer. Cloning is just a fancy way of saying we're copying this repository onto our own computers. </p>

<a href="#">
    <img src="{{ site.baseurl }}/img/img1.jpg" alt="Hunter Titan and Warlock">
</a>
<span class="caption text-muted">I like to play Destiny.</span>