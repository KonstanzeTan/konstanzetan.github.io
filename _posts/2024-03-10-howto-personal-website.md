---
title:  "How I made this personal website using GitHub Pages"
mathjax: true
layout: post
categories: media
---

This workflow is largely based on an excellent, easy-to-follow YouTube tutorial by [Assistant Professor Kathryn Schuler](https://www.youtube.com/watch?v=qZsgPgGdOzQ). What makes this tutorial stand out from the myriads out there is that it’s entirely GUI-based, meaning that you can build a website from GitHub’s browser without needing the command line. This website is built using Jekyll: there are other generators around, but Jekyll has been optimised to work with GitHub Pages. In this post, I’ve rearranged the flow of the tutorial according to my actual implementation.  I will also be highlighting the features I found useful, and sharing the challenges I’d faced in case it may help with troubleshooting. I will be updating this document from time to time, as I continue building this website.

# Pre-requisites
- A GitHub account. 

# Choosing and setting up a theme
1. Log in to your GitHub account. 
2. Pick a theme from [jekyllthemes.io](https://jekyllthemes.io/). I'm using the free 'Contrast' theme for my website.
3. Click on your selected theme and preview it with 'Live Demo'. Typically, website-building instructions will be contained under the 'About' section.
4. Fork the repository of your Jekyll theme. The repository houses all files needed to build the website.
![fork repository](/assets/photos/1_fork_repo.png)


5. Enter the newly-forked repository and rename it.  after this step, people should be able to access your website at your given URL. 
	- Click on ‘Settings’, then change the name of this repository to <username>.github.io.

![change_repository_name](/assets/photos/2_change_repo_name.png)


	- Edit the repository details by navigating back to the main page of the repository, then clicking on ‘About’. In the popup window, edit the ‘Description’ and ‘Website’ fields. The website URL needs to follow this format: https://<yourusername>.github.io. ⚠️ It’s SUPER IMPORTANT to adhere to this URL format as this is what GitHub recognises to successfully build your website. Checking the ‘Use your GitHub Pages website’ box will automatically generate the correct URL.

![edit_repo_details](/assets/photos/3_edit_repo_details.png)


# Edit the configuration file (\_config.yml)
This file acts as your website's content page, determining what visitors first see and how they navigate to the information they want. Many academic websites include links to an updated CV. There are lots of things that we can play with on the config page, but for starters, I’ve mostly edited the **navigation section** and left the rest as is ⚠️  I'd rather have 'Home' show a short description about me instead of the default latest blog posts. These instructions reflect that preference.

1. Edit the ‘header’ section of the configuration file. ⚠️ To enter the editing mode, click the pen icon. 
2. Edit the ‘navigation’ section.  Websites typically have a navigation bar on top with buttons like ‘Home’, ‘About’, etc. The ‘navigation’ section of the config file is where we specify what visitors see when they click on buttons in the navigation bar. In this example, ‘index.md’ should contain information that I want to be displayed on my home page. ⚠️ For some website themes, the default ‘Home’ page is a list of the latest blog posts. This is because the file that ‘Home’ links to (‘index.md’ in this example) contains a lists of the latest blog posts. Since I wanted my blog posts to be under separate  ‘Blog’ section rather than show up as my home page,  I renamed ‘index.md’ to ‘blog.md’, and linked this file to the ‘Blog’ heading in the navigation bar, instead of ‘Home’.
![edit config file](/assets/photos/4_edit_config_file.png)


3. Create a file for the ‘Home’ page and name it ‘index.md’.   ⚠️ It’s important to name the file ‘index’ since GitHub Pages looks for a file with this name to build a page. Without an index file in the repository,  your page will not load.
![create new file](/assets/photos/5_create_new_file.png)


4. Edit the index.md file. ⚠️ The format specified by your extension needs to be adhered to exactly.  I am using the markdown format, indicated by ‘.md’. The ‘---‘ lines demarcate the header and are necessary for the page to render properly.
![format home page](/assets/photos/6_format_home_page.png)


# Updating the blog
1. Look through blog templates that came with the theme. 
2. Copy any blog template and edit it to make it your first post! 


# Troubleshooting 
1. After forking the repository and renaming it, the  '404: Page not found' error message shows up.

Suggestion: Some wait time is expected: I waited for thirty minutes. However, there are a few things that you could check or try: 

- Clear your cache. 
- Check also that you have named your website <username.github.io>: this is the format that GitHub recognises for building a personal website.
- Check your config file to see if the links under the ‘navigation’ section are correct: no extra spaces!  


# Resources 
- Asst Prof Kathryn Schuler’s [tutorial](https://www.youtube.com/watch?v=qZsgPgGdOzQ) 
- Free [Jekyll themes](https://jekyllthemes.io/) to choose from 
