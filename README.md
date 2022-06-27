## The Goal...
The goal of this exercise is to get used to creating branches, merging and deleting branches, and also pushing them to the remote origin branch of the original repo. (NOTE: you should not fork this repo before you clone it down to your machine.) 

## The Reason...
The REASON for this exercise is to get used to protecting the functionality of your existing work as you go. We should start creating feature branches to work on, make sure those work properly, and then merge into main. You can then delete the feature branch (after making sure that main has successfully merged) because you no longer need it!

When you start working on teams you won't be merging drectly into main, you will be pushing your feature branch to origin and creating a pull request to have someone review your work!

There are many git cheatsheets out there. Here is [one](https://about.gitlab.com/images/press/git-cheat-sheet.pdf).

***
## Today's Exercise

I will be asking for a volunteer for each exercise to share screen and work thru this git flow.

1. First exercise: assuming that you've already cloned down this repo to your machine, create a feature branch with a meaninful branch name (usually includes your name and what your intended feature will be). Get the feature working. Can be any old thing: change the background color of the page, add a button, or an image. You may format something that is already on the page. Once this is working the way you expect, go back to the main branch, merge with your feature branch and push to origin main. Then delete the local feature branch. From there, go to Github and follow the commands to create a pull request.

2. Second exercise: assuming that you've already cloned down this repo, create a feature branch as above. But instead of merging with main, push to -u origin <feature-branch-name>. This will create a new branch at origin that tracks with your local feature branch. From there, go to Github and follow the commands to create a pull request. I will accept and merge, and then you can pull down to your main branch and delete your local feature branch.

3. Third exercise: Two people will create their own individual branches and create some small feature, then merge into main. One will push to origin main and the other will pull the updates from origin main. Assuming that you have been working in the same file, this will create a merge conflict which we will resolve and then push back to origin main.