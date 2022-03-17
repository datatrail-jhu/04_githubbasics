There are two parts to the Git and GitHub system. 

Git is focused on version control - basically keeping track of the different versions of all the files you are working on. You can track a git repo on r studio cloud just for yourself to make sure you always have your file history available to you.

GitHub is two things, first it is a way to back up and store all of your projects on the internet.

But it is also a social network for coders. You can use GitHub to contribute to other people's projects and get feedback on your projects as well.

In an an earlier lesson we learned about issues. Issues are comments that you can make on either one of your own repos or on someone else's repos. Pull requests are a different kind of interaction that involve making a change directly to someone's code. First you would fork the repo to make your own copy. 

Then you can send the owner of the repo a "request" to "pull" your change into their code. If they accept your pull request, then their code will be updated with your suggestion! 

Pull requests are a great way to contribute to projects that are being worked on by more than one person. This may be because you are working directly with a team and you all need to edit a document. Or it may be because you see someone else's project and want to make a suggestion. This is in fact one of the best ways to start to introduce yourself to the R community on GitHub. Find a project or a repo where you see something small you can help with - even if it is just fixing a typo or adding a comments - and send them a pull request. 


Now let's talk about how to make a pull request. The first thing that you will need to do is to create a "fork" of the repository you want to edit. This is a little different than "cloning" which you learned about in an earlier lesson. When you clone a repository you are just getting a copy of the project on r studio cloud. You are not creating a new version that you can work on. 

When you fork a repo, then something different happens. First a new repo is created under your account on GitHub. You can then clone that copy to your computer. Now when you make edits to the files on r studio cloud and push them, they will be pushed to your fork. 


Let's try this out. We are going to make some changes to a repo and send a pull request. We will use https://github.com/jtleek/new project as an example project to send a pull request to. The first step is to create a fork of this repository. To do this, go to the project webpage and click on Fork in the top right hand corner of the screen. 

This may ask you where to fork the repository if you are on multiple teams. Select your main account and wait while the repository is forked.


You will see now that you have your own version of the new project repository on your GitHub profile and you will be able to see where the repository was forked from right under the repository name on the upper left. 


Now that you have a copy of this repository on your GitHub account, you can clone it to r studio cloud as we learned about in a previous lesson. You can clone it by navigating to the terminal in your r studio dot cloud account and typing the command git clone https://github.com/your_username/new project.git. 


where you replace your under score username with your GitHub username. This should create a folder on your r studio dot cloud account called new project. You may have to enter your username and password. 

Now you have successfully "forked" and "cloned" the new project repository.


The next step is to make some edits to one or more of the files. This could be as simple as fixing a typo or as complicated as adding a whole new function. For now, let's open up the file  myfile dot Rmd and make an edit. For example, we could change the line of code that reads summary cars to a line that loads the d plier package and uses the glimpse function to look at the data set. After making this edit you can save the file. Now we are ready to start the process of sending a pull request. 


Remember that when we forked the repo from j t leek's GitHub account, we got a new repo under your account. The first step in sending a pull request is to commit and push the edits to your fork, or copy, of the repo. To do this, navigate to the terminal and make sure that you are in the right folder. To do this you can use the Unix commands p w d and c d to make sure you are in the right place. When you type the command. You should hopefully see that you are in the folder for new project. If you are not, then you will need to use the c d command to make sure you are in that folder. 


To start a pull request, you need to make sure you use git add to add any new files you might have changed or deleted. This will make sure that git is now monitoring those files you might have added. 


Next you can commit your changes with a message describing what you did. Since we are going to be sending a pull request to someone else, it is a good idea to have a very clear commit message. So for example we could use the git commit command like this. git commit dash m "I edited myfile dot R m d to use glimpse to summarize the cars data". 

Now you will have saved the file on r studio dot cloud, but you still need to make the change to your fork of the repo. To do this we need to use the git push command. 

You might be asked to input your username and password for GitHub to make this push. But once it has happened you should be able to got to your forked version of the repository at https://github.com/your_username/new project/ and see the changes in the file myfile dot R m d on the GitHub website. 

Now you have successfully forked j t leek's new project repo, cloned it to r studio dot cloud and made some edits. You have added, committed, and pushed those changes to your own fork. The next step is to send a pull request to the user who created the original repo. To do this you should go to the website with your fork. Now you can click on the "Pull requests" tab for your repo. Then click on "New Pull Request". 


If there have been no changes made to the original repo from j t leek other than yours you should see that your pull request is "able to be merged" in green. You will also see a "diff" which is all of the files and changes to those files that you have made. You can then click on "Create Pull Request" to send the change to j t leek for him to review. 


You will be shown a screen where you can describe your pull request with a title and with a description of what you did. It is a good idea to put a pretty complete description of what you did - this will be the only description that j t leek can use to decide whether to merge the changes to his repo or not.


When you have finished typing your message click "Create Pull Request" to send the pull request to j t leek.


Now that you have created the pull request you can go to the original repo https://github.com/jtleek/new project and click on the pull requests tab. You will be able to find your pull request among those that are open. In this case, since this is a repo that is used as an example for a MOOC there may be many open pull requests.

The author of the original repo can then either accept your change, or they can ask you questions about your pull request just below the place where they can decide whether to merge the change.  


Once they click on "Merge pull request" your changes will automatically be incorporated into their code. Congratulations you have helped someone fix their code and made a new friend on GitHub! 


This is the easiest case of a pull request. The author of the original repo hasn't made any changes to the files that conflict with the changes that you made. In general, it is much nicer for the owner of the repo to accept your pull request if they don't have to fix any conflicts. So when you decide to make a change to someone's code, it is a good idea to make sure you make a fresh fork with all the latest changes in their code. Then clone, edit, push, and send your pull request in a timely way. This should ensure that there are no conflicts when you send the pull request to the original author. Sometimes it is more difficult than that since you may be editing a repo that is in active development or is being edited by multiple people. In this case, you will need to keep your forked version of the repo up to date with the original version. GitHub has instructions for keeping your fork up to date and Jenny Bryan's book Happy Git and GitHub for the useR also has a section on forking that may be useful when encountering these more complicated scenarios. 




