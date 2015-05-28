Quick Start Guide
=================

This guide will get git set-up for you and allow you to start contributing to a repository.

First install git: [http://git-scm.com/downloads](http://git-scm.com/downloads) Just use the default option when installing.

Now that you have git installed open a terminal widow (or start Git Bash on windows).

One quick thing before we get started is to tell git your identity. In the terminal or Git Bash run:

	git config --global user.name "mbrenn3" (obviously use your user name)
	git config --global user.email email@uic.edu

First you'll want to navigate to a directory (folder) that you want to put the repository (git folder). [Here is a quick reference for commands for navigating directories in the command line](http://www.st-andrews.ac.uk/ITS/training/unix/unix1.html)  *Tip: you can drag a file or directory into the terminal or bash window to paste it's location.*


For this example we will put the git repository in our Documents folder. So first get to that folder by running:

	$ cd Documents

Now find the repository on GitHub that you want to work on and clone it. At the bottom of the right side of a GitHub repository page you should see a clone URL. Below is the command for cloning the oxygen measurement repository. *Tip: you can copy the URL and then paste it into Git Bash with the 'insert' key.

	$ git clone https://github.com/Biological-Microsystems-Laboratory/oxygen-measurement.git

Now when you look in your Documents folder you will see a new directory 'oxygen-measurement'. Now in the in the command line change to that directory:

	$ cd oxygen-measurement

Now you may open and edit any files in the directory and add or delete files. When you have made changes that you want to save, first save the files normally. Then you will take a snapshot of the repository by 'committing' it. First you will want to run 'git status' to see what changes have been made:

	$ git status

This will show you any changes to tracked files (ones that that have been modified from earlier committed versions) and any new files to be added or files that were deleted. Running git status lets you see if there are any additional files that you may have accidentally added or any automatically created backup file that are not necessary to track. 

If you added new files that you would like to track run 'git add' followed by the file name. *Tip: again you can complete the file name with 'tab'*

	$ git add new-file.md

Now when you run 'git status' you will see that file as being marked to be tracked. Now you should be ready to commit the changes. Type the command below. The '-m' are flag that is a short-cut. It lets you enter your commit message in-line without opening and editor. The -a flags is also a shortcut. It tells git to commit changes made to file that were modified.

	$ git commit -am 'this is my commit message'

Now that you have a commit you are ready to push changes to GitHub. (Note: you can make a series of commits before pushing. You don't need to push after every commit.) Run:

	$ git push

You should be prompted to enter you user name or email for GitHub and your password. (note: when you enter your password the line will just remain blank. Just type it and press enter)

Now when you check the GitHub page you will see your changes made.

If someone has pushed changes since you last cloned or pulled, your push will be rejected. You need to pull the latest changes before you can push. Don't worry git will usually merge the changes automatically for you. Run:

	$ git pull
	$ git push

Also when ever you begin working again make sure to pull the latest changes before working

	$ git pull


tips
----
use insert to paste in widows in Git Bash
