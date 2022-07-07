## The Goal...
The goal of this exercise is to get used to creating branches, merging and deleting branches, and also pushing them to the remote origin branch of the original repo. (NOTE: you should not fork this repo before you clone it down to your machine.) 

## The Reason...
The REASON for this exercise is to get used to protecting the functionality of your existing work as you go. We should start creating feature branches to work on, make sure those work properly, and then merge into main. You can then delete the feature branch (after making sure that main has successfully merged) because you no longer need it!

When you start working on teams you won't be merging drectly into main, you will be pushing your feature branch to origin and creating a pull request to have someone review your work!

There are many git cheatsheets out there. Here is [one](https://about.gitlab.com/images/press/git-cheat-sheet.pdf) and here is [another](./assets/git-essentials-cheatsheet.pdf) - pdf file can be viewed here via [this extension](https://marketplace.visualstudio.com/items?itemName=tomoki1207.pdf).

***
## Today's Exercise

I will be asking for a volunteer for each exercise to share screen and work thru this git flow.

1. First exercise: assuming that you've already cloned down this repo to your machine, create a feature branch with a meaninful branch name (usually includes your name and what your intended feature will be). Get the feature working. Can be any old thing: change the background color of the page, add a button, or an image. You may format something that is already on the page. Once this is working the way you expect, go back to the main branch, merge with your feature branch and push to origin main. Then delete the local feature branch. From there, go to Github and follow the commands to create a pull request.

2. Second exercise: assuming that you've already cloned down this repo, create a feature branch as above. But instead of merging with main, push to -u origin <feature-branch-name>. This will create a new branch at origin that tracks with your local feature branch. From there, go to Github and follow the commands to create a pull request. I will accept and merge, and then you can pull down to your main branch and delete your local feature branch.

3. Third exercise: Two people will create their own individual branches and create some small feature, then merge into main. One will push to origin main and the other will pull the updates from origin main. Assuming that you have been working in the same file, this will create a merge conflict which we will resolve and then push back to origin main.

Some handy commands: 
  'git log --oneline' - to view all commit names and numbers in a concise list

  'git checkout <commit#>' - safely allows us to go back in time to view an earlier commit without losing our work

  'git checkout master' takes us back to the HEAD of our master branch

  'git revert <commit#>' - adds a new commit that reverts (reverses) that particular commit. we'll need to use :wq to quit the vim editor that is asking us to add/change the commit message.

  'git reset <commit#>' - slightly scary option. permanently reverts to a previous commit but doesn't not remove our code from those later commits. leaves all our code intact but as uncommitted. in case we change our minds.... 
  very scary option => if we want to discard our additions, we run 'git reset <commit#> --hard'