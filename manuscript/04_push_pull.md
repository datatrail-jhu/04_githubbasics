# Pushing and pulling changes

Now that you have learned how to create a repository and clone it, it's time to start using repositories to manage projects and work with collaborators. In this lesson you will learn about new git commands for publishing changes so that others can see them. You will also learn a git command for incorporating changes made by others in your local copy of a repository.

### Pushing

Over the course of working on a project, you will be creating a number of files containing code, results, documentation, or other information. How do you add these files to the Git version control system and make this information available to the public? In the first part of this lesson, you will learn about three git commands that allow you to do this: add, commit, and push.

#### Create a file

Let's start by creating a file within the project. Below we've created a text file containing a list of tasks. This is saved as tasks.txt within the `first_project` folder. This is the repository that we cloned in the previous lesson.

![Creating a file in our project repository](images/04_push_pull/04_githubbasics_push_pull-2.png)

#### Adding and committing

Now that we have added a file to this repository, let's put it under version control and publish these changes. First we need to move to the Terminal pane. Recall that the text at the beginning of the line is called the **prompt**. The Terminal prompt shows the current working directory within the Terminal. Initially, the working directory is the `/cloud/project` folder. We can see the same information by entering the `pwd` command. We can use the `ls` command to list the files and folders that are in the current working directory. We see that the `first_project` folder is the only thing present. Before working with the Git commands that will track and publish our changes, we need to change the working directory in the Terminal to be the `first_project` folder. We can do this with the `cd` command. Using the command `cd PATH` changes the working directory to the folder specified by `PATH`. For example, if the `first_project` folder contained a folder called `analysis`, we could set our Terminal working directory to this folder with `cd first_project/analysis`. 

![Changing the working directory in the Terminal](images/04_push_pull/04_githubbasics_push_pull-3.png)

We will first use the `git add` command to tell Git that the `tasks.txt` file is to be tracked for version control. The syntax for the `add` command is

```text
git add file_or_folder1 file_or_folder2
```

Any number of files and/or folders can be specified in this way. To add the `tasks.txt` file, we use

```text
git add tasks.txt
```

Now that we have let Git know that this file should be tracked for version control, we will actually record those changes with `git commit`. The `commit` command takes the files that we added with `add` and updates the Git version history record with these changes. When we use the `commit` command we also supply a descriptive message about the changes that were made by specifying the `-m` option followed by the message in quotes.

```text
git commit -m "Add task list"
```

![Adding a file and committing changes](images/04_push_pull/04_githubbasics_push_pull-4.png)

#### Publishing changes (pushing)

We are finally ready to publish our changes to a **remote repository**. We've been doing work in a local copy of the repository on RStudio Cloud. This personal copy is called a **local repository**. To make changes available to others, there needs to be an external version of the repository accessible by others. This is called a **remote repository**. Our remote repository is the one available on GitHub. To publish our changes, we use the `git push` command. Because we cloned this repository from GitHub, Git automatically knows that this is the remote repository. A local repository can have multiple remotes, and it is possible to push changes to a specified remote. We will not cover this here though. After you run `git push`, you will see some status text and you will be prompted for your GitHub username and password. After you enter these, the push will be complete.

![Pushing changes](images/04_push_pull/04_githubbasics_push_pull-5.png)

### Pulling

While working on a project, we may have a collaborator working on files in the same repository. If they create and edit files in their own local repositories and push changes to our shared remote repository on GitHub, we will want to incorporate their changes into our files. We can do this with `git pull`.

For example, a collaborator might have added an additional task to the `tasks.txt` file.

![Seeing on GitHub that a file has been edited](images/04_push_pull/04_githubbasics_push_pull-7.png)

When we run the `git pull` command, the changes present in the remote repository are incorporated into our local repository. So when we open the `tasks.txt` file, we will see the additional task.

![Pulling changes from the remote to our local repository](images/04_push_pull/04_githubbasics_push_pull-8.png)

### Slides and Video

![Pushing and Pulling Chnages]()

* [Slides](https://docs.google.com/presentation/d/1syZGx4saIzmiWVGZzIjqBjQaGkFXyC_Hlo5Pq-edYs8/edit?usp=sharing)

### Pushing and Pulling Changes Quiz

{quiz, id: quiz04_push_pull}

# Pushing and pulling quiz

? What git commands are involved in making local changes available in a remote repository?

a) clone
B) add
C) commit
D) push
e) pull

? What git commands are involved in creating a local copy of a remote repository for the first time?

A) clone
b) add
c) commit
d) push
e) pull

? What git commands would be used to mark that updates to the files `codebook.md` and `tidy.csv` should be tracked? (Multiple separate commands are separated by semicolons.)

a) git commit codebook.md tidy.csv
b) git commit codebook.md; git commit tidy.csv
C) git add codebook.md tidy.csv
D) git add codebook.md; git add tidy.csv

{/quiz}

