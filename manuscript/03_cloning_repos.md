# Cloning a repository

Now that you have learned how to create a GitHub repository, you will learn how to obtain a copy of that repository in a location that you use for writing code. That is, we will cover how to **clone** an existing repository in RStudio Cloud.

### Step 1: Navigate to the Terminal in RStudio

Within a project in RStudio Cloud, navigate to the Terminal tab, indicated in the picture here. This is where you can type Git commands to work with repositories. The text that you see at the beginning of the line in the Terminal is called the **prompt**. When you see the prompt at the beginning of a line, this indicates that the Terminal is ready to accept your commands.

![Navigating to the Terminal](images/03_cloning_repos/03_githubbasics_cloning_repos-1.png)


### Step 2: Obtain the URL for the repository to clone

Navigate to the GitHub webpage for your repository. This URL always has the form

```text
https://github.com/github_username/repository_name
```

For example, in our last lesson, the URL for our repository is [https://github.com/JaneEverydayDoe/first_project/](https://github.com/JaneEverydayDoe/first_project/). On this page, you will see a button on the right hand side that says "Clone or download". When you click this, highlight the URL in the box, and copy it to the clipboard. Make sure it starts with "https" rather than "git@". If you see "git@", click the link in the top right corner of the box that says "Use HTTPS".

![Obtaining the clone URL](images/03_cloning_repos/03_githubbasics_cloning_repos-2.png)

### Step 3: Use the clone command in the RStudio Terminal

Navigate back to the Terminal tab in RStudio that you opened in Step 1. Type the command:

```text
git clone repository_url
```

Replace `repository_url` with the URL that you copied in Step 2, and hit Enter. You will see some status text appear as the repository is being cloned to a location on RStudio Cloud. When this is complete, typically after a few seconds, the Terminal prompt will appear again on a new line, indicating that you are able to input new commands if you wish.

Also note that in the bottom right hand corner of RStudio, in the Files pane, you will have a new folder that has the same name as your Git repository.

![Using the git clone command](images/03_cloning_repos/03_githubbasics_cloning_repos-3.png)

### Aside: directory/folder organization

A big part of staying organized with your files is understanding how folders in your project are organized. Also important is the concept of a **working directory**. Whenever you are working in R or the Terminal, you are housed in some folder. This folder is called the working directory. Knowing this is important so that you know how to specify paths to other important folders in your project. We can see what the current working directory is in a number of ways. In the image below, we can see from the Terminal prompt that the working directory is `/cloud/project`. We can also see this in the Files pane. We see that the first level folder is `cloud` and that the second level folder is `project`.

![Working directories](images/03_cloning_repos/03_githubbasics_cloning_repos-4.png)

Congratulations! You have cloned your first repository!


### Slides and Video

* [Slides](https://docs.google.com/presentation/d/1bhTNTBhdXa0e0BXRZmQoHY6zTKGqgrr4wwYS8-v7ob8/edit?usp=sharing)


{quiz, id: quiz03_cloning_repos}

# Cloning repositories quiz

? What is *cloning* in Github terminology?

a) Sending committed changed to a repository
B) Creating a local copy of a repository on your computer
c) Taking the changes in one branch and applying to another
d) Getting the latest changes from an online repository

? How do you use the `clone` command in terminal in order to clone a repository?
a) `clone repository_url`
b) `git repository_url`
c) `clone git repository_url`
D) `git clone repository_url`

{/quiz}









