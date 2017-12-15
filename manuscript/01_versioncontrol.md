# Version Control

## What is Version Control?

One common mantra from data analysis and writing code is "save early, save often". What is meant by this is that you do not want to create content without saving it frequently. This way, if you lose your internet connection, or your computer crashes, you will not lose the hard work you have put in. On the other hand, sometimes we create some content, only to realize that it is not what we want, and we want to undo the changes we have just made. *Version control* allows us to save frequently, while also taking snapshots of our work at any point in time, allowing us to go back to a previous version if necessary. A good version control system will do this without you having to save multiple copies of your work (myFile_version1, myFile_version2, etc.) or keep track of what the latest version of the file is.

## Version control on your own

As mentioned above, even if you are the only one working on a project, saving frequently and preserving snapshots of your work at a specific time prevents you from losing work or making changes that cause the work you have already done to not work anymore. 

## Version control for collaboration or sharing

One advantage of using version control for your projects is that multiple users can work on different parts of the same project at the same time. Each individual can edit different files that make up a project simultaneously, and all the results can be saved in the same place. Two (or more) individuals can even work on editing the same file simultaneously, and a good version control system will allow them to then resolve any differences between the two file versions that result. 

## What is Git?

In this course, we will introduce version control software called Git. Git is a specific implementation of a version control system that allows you to first save snapshots locally on your computer, called *committing* them, and then *push* them to a *repository* where they are saved on the cloud. Git will automatically create copies of the files as you make changes to them -- no need for you to save your own copy with different versions or different dates. This way you can easily keep track of what file you should be working on.

All of these terms will be made more clear in later modules. Briefly, committing saves a local copy of your work, like tucking it into a file drawer. Pushing creates a copy of your local files, and saves this copy on the cloud. You can think of a repository as a file cabinet that multiple people have access to, where you have put a copy of the files you were working on. Other people can see your files and edit them as well, depositing their own changes in the shared file cabinet. They can let you know that they have made changes, which you can then incorporate by *pulling* these changes from the cloud to your local files. This allows multiple people to work on the same set of files without having to keep track of who is editing when, and have multiple copies or versions floating around.

## What is GitHub?

GitHub is a website that provides an interface to a cloud-based repository management system. You can think of it as a big room with lots of large filing cabinets. Each filing cabinet contains the files associated with a particular project. These files have been created and are being edited by one or more people who have access to that particular filing cabinet or repository. GitHub allows you to control who can see and access your files.

GitHub uses the version control system Git, described above, to manage version control, and provides users with a web-based interface for creating projects, sharing them, updating code, etc. In this course, we will be teaching you how to do version control using GitHub. We will introduce you to the basics of working with GitHub, both through your browser and through RStudio. For our purposes, you will not need to think about Git itself, just use GitHub.
 
## Summary: Why is working with GitHub useful?

1 It gives you an easy way of saving a backup of your work as you go, making sure you don't lose anything you have created.
2 It allows you to go back to an earlier version of your work if something gets broken due to the changes you have made.
3 It allows multiple people to edit code at the same time, without worrying that what they’re doing might be messing someone else’s code up.

{quiz, id: 01_versioncontrol}

# Version control quiz

? What is one way we can think of a GitHub repository?

a) A file cabinet that only you have access to.
B) A file cabinet that you and other people may have access to.

? Which of these is not true about using a version control system?

a) Version control allows you to go back if you make mistakes.
b) Version control is a way to allow multiple people to work together on a set of files for a project.
C) Version control is time-consuming and difficult to use.
d) Version control helps make sure that you do not lose work that you have done.



{/quiz}
