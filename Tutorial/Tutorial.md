---
title: "Tutorial"
author: "Wendy Leuenberger"
date: "2024-03-25"
output: 
  html_document:
    keep_md: true
---

# Tutorial with the repository

This tutorial is designed for step-by-step editing of a GitHub repository and for learning how to submit jobs to the HPCC. The repository is meant to pick up at the end of HPCC.Rmd/md/html, once you have your computer configured to allow GitHub and RStudio to talk to each other and have the HPCC account mapped to your drive. You can also work through the exercises without the HPCC. 

## Put this repository on your computer

Fork the repository: Only owners of a repository can make changes. But if the repository is public, others can "fork" the repository. This creates a local copy on their GitHub that they can make changes to. Go to the main page of this repository. Above the green `<> Code` button, there are four buttons. The third says `Fork`. Click this button and make a copy of this repository in your account. 

## Clone the repository to your computer

Create a new RStudio project with Version Control and use your forked repository's url to link the project to your repository. You can find the url by clicking the green  `<> Code` button. (See the HPCC.* for more detail). Leave this project open. 

## Learn how to make edits

There are multiple ways to make edits to a GitHub repository. Try out these three ways:

1. Commit using the web browser. 

    - In your web browser, navigate to the main page of the repository. Your README file should be showing.
    
    - Above the header, you can see README on the left and a pencil and outline buttons on the right. Click on the pencil to edit. Alternatively, you can click the file name and then the edit button on the right. 

    - Replace my name with your name.

    - Click the green `Commit changes...` button on the upper right.
  
    - Add a commit message that is useful - i.e. "Added my name"

    - Leave the toggle on `Commit directly to the main branch`

    - Click the green `Commit changes` button. 

    - Your name will now appear on the main README page!
    
    - Go to your RStudio window that is linked to your GitHub repository. Go to the Terminal window (usually the tab next to the Console in the lower left window). You'll see the file path to your repository. Type `git pull` to pull the change you just made to the README.md in the browser. 

2. In RStudio, using the Git tab. 

    - Open the README.md document. You can find it under Files in the lower right window. 

    - Underneath your name, replace `Today's Date` with the Date. 
    
    - Save the file. 
    
    - In the upper right window, go to the Git tab. Check the box under the `Staged` column for the README.md. 
    
    - Click the `Commit` button above the files.
    
    - Type a commit message like `Added today's date` in the window on the upper right. 
    
    - Click `Commit`
    
    - On the upper right, click the `Push` button.
    
    - Close the Git window and go to the repository in your web browser. Refresh and the date that you added will show up. 
    
3. In RStudio, using command line. 

    - Go back to your README.md in RStudio. 
    
    - Underneath the Date, note the Favorite Animal line. Replace Favorite Animal with your favorite animal or something else fun. 
    
    - Go to the Terminal tab next to the console. (On windows, you can use Ctrl + Alt + M to navigate to the terminal)
    
    - Type `git pull` (you haven't done anything that needs to be pulled, but it's a good practice to pull before pushing in case of changes)
    
    - Type `git add README.md`
    
    - Type `git commit -m 'Added favorite animal'`
    
    - Type `git push`
    
    - Typing `git status` is also helping for seeing what files have been changed and if you're ahead of or behind the uploaded Git repository. 
    
All of these methods work! The rest of the tutorial will be in command line, but most could be done with any method. Command line is particularly useful with the HPCC, as you can have multiple terminal windows for your computer, the HPCC, and the mapped drive, all within one RStudio window.