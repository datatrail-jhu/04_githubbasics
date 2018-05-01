{
course-completeness: 90
course-attempts: 2
default-quiz-attempts: 2
authors: Jeffrey Leek
contributors: Sarah McClymont, Leslie Myint, and Sarah Wang
}

# Version Control

In this lesson, we'll give you a basic understanding of version control. We'll look at what version control is, some of its benefits, and give an introduction to Git and GitHub, the main way you will interface with version control systems in these courses.  

### What is version control?

One common mantra from data analysis and writing code is "save early, save often". What is meant by this is that you do not want to create content without saving it frequently. This way, if you lose your internet connection, or your computer crashes, you will not lose the hard work you have put in. On the other hand, sometimes we create some content, only to realize that it is not what we want, and we want to undo the changes we have just made. Version control allows us to save frequently, while also taking snapshots of our work at any point in time, allowing us to go back to a previous version if necessary. A good version control system will do this without you having to save multiple copies of your work (myFile_version1, myFile_version2, etc.) or keep track of what the latest version of the file is.

If you've ever used the "Track changes" feature in Microsoft Word, you have seen a rudimentary type of version control, in which the changes to a file are tracked, and you can either chose to keep those edits or revert to the original format. Version control systems, like [Git](https://git-scm.com/), are like a more sophisticated "Track changes" - in that they are far more powerful and are capable of meticulously tracking successive changes on many files, with potentially many people working simultaneously on the same groups of files. 

If you've ever worked collaboratively on a document before, [this comic](http://phdcomics.com/comics/archive.php?comicid=1531) from PHD Comics might resonate with you. Hopefully, once you've mastered version control software, Paper_Final_FINAL2_actually_FINAL.docx will be a thing of the past for you! 

### Version control on your own

As mentioned above, even if you are the only one working on a project, saving frequently and preserving snapshots of your work at a specific time prevents you from losing work or making changes that cause the work you have already done to not work anymore. Or, you might be keeping multiple, very similar, copies of a file. And this could be dangerous - you might start editing the wrong version, not recognizing that the document labelled "FINAL" has been further edited to "FINAL2" - and now all your new changes have been applied to the wrong file! Version control systems help to solve this problem by keeping a single, updated version of each file, with a record of *all* previous versions AND a record of exactly what changed between the versions.

### Version control for collaboration or sharing

One advantage of using version control for your projects is that multiple users can work on different parts of the same project at the same time. Each individual can edit different files that make up a project simultaneously, and all the results can be saved in the same place. Two (or more) individuals can even work on editing the same file simultaneously, and a good version control system will allow them to then resolve any differences between the two file versions that result. 

Additionally, since version control systems keep a record of all changes made to the files, this can be of great help when you are collaborating with many people on the same files - the version control software keeps track of who, when, and why those specific changes were made. It's like "Track changes" to the extreme! 

### Summarizing the benefits of version control systems

1. It gives you an easy way of saving a backup of your work as you go, making sure you don't lose anything you have created  
2. It allows you to go back to an earlier version of your work if something gets broken due to the changes you have made  
3. It allows multiple people to edit code at the same time, without worrying that what they’re doing might be messing someone else’s code up  

### What is Git? Why should you use it?

In this course, we will introduce version control software called Git. Git is a free and open source version control system. It was developed in 2005 and has since become *the* most commonly used version control system around!  StackOverflow surveyed over 60,000 respondents on which version control system they use, and as you can tell from the chart below, [Git is by far the winner](https://insights.stackoverflow.com/survey/2017#work-version-control).

![Git is far and away the most commonly used version control system according to StackOverflow](images/00_version_control/00_githubbasics_version_control-5.png)

As you become more familiar with Git and how it works and interfaces with your projects, you’ll begin to see why it has risen to the height of popularity. One of the main benefits of Git is that it keeps a local copy of your work and revisions, which you can then edit offline, and then once you return to internet service, you can sync your copy of the work, with all of your new edits and tracked changes to the main repository online. And since Git is automatically taking these snapshots, there is  no need for you to save your own copy with different versions or different dates. Additionally, since all collaborators on a project have their own local copy of the code, everybody can simultaneously work on their own parts of the code, without disturbing that common repository. 

Another big benefit that we’ll definitely be taking advantage of is the ease with which RStudio and Git interface with each other. 

### What is GitHub?

GitHub is a website that provides an interface to a cloud-based repository management system. GitHub is an online interface for Git. Git is software used locally on your computer to record changes. GitHub is a host for your files and the records of the changes made. You can sort of think of it as being similar to DropBox - the files are on your computer, but they are also hosted online and are accessible from any computer. GitHub has the added benefit of interfacing with Git to keep track of all of your file versions and changes. 

Another way of thinking of it is as a big room with lots of large filing cabinets. Each filing cabinet contains the files associated with a particular project. These files have been created and are being edited by one or more people who have access to that particular filing cabinet or repository. GitHub allows you to control who can see and access your files.

GitHub uses the version control system Git, described above, to manage version control, and provides users with a web-based interface for creating projects, sharing them, updating code, etc. In this course, we will be teaching you how to do version control using GitHub. We will introduce you to the basics of working with GitHub, both through your browser and through RStudio. For our purposes, you will not need to think about Git itself, just use GitHub.

### Version control vocabulary

There is a lot of vocabulary involved in working with Git, and often the understanding of one word relies on your understanding of a different Git concept. Take some time to familiarize yourself with the words below and read over it a few times to see how the concepts relate. 

**Repository:** Equivalent to the project's folder/directory - all of your version controlled files (and the recorded changes) are located in a repository. This is often shortened to **repo**. Repositories are what are hosted on GitHub and through this interface you can either keep your repositories private and share them with select collaborators, or you can make them public - anybody can see your files and their history. 

**Commit:** To commit is to save your edits and the changes made. A commit is like a snapshot of your files – Git compares the previous version of all of your files in the repo to the current version and identifies those that have changed since then. Those that have not changed, it maintains that previously stored file, untouched. Those that have changed, it compares the files, logs the changes and uploads the new version of your file. We’ll touch on this in the next section, but when you commit a file, typically you accompany that file change with a little note about what you changed and why. 

When we talk about version control systems, commits are at the heart of them. If you find a mistake, you revert your files to a previous *commit.* If you want to see what has changed in a file over, you compare the *commits* and look at the messages to see why and who. 

**Push:** Updating the repository with your edits. Since Git involves making changes locally, you need to be able to share your changes with the common, online, repository. Pushing is sending those committed changes to that repository, so now everybody has access to your edits.

**Pull:** Updating your local version of the repository to the current version, since others may have edited in the meanwhile. Because the shared repository is hosted online and any of your collaborators (or even yourself on a different computer!) could have made changes to the files and then pushed them to the shared repository, you are behind the times! The files you have locally on *your* computer may be outdated, so you pull to check if you are up to date with the main repository. 

**Staging:** The act of preparing a file for a commit. For example, if since your last commit you have edited three files for completely different reasons, you don’t want to commit all of the changes in one go – your message on why you are making the commit and what has changed will be complicated since three files have been changed for different reasons. So instead, you can stage just one of the files and prepare it for committing. Once you’ve committed that file, you can stage the second file and commit it. And so on. Staging allows you to separate out file changes into separate commits. Very helpful! 

To summarize these commonly used terms so far and to test whether you’ve got the hang of this, files are hosted in a **repository** that is shared online with collaborators. You **pull** the repository’s contents so that you have a local copy of the files that you can edit. Once you are happy with your changes to a file, you **stage** the file and then **commit** it. You **push** this commit to the shared repository. This uploads your new file and all of the changes and is accompanied by a message explaining what changed, why and by whom. 

**Branch:** When the same file has two simultaneous copies. When you are working locally and editing a file, you have created a branch where your edits are not shared with the main repository (yet) - so there are two versions of the file: the version that everybody has access to on the repository and your local edited version of the file. Until you push your changes and merge them back into the main repository, you are working on a branch. Following a branch point, the version history splits into two and tracks the independent changes made to both the original file in the repository that others may be editing, and tracking your changes on your branch, and then merges the files together. 

**Merge:** Independent edits of the same file are incorporated into a single, unified file. Independent edits are identified by Git and are brought together into a single file, with both sets of edits incorporated. But, you can see a potential problem here – if both people made an edit to the same sentence that precludes one of the edits from being possible, we have a problem! Git recognizes this disparity (**conflict**) and asks for user assistance in picking which edit to keep. 

**Conflict:** When multiple people make changes to the same file and Git is unable to merge the edits. You are presented with the option to manually try and merge the edits or to keep one edit over the other. 

![A visual representation of these concepts, from https://www.atlassian.com/git/tutorials/using-branches/git-merge](images/00_version_control/00_githubbasics_version_control-14.png)

**Clone:** Making a copy of an existing Git repository. If you have just been brought on to a project that has been tracked with version control, you would clone the repository to get access to and create a local version of all of the repository’s files *and all of the tracked changes.*

**Fork:** A personal copy of a repository that you have taken from another person. If somebody is working on a cool project and you want to play around with it, you can fork their repository and then when you make changes, the edits are logged on *your* repository, not theirs. 

### Best practices

It can take some time to get used to working with version control software like Git, but there are a few things to keep in mind to help establish good habits that will help you out in the future. 

One of those things is to make purposeful commits. Each commit should only address a single issue. This way if you need to identify when you changed a certain line of code, there is only one place to look to identify the change and you can easily see how to revert the code. 

Similarly, making sure you write informative messages on each commit is a helpful habit to get into. If each message is precise in what was being changed, anybody can examine the committed file and identify the purpose for your change. Additionally, if you are looking for a specific edit you made in the past, you can easily scan through all of your commits to identify those changes related to the desired edit. You don't want to get in the same habit that [xkcd](https://xkcd.com/1296/) has!

Finally, be cognizant of the version of files you are working on. Frequently check that you are up to date with the current repo by frequently pulling. Additionally, don't hoard your edited files - once you have committed your files (and written that helpful message!), you should push those changes to the common repository. If you are done editing a section of code and are planning on moving on to an unrelated problem, you need to share that edit with your collaborators! 

### Summary

Now that we've covered what version control is and some of the benefits, you should be able to understand why we have an entire course dedicated to understanding it! Additionally, we looked at what Git and GitHub are, and then covered much of the commonly used (and sometimes confusing!) vocabulary inherent to version control work. We then quickly went over some best practices to using Git -- but the best way to get a hang of this all is to use it! Hopefully you feel like you have a better handle on how Git works than the people in [this xkcd comic](https://xkcd.com/1597/)!

### Slides and video

This lesson's slides can be found [here](https://docs.google.com/presentation/d/1nBgMcaXeF-hz5hX6712d_LC9Zm04s2mSCjuGECuht0M/edit?usp=sharing)  
This lesson's video can be found [here]()

### Quiz

{quiz, id: quiz00_versioncontrol}

? What is one way we can think of a GitHub repository?

a) A file cabinet that only you have access to.
B) A file cabinet that you and other people may have access to.

? Which of these is not true about using a version control system?

a) Version control allows you to go back if you make mistakes.
b) Version control is a way to allow multiple people to work together on a set of files for a project.
C) Version control is time-consuming and difficult to use.
d) Version control helps make sure that you do not lose work that you have done.

? Fill in the blanks. 

I'm done editing a file, I need to ______ those changes then _______ them, and ______ it to the ________?  

a) Commit, merge, push, repository
B) Stage, commit, push, repository
c) Pull, push, commit, branch 

? What is a good example of a message to accompany a commit ?  

A) Modified linear model of height to include new covariate, genotype   
b) Fixed problem with linear model  
C) Added genotype  
d) Fixed.

{/quiz}
