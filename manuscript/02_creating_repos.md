# Creating A Repository

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

When you click on that link, you will be taken to a page pictured below where you can edit the text of this file and preview what it will look like on the GitHub website. It has been automatically filled in with the title of our repository and the optional description we entered previously. Feel free to add additional description. The README file is a markdown document so you will have to use the markdown syntax you learned in the last course to edit this document.

![Editing a README](images/02_creating_repos/02_githubbasics_creating_repos-6.png)

When you are finished editing your README file, scroll to the bottom of the page to commit your changes. Here, GitHub automatically suggests that "Create README" is your commit messages. As this is informative of what you have done, you do not need to add additional text; however, you're welcome to make this commit message even more informative if you'd like.

![Committing changes](images/02_creating_repos/02_githubbasics_creating_repos-7.png)

Click the "Commit new file button" to add this README to your repository. You will be taken to the homepage for your repository, as pictured below.

![Repository homepage](images/02_creating_repos/02_githubbasics_creating_repos-8.png)

Congratulations! You have created and set up your first repository!

### The GitHub guide 

GitHub also recognizes that this can be an overwhelming process for new users, and as such have developed a mini tutorial to get you started with GitHub. You can go through [this guide](https://guides.github.com/activities/hello-world/) to get further process setting up repositories on GitHub!



### Slides and Video

![Creating A Repository](https://www.youtube.com/watch?v=tUnp7nZSS5E)

* [Slides](https://docs.google.com/presentation/d/1Dxf8VZi4RAf4BA8Xb__gbnTxFLIJKM-mxSy_BMA48DU/edit?usp=sharing)


{quiz, id: quiz_02_creating_repos}

# Creating A Repository quiz

{choose-answers: 4}
? In which of the following instances would you create a public repository?

C) To share your work with others
o) To comply with employer specifications about project security
o) To use version control on the analysis of sensitive data
o) To use version control on the analysis of private data
o) To use Git but ensure that you are the only person with access to the code.

{choose-answers: 4}
? Fill in the blank: I will have a GitHub repository for each ________.

C) project
o) part of my project
o) script
o) different directory
o) GitHub
o) version control

{points: 2}
? To make a new repository, which can you **not** do? (Note: To figure out the answer to this question, you may have to play around on GitHub a bit.)

A) Profile > New repository  
b) Plus sign > New repository  
c) Profile > Repositories > New  

{/quiz}

