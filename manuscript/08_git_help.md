# Version Control Help 

We've previously discussed how to get help generally (Google!) and in the future we'll cover how to get help when you're stuck coding in R; however, at this point it's important to briefly discuss getting help when working with a version control system like GitHub.

In the lessons in this course we've covered a number of important git commands, such as clone, status, pull, push, add, commit, etc. As you're learning these commands and getting more comfortable with how to use them, you will certainly make mistakes. There are ways using git commands to revert back to previous versions (previous commits) of your GitHub repo and to fix merge conflicts (which often arise when multiple people are editing the same file at the same time). However, the ways in which you will make mistakes using git commands is not necessarily predictable. Because of this, we aren't going to walk you through any "this is how you fix that common error" tutorials. 

Instead, we're going to walk you through how to find the answer to the mistake you made yourself. While there are many ways to make a mistake on GitHub, take solace in the fact that you probably aren't the *first* person to have made this mistake. This means that the answer to your error is likely to be found on the Internet!

### Google for git help

When you're getting merge conflicts or errors when trying to run git commands in the Terminal, Googling the specific error message you're getting can be very helpful. For example, if you're getting a merge conflict error on GitHub, you may want to Google "git merge conflict help" to start you on your path to git merge conflict recovery.

![Google: "git merge conflict help"](images/08_git_help/08_githubbasics_git_help-1.png)

Or, if you've changed some documents, realized you didn't actually want to make those changes, and want to revert back to a previous commit, you may google "git revert to previous commit"

![Google: "git revert to previous commit"](images/08_git_help/08_githubbasics_git_help-2.png)

In both of these cases, links that will be helpful in figuring out your issue are provided and what git commands you'll want to try to recover from your mistake. 

By clicking on the links and following the instructions provided, you'll often be able to solve your problem. However, some links will be more helpful than others. Help from places like [Stack Overflow](www.stackoverflow.com) (www.stackoverflow.com) and [help.github.com](help.github.com) are good places to start. Additionally, as you practice and get more comfortable with git and GitHub you'll make fewer mistakes and understand the process even better! 

### Burn it Down

That all said, while sometimes Googling can be incredibly helpful, it's important to remember that git and GitHub are tackling incredibly difficult problems (version control and tracking changes is no simple task!). This means that while trying to track all your changes and use git commands, you may run into trouble that Googling won't help you solve. For times when  you've made a lot of changes and are struggling to even track down what it is you've done and what you want the GitHub repository to look like when it's all better. For these cases, it's best to just do what is referred to as "burning it all down," the process of which is described in [a chapter](http://happygitwithr.com/burn.html) of Jenny Bryan's *Happy Git with R* and captured perfectly in this [xkcd cartoon](http://explainxkcd.com/wiki/index.php/1597:_Git). 

Briefly here, for those worst-case scenarios when your GitHub repository and your local copy just cannot get to a happy place where you can push and pull with ease, you'll likely just want to:

1. move the files and directories from your local copy to a safe space that is separate from the directory you've cloned from GitHub. It's best at this point to rename the directory.
2. Once your files are in a safe (and different) directory, you'll want to clone the repo from GitHub again (which takes the last happy copy from GitHub and makes it available to you locally). You are now back to a safe state where you can easily push and pull. 
3. You're then ready to copy all the files from the safe directory back to this newly-cloned and happy repository. 
4. After the files have been returned, you'll want to *stage (git add), commit, and push* your files back to GitHub. 

While this is not a particularly elegant solution, it works in your most desperate times of need! Practice these steps now so that you know how to use them when you actually need them. And trust me, if you're new to git and GitHub, you'll probably need them.

 
### Summary

This lesson is intentionally short. There are lots of ways that git and GitHub will seem frustrating as you learn to use them. Remember that this is because git and GitHub are tackling difficult problems. When you run into issues with git and GitHub, the best thing is to look to the Internet for help. Read the answers online, think about whether they'll work for the issue you're having, and then give them a try. As you get more comfortable working with git for version control, you'll run into fewer and fewer of these problems. However, in the meantime, use the Internet for help, and when all else fails, just burn it all down.

### Additional Resources

* [Happy Git and GitHub for the useR](http://happygitwithr.com/reset.html), by Jenny Bryan
* [GitHub Help](https://help.github.com/)


### Slides and Video

![Version Control Help](https://www.youtube.com/watch?v=l2K3zWYEJBE)

* [Slides](https://docs.google.com/presentation/d/1Aj1Y0lIYdKftZVzAjWCWkOd8c0-IxnxtPbBmIUOdYC4/edit?usp=sharing)


{quiz, id: quiz_08_git_help}

### Version Control Help quiz

{choose-answers: 4}
? What does it mean when we say "burn it all down" with regards to a GitHub repository?

C) Move files to a new directory locally and re-clone the repo before moving files back and pushing to GitHub.
C) Move files to a new directory locally, re-clone the repo, then move files back into version control repo before pushing to GitHub.
o) Delete your GitHub account and all repositories to start completely over.
o) Delete the GitHub repository and push local changes.
o) Make a duplicate repository on GitHub and just start working there.
o) Tweet out issue you're having with GitHub and hope someone knows how to help.
o) Google how to solve your issue and read through solutions from others.

{choose-answers: 4}
? When you run into a problem using git and GitHub, what's the first thing you should do?

C) Google how to solve your issue and read through solutions from others.
C) Use the Internet to see if anyone else has had a similar issue and solved it.
o) Move files to a new directory locally and re-clone the repo before moving files back and pushing to GitHub.
o) Delete your GitHub account and all repositories to start completely over.
o) Delete the GitHub repository and push local changes.
o) Make a duplicate repository on GitHub and just start working there.
o) Tweet out issue you're having with GitHub and hope someone knows how to help.

{choose-answers: 4, points: 2}
? What git command will you want to run if you realize you want to change the message on your last commit (Hint: This has not been directly discussed in this lesson. You'll need to Google to determine the answer!)?

C) `git commit --ammend`
o) `git commit --message`
o) `git fix`
o) `git --rename commit`
o) `git edit commit`
o) `git edit --ammend`
o) `git edit --message`

{/quiz}
