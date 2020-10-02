---
title: "Creating an R Package"
author: "Jacob Castro"
date: "9/22/2020" 
layout: page
---
<br>  
  


# Creating an R package

"This tutorial will take you through the steps of creating a new package in R.

There are five primary tasks:

Create a package skeleton (set of empty files and folders).
Add your R code to the skeleton directory.
Create documentation for your package (similar to knitting RMD files).
Install your new package on your computer and test it out.
Upload the package to GitHub."


<br>


# Starting Your R Project

To start making your own package, youre going to want to go to the rop right where it says R project and click new.


![](/assets/img/12.png)

<br>

You're going to click new directory and then start a new project with dev tools
<br>

![](/assets/img/1.png)

<br>

Once started you can edit the description in R and complete with the information thats needed
<br>

![](/assets/img/3.png)

<br>

# How to Add Functions
<br> 

To add Functions You have to Ctrl + Shift + N. Then You will add you function and your function skeleton. To add a skeleton without copy and pasting, you can Ctrl + Alt + Shift + R.  Then you want to save it as the name of the function and it will be saved under name space. Youll see the file kb memory get bigger as you add more functions.
<br>
![](/assets/img/5.png)
<br>

To make sure the function is working properly, you want to hit check and make sure you have no errors and if you do, fix them. Then after your check is done, install and restart. You might have to do this twice to get it to work. 
<br>

![](/assets/img/6.png)

<br>

# Test It
To make sure your function is working type your package name in the console and then type out the fucntion. 

![](/assets/img/7.png)

# GitHub Hosting
You have a couple of options for sharing your new package with others. You could submit the package to the CRAN so that everyone in the world could install it in R using install.packages(“montyhall”).

We cannot use this option because (1) it’s a homework assignment so we don’t want to burden people with the task of reviewing a new package, (2) package names on the CRAN must be unique so everyone from the class would have to name it something different, and (3) the CRAN requires that the package passes some robustness checks to ensure everything is documented correctly and all of the code is running smoothly.

A simpler option is to host your package on GitHub. Complete the following steps to upload your code to a new repository on GitHub:

1. Install the git client on your computer: LINK.
2. Install GitHub Desktop application: LINK.
3. Open GitHub in a browser and navigate to your profile.
4. Create a new repository titled “montyhall”. Check the “Create with README” option.
5. Copy the URL for your new repository.
6. Open GitHub desktop and select File >> Clone Repository.
7. Select the desired location of the folder and paste the URL into the appropriate dialogue.
8. Clone your GitHub repo.
9. Open the new “montyhall” folder that was just created by GitHub on your machine.
10. Transfer all of the files inside of your old “montyhall” folder into the GitHub version.
11. You should see the files appear in the GitHub Desktop app. In the “summary” field type something like “initial commit” and at the bottom left select “Commit to master”.
12. Now up at the top select “Push origin”.

This last step sends all of the files to GitHub. They sould appear on your repo page shortly.

Now others should be able to install your package by typing:

devtools::install_github( "yourGitHubName/montyhall" )
