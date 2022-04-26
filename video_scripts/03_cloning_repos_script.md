Now that you have learned how to create a GitHub repository, you will learn how to obtain a copy of that repository in a location that you use for writing code such as RStudio Cloud. This process is called "cloning" a repository from GitHub.

Within a project in R Studio Cloud, navigate to the Terminal tab, indicated in the picture here. This is where you can type Git commands to work with repositories. The text that you see at the beginning of the line in the Terminal is called the prompt. When you see the prompt at the beginning of a line, this indicates that the Terminal is ready to accept your commands.

Next, navigate to the GitHub webpage for your repository. This URL always has the form h t t p s colon slash slash git hub dot com slash git hub username slash repository name. On this page, you will see a button on the right hand side that says "Clone or download". When you click this, highlight the URL in the box, and copy it to the clipboard. Make sure it starts with h t t p s rather than git at. If you see git at, click the link in the top right corner of the box that says use h t t p s.

Navigate back to the Terminal tab in R Studio that you opened in Step 1. Type the command: git clone. Then paste the URL that you copied in Step 2. Then hit Enter. You will see some status text appear as the repository is being cloned to a location on R Studio Cloud. When this is complete, typically after a few seconds, the Terminal prompt will appear again on a new line, indicating that you are able to input new commands if you wish. Also note that in the bottom right hand corner of R Studio, in the Files pane, you will have a new folder that has the same name as your Git repository.

A big part of staying organized with your files is understanding how folders in your project are organized. Also important is the concept of a working directory. Whenever you are working in R or the Terminal, you are housed in some folder. This folder is called the working directory. Knowing this is important so that you know how to specify paths to other important folders in your project. We can see what the current working directory is in a number of ways. In the image below, we can see from the Terminal prompt that the working directory is slash cloud slash project. We can also see this in the Files pane. We see that the first level folder is cloud and that the second level folder is project.