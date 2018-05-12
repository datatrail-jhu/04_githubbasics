# Setting up A Project on Github

Now that we've learned the basics of organizing data science projects and Github, in this lesson we'll walk through setting up an example project and pushing the content to Github.

### Setting up a Github repository

First things first, we need to create a repository. Go to [Github](www.github.com), login to your account, and create a repository just like we learned before.

![Create a new repository](images/06_git_projects/06_githubbasics_git_projects-01.png)

You can also create a new repository by clicking on the plus sign in the top right corner of Github homepage and clicking on New repository.

![Second way of creating a new repository](images/06_git_projects/06_githubbasics_git_projects-02.png)

On the page that follows, type the repository name. Choose the name `my_first_project`, add a description if you wish (always recommended), make it public, and choose to initialize with a README file. At the end click on the buttion Create repository.

![Add repository information](images/06_git_projects/06_githubbasics_git_projects-03.png)


The next step is to clone this repository into RStudio Cloud but as you may remember, we first need the url to this repository we just created. On the repository page, click on Clone or download and copy the link address. Make sure the address starts with `https` rather than `git`. If it starts with `git`, click on Use HTTPS on the corner of the small window to have the link starting with `https`. 

![Repository link](images/06_git_projects/06_githubbasics_git_projects-04.png)

### Creating a new project from a Github repository

Ok, now that we have everything set up on the Github end, Go to [RStudio Cloud](https://rstudio.cloud/) and login with your account. When you're redirected to yoru Projects page, Next to the New Project button, click on the drop down button and then click on New Project from Git Repo. 

![Create new project from Git repo on RStudio Cloud](images/06_git_projects/06_githubbasics_git_projects-05.png)

On the popup window, paste the repository url that you just copied and click Ok. 

![Enter repository url](images/06_git_projects/06_githubbasics_git_projects-06.png)


This will automatically clone the remote repository and create a new project on RStudio Cloud. Note that the repository is still unnamed so you may want to change the name to something else. If you click on the README file under Files, you will see that the README file contains the description you added on the Github website.


![All the files in the remote repository are cloned in RStudio Cloud](images/06_git_projects/06_githubbasics_git_projects-07.png)

Start editing the README file. Specifically, replace the content with the following lines.

```text
# This is the README file for my_first_project
The folders in this project are: 

* _data_ - is the folder where you will put all the data you have collected or been given to analyze. 
* _figures_ - is where you will put plots, data pictures, and other images you have created to show data to other people. 
* _code_ - is where you will create code files for collecting, cleaning up, or analyzing data. 
* _products_ - this is the place where you will place any reports, presentations, or products you create for sharing with other people.
```

### Pushing local changes to the remote repository in RStudio Cloud

Now, it's time to push the changes we made to the remote repository. As we've seen we should follow the steps here. Type the following commands in the terminal one by one. Previously, we used the `git add` command with specific file names. However here we're using `git add .` which means we are tracking changes in all files in the project.

```text
git add .
git commit -m "changed readme file"
git push
```

Once you enter `git push`, you will see a prompt asking you for your repository user name and then password. Enter those correctly and voila, you will see something similar to this which means that all the changes are pushed to the remote repository.

```text
Counting objects: 3, done.
Delta compression using up to 16 threads.
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 338 bytes | 0 bytes/s, done.
Total 3 (delta 1), reused 0 (delta 0)
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To https://github.com/JaneEverydayDoe/my_first_project.git
   e80844c..24fec16  master -> master
```

You should be able to see your changes on the repository on Github.com. 

![Changes can be seen on the remote repository](images/06_git_projects/06_githubbasics_git_projects-11.png)

We have learned about the importance of organization and folder structure in data science projects. Let's practice creating the main folders required in a data science project. As you may remember, these folders represent the four parts of any data science project: data, figures, code, and products. Let's create them on RStudio Cloud.

![Data science project folders](images/06_git_projects/06_githubbasics_git_projects-21.png)

Now go ahead and further create the folder structure that we learned. An important note is that if you push the changed you created in the project to Github, you won't see the folder structure that you created. Unfortunately, a folder structure won't be pushed to Github unless the folders contain at least a file. So don't worry. Once you populate this project with your data, code, figures, and writings and push them to Github you will see the folders your just created.

* data/
  * raw_data/
  * tidy_data/
* code/
  * raw_code/
  * final_code/
* figures/
  * exploratory_figures/
  * explanatory_figures/
* products/
  * writing/
  
  


### Slides and Video

![Setting up projects on Github]()

* [Slides](https://docs.google.com/presentation/d/1pmSkcf0iSQysOAMuuMK-CihaiSbtqDhg0ME2R9zqRDA/edit?usp=sharing)

### Issues on Github Quiz

{quiz, id: quiz06_git_projects}

# Setting up a project on Github quiz

? 

{/quiz}

