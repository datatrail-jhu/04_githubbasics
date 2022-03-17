Now that we've learned the basics of organizing data science projects and GitHub, in this lesson we'll walk through setting up an example project and pushing the content to GitHub.

First things first, we need to create a repository. We'll do this as discussed in the "Creating A Repository Lesson," by going to www.github.com, logging in to your account, and creating a new repository

You can also create a new repository by clicking on the plus sign in the top right corner of GitHub homepage and clicking on New repository.

On the page that follows, type the repository name. Choose the name my first project, add a description if you wish (always recommended), make it public, and choose to initialize with a README file. At the end click on the button Create repository.

The next step is to clone this repository into RStudio Cloud but as you may remember, we first need the url to this repository we just created. On the repository page, click on Clone or download and copy the link address. Make sure the address starts with https rather than git. If it starts with git, click on Use H T T P S on the corner of the small window to have the link starting with https. 

Ok, now that we have everything set up on the GitHub end, Go to R Studio dot Cloud and login with your account. When you're redirected to your Projects page, Next to the New Project button, click on the drop down button and then click on New Project from Git Repo. 

On the popup window, paste the repository url that you just copied and click Ok. 

This will automatically clone the remote repository and create a new project on RStudio Cloud. Note that the repository is still unnamed so you may want to change the name to something else. If you click on the READ ME file under Files, you will see that the README file contains the description you added on the GitHub website.

Start editing the README file. Specifically, replace the content with these lines.

Now, it's time to push the changes we made to the remote repository. As we've seen we should follow the steps here. Type the following commands in the terminal one by one. Previously, we used the git add command with specific file names. However here we're using git add dot which means we are tracking changes in all files in the project.

Once you enter git push, you will see a prompt asking you for your repository user name and then password. Enter those correctly and voila, you will see something similar to this which means that all the changes are pushed to the remote repository.

You should be able to see your changes on the repository on Git hub dot com. 

We have learned about the importance of organization and folder structure in data science projects. Let's practice creating the main folders required in a data science project. As you may remember, these folders represent the four parts of any data science project: data, figures, code, and products. Let's create them on RStudio Cloud.

Now go ahead and further create the folder structure that we learned. An important note is that if you push the changed you created in the project to GitHub, you won't see the folder structure that you created. Unfortunately, a folder structure won't be pushed to GitHub unless the folders contain at least a file. So don't worry. Once you populate this project with your data, code, figures, and writings and push them to GitHub you will see the folders your just created.