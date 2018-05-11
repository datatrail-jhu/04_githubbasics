# Creating a repository and setting up your GitHub profile

Now that you have learned about version control and the GitHub website, we will do some actual work with the GitHub website to create a new repository and set up your user profile.

### What is a repository?

First let's review what a repository is. A repository houses the entirety of a project. Imagine a filing cabinet. A repository for this project would be the filing cabinet itself. Inside the cabinet are various folders and files that make up the project. As you begin working on various projects, each one will likely have its own repository, and any work that you do will be housed in that repository. In the first part of this lesson, we will discuss how to create a repository using the GitHub website.

### How do I create a Github repository?

#### Step 1

First, navigate to the GitHub website: [GitHub.com](https://github.com/). Click the green button on the right hand side of the page that allows you create a new repository.

![Creating a new repository](images/02_creating_repos/02_githubbasics_creating_repos-2.png)

#### Step 2

You will be taken to a new page where you can set up information about this new repository. Most importantly, create a descriptive name for the repository that relates to your project. This will help you remember what repository holds your files for this project if you have many repositories or come back to the project at a later time.

Including a description for your repository is optional.

You have a choice to make your repository public or private. Public repositories are viewable by the public. Anyone can see what code you have used for this project. You can still control who can contribute to this particular repository, but the repository is open to being forked by other people who may want to build off of your work in their own repositories. Private repositories are not viewable by the public, and you can still control who can contribute to this particular repository. It is generally a nice choice to make a repository public to share your work with others, but if you are working with sensitive information, it would be best to make the repository private. Keep in mind that you can have private repositories on Github only if you are a paid subscriber. 

You can leave the other options at their default settings.

When you are satisfied with these settings, click the "Create repository" button at the bottom.

![Setting up a new repository](images/02_creating_repos/02_githubbasics_creating_repos-3.png)

And you're done! You will be taken to a page that looks as below. This page contains information about the commands that will be useful when adding files to your repository later on. We will cover the use of these commands from RStudio Cloud in subsequent lessons.

![Landing page](images/02_creating_repos/02_githubbasics_creating_repos-4.png)

### Adding a README file

If you click on the link labeled README indicated in the picture below, you can add a README file to your currently empty repository. The README file is the first thing someone sees when they navigate to the page for your repository. It is useful for providing an overview for what is contained within it.

![Creating a README](images/02_creating_repos/02_githubbasics_creating_repos-5.png)

When you click on that link, you will be taken to a page pictured below where you can edit the text of this file and preview what it will look like on the GitHub website. It has been automatically filled in with the title of our repository and the optional description we entered previously. Feel free to add additional description. The README file is a markdown document so you will have to use markdown syntax for editing this document.

![Editing a README](images/02_creating_repos/02_githubbasics_creating_repos-6.png)

When you are finished editing your README file, scroll to the bottom of the page to commit your changes. As in the picture below, add a short description to the first box to describe what you've done. Usually this alone will suffice so that you don't need to add additional description in the box beneath.

![Committing changes](images/02_creating_repos/02_githubbasics_creating_repos-7.png)

Click the "Commit new file button" to add this README to your repository. You will be taken to the homepage for your repository, as pictured below.

![Repository homepage](images/02_creating_repos/02_githubbasics_creating_repos-8.png)

Congratulations! You have created and set up your first repository!


### Setting up your GitHub user profile

Now that you have some public GitHub activity, let's take a brief detour to optimize your GitHub experience in terms of interacting with other users and customizing your workflow.

You can navigate to your public profile from anywhere on the GitHub website by clicking the drop down menu in the top right hand corner and clicking "Your profile."

![Navigating to your public GitHub profile](images/02_creating_repos/02_githubbasics_creating_repos-10.png)

You will be taken to your public profile. The Overview tab provides a summary of your work on GitHub. You can showcase up to 6 of your repositories by clicking the link labeled "Customize your pinned repositories." When you are logged into GitHub, the Repositories tab lists all public and private repositories you have. If your are not logged in, it will only show your public repositories. The Stars tab shows repositories you have starred, similar to boomarking a web page in your browser. If you find the contents of a repository interesting, you can go to the main repository page and click the Star button near the top right. The Followers and Following tabs shows users that you follow and who follow you for activity updates. Following others is is a nice way to explore other people's work.

![Your profile page on Github](images/02_creating_repos/02_githubbasics_creating_repos-11.png)


If you would like to change any of your profile information, click on the drop down menu in the top right hand corner and click on "Settings."

![Navigating to your profile settings](images/02_creating_repos/02_githubbasics_creating_repos-12.png)


The panel on the left let's you customize your work experience and notifications in a variety of ways. You will by default be taken to a tab where you can edit what appears on your public profile.

![Profile settings on Github](images/02_creating_repos/02_githubbasics_creating_repos-13.png)


The Account tab lets you change your username or password. The Emails tab lets you modify what e-mail address(es) to use for notifications and has some privacy settings relating to where your e-mail addresses can appear publicly. The Notifications tab allows you to fine tune what GitHub updates send notifications and where they are sent.


### Slides and Video

![Creating A Repository]()

* [Slides](https://docs.google.com/presentation/d/1Dxf8VZi4RAf4BA8Xb__gbnTxFLIJKM-mxSy_BMA48DU/edit?usp=sharing)


{quiz, id: quiz02_creating_repos}

# Creating Repositories quiz

? In which of the following instances would you create a public repository?

A) To share your work with others
b) To comply with employer specifications about project security
c) To use version control on the analysis of sensitive data


{/quiz}

