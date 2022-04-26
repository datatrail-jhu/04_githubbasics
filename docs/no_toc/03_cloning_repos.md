---
title: "cloning_repos"
output: html_document
---



# Cloning A Repository

Now that you have learned how to create a GitHub repository, you will learn how to obtain a copy of that repository in a location that you use for writing code such as RStudio Cloud. This process is called "cloning" a repository from GitHub.

### Step 1: Obtain the URL for the repository to clone

Navigate to the GitHub webpage for your repository. This URL always has the form

```text
https://github.com/github_username/repository_name
```

For example, in our last lesson, the URL for our repository is [https://github.com/JaneEverydayDoe/first_project/](https://github.com/JaneEverydayDoe/first_project/). On this page, you will see a button on the right hand side that says "Clone or download". When you click this, highlight the URL in the box, and copy it to the clipboard. Make sure it starts with "https" rather than "git@". If you see "git@", click the link in the top right corner of the box that says "Use HTTPS".

{format: png}
![Obtaining the clone URL](https://docs.google.com/presentation/d/1bhTNTBhdXa0e0BXRZmQoHY6zTKGqgrr4wwYS8-v7ob8/export/png?id=1bhTNTBhdXa0e0BXRZmQoHY6zTKGqgrr4wwYS8-v7ob8&pageid=g36809c5e39_0_0)

### Step 2: Use the RStudio interface to clone the repository

In RStudio cloud, go to your workspace by clicking the appropriate button on the left side navigation bar.

Click the `New Project` button and choose `New Project from Git Repository`


AVOCADO: Slides here.

Place the URL that you copied in Step 1 in the `URL of your Git Repository` box, and click `OK`.
You will a `Deploying Project` progress screen, typically after a few seconds, the RStudio interface for your project will appear.

Also note that in the bottom right hand corner of RStudio, in the `Files` pane, you will have the files that are in your GitHub repository, now available in this RStudio cloud workspace.

### Step 3: Set up GitHub Credentials

In order to be able to access everything in your GitHub repository from RStudio cloud, you will need to set up GitHub credentials. You should only need to do this once per project.

1. In your RStudio interface, make sure that you are in the `Console` tab.

2. Now use the command below to install the package `usethis`. This package will help us manage our GitHub credentials from RStudio more easily.

```r
install.packages("usethis")
```
This will take a minute or so to install.

3. Now to use this package, we need to attach its library using the following command:

```r
library("usethis")
```

4. RStudio and GitHub require you make a special fancy password to use as credentials called a **GitHub Personal Access Token** (sometimes abbreviated as a "PAT").

To create a 'PAT' from RStudio we can run this handy command:

```r
usethis::create_github_token()
```
Running this command will open up a window in your GitHub that will ask you for your password. Login to GitHub as you normally would.

This will open up a page in GitHub for creating a `New personal access token`.

Underneath the `Note` put something that reminds you what this PAT is for. Something like `RStudioCloud Access`. (Note that each PAT you make needs its own unique `Note` though).

Underneath the `Select scopes` section **you don't need to do anything**, `usethis` package already chose the permissions we need.

Click `Generate Token`. You've created your first PAT! **Do not close this window**, keep it handy for now.

5. Return back to your RStudio Cloud project while keeping your PAT handy.
In the `Console` window, run this command:

```r
gitcreds::gitcreds_set()
```

It will ask you to `? Enter password or token`. Copy your PAT and paste it into the command window and press Enter.

After you've entered your PAT in RStudio here, you are now free to close that GitHub PAT window. Note that you will want to be very careful with your PAT. **Do not share it or put it anywhere that others could see it or access it!**

7. Now we also need to add your username and email to the RStudio GitHub credentials by running a command like below.
But replace the example username and email with what corresponds to your GitHub account.

```r
use_git_config(user.name = "Jane", user.email = "jane@example.org")
```

Run this in the `Console` tab as well and click Enter.

8. Now to double check that everything is set, we can run this command to have the `usethis` package echo back our credentials:

```r
git_sitrep()
```

You should see that `Name`, `email` have your credentials set as well as a `Personal access token for 'https://github.com': '<discovered>'`

Yay! Now you should be able to use GitHub from RStudioCloud!

### Directory/Folder Organization

A big part of staying organized with your files is understanding how folders in your project are organized. Also important is the concept of a **working directory**. Whenever you are working in R or the Terminal, files are housed in some folder. This folder is called the working directory. Knowing this is important so that you know how to specify paths to other important folders in your project. We can see what the current working directory is in a number of ways. In the image below, we can see from the Terminal prompt that the working directory is `/cloud/project`. We can also see this in the Files pane. We see that the first level folder is `cloud` and that the second level folder is `project`.

{format: png}
![Working directories](https://docs.google.com/presentation/d/1bhTNTBhdXa0e0BXRZmQoHY6zTKGqgrr4wwYS8-v7ob8/export/png?id=1bhTNTBhdXa0e0BXRZmQoHY6zTKGqgrr4wwYS8-v7ob8&pageid=g36809c5e39_0_38)

Congratulations! You have cloned your first repository!

### Slides and Video

![Cloning A Repository](https://www.youtube.com/watch?v=RrajGWw_3wM)

* [Slides](https://docs.google.com/presentation/d/1bhTNTBhdXa0e0BXRZmQoHY6zTKGqgrr4wwYS8-v7ob8/edit?usp=sharing)


{quiz, id: quiz_03_cloning_repos}

### Cloning A Repository quiz

{choose-answers: 4}
? What is *cloning* in GitHub terminology?

C) Creating a local copy of a repository on your computer
C) Creating a copy of a repository from GitHub locally on your computer
o) Taking the changes in one branch and applying to another
o) Getting the latest changes from an online repository
o) Sending committed changed to a repository
o) Adding a message to briefly explain what changes have been made
o) Figuring out what disagreements exist between two files

{choose-answers: 4}
? How do you use the `clone` command in terminal in order to clone a repository?

C) `git clone repository_url`
o) `clone repository_url`
o) `git repository_url`
o) `clone git repository_url`
o) `git commit repository_url`
o) `commit git repository_url`
o) `git merge repository_url`

{/quiz}
