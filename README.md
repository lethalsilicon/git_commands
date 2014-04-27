git_commands
============

This file was to practice GitHub and Git Bash (Use Raw View to see this file properly)

Here is how you use GitHub:

Step 1: Create a Repo(Project) on Github. Just click "New Repository" and make sure to initialize a README.md file.

Step 2 (Optional): Fork a Repo. Go to someone else's repo and click "Fork Repository" button. This clones the repo to your Github account on GH's servers.

Step 3 (Startup): Install Git Bash (Mac already has Terminal).
	To check Git version #:
		git --version
	To configure Git for your Github account:
		git config --global user.name "lethalsilicong5"
		git config --global user.email "samalegria@gmail.com"

Step 4: Clone a Repo. We are copying the project from Github's servers on to our computer.
	Use cd and ls in Bash to get to the directory you want repo to be in.
	To clone repo (use Clone Url located on repo's page.):
		git clone https://github.com/lethalsilicong5/open-sourcerer.git
	Add original repo (if this was forked):
		git remote add upstream https://github.com/diy/open-sourcerer.git
	Make sure you have latest updates:
		git pull upstream master

Step 5: Push changes. After you've done any changes to the files.
	You can check status of the repo:
		git status
	You can check where the differences are (if any):
		git diff
		Press "q" to exit diff!
	If you want to add a file you changed:
		gid add FILENAME.EXTENSION
	Don't forget to write a comment:
		git commit -m "Fcuking Comment"
	To push files:
		git push origin master
	Then just write username/password for GitHub

step 6 (Errors): Merge Conflicts. I googled. Found this link. http://stackoverflow.com/questions/161813/how-do-i-fix-merge-conflicts-in-git
	Try this:
		git checkout --ours FILENAME.EXTENSION (Pick yours)
		git checkout --theirs FILENAME.EXTENSION (Pick theirs)
		git add FILENAME.EXTENSION (Then standard procedure)
		git commit -m "using ours (or) theirs" (With comment)


Step 7: Submit a Pull Rgitquest. If you edited someone else's repo and want to add it to theirs. Look for the "Pull Request" button on your repo page.