# Dive into Git
Quick guide to the basics of using git | github.

If you need clarification, please raise an issue [Here](https://github.com/devsgroupuon/in2git/issues)

## What git is
Git is a distributed revision control system with an emphasis on speed, data integrity, and support for distributed, non-linear workflows. Git was initially designed and developed by Linus Torvalds for Linux kernel development in 2005, and has since become the most widely adopted version control system for software development. [Wiki](http://en.wikipedia.org/wiki/Git_(software))

## What git is not
Git is EVERYTHING
 

## Installing Git
Git basically provides GUI based client application as well as command line. 
Command line is powerful and is what we want to encourage devs to take on.

### GUI Based
* Github for Windows
	* [Open this Window](https://windows.github.com)

* Github for Mac
	* [Mac me here](https://mac.github.com)

### Command Line based(Terminal | CMD)

* Linux Users [Run the command in the terminal]
		
		Debian-based(e.g Ubuntu)
		sudo apt-get install git

		Fedora
		yum install git

* Mac Users
	* Mavericks and Yosemite
		* Install X-code and git will be installed

	* Mountain Lion and below
		* [Get it here](http://git-scm.com/download/mac)
			* Follow through the on screen installer. 

## Configuring Git:hammer: :wrench:
Configure user information for all local repositories.
### Run the following command on the terminal
	* Set the name you want attached to all your commints
			$ git config --global user.name "Your Name"
	* Set the email you want attached to all your commits
			$ git config --global user.email "your email address"
	* Enable helpful colorization in the command line output
			$ git config --global color.ui auto

###### This creates a .gitconfig file in your home folder. You can view the details by running
			$ cat ~/.gitconfig


## Creating Repos:footprints:
Create a new repository which you want git to track changes. :footprints:
### New repos
* Change directory to the newly created folder

		$ cd [path_to_folder]
* Initialize git. Tell git to track changes :footprints:

		$ git init 

		This creates a .git folder which now helps in keeping track of every change 
		made in that folder alone.

### Existing repos:globe_with_meridians:
* Online repos

		$ git clone [url_to_the_repo] "name_of_folder"[optional]

		This downloads a project and it's entire version history.


## Make Changes
Reviewing edits and crafting commit transactions

		$ git status
		~Lists all the new or modified files to be commited

		$ git diff
		~Shows file differences not yet staged

		$ git diff [filename]
		~Shows differences not yet staged for a particular file

		$ git diff --staged
		~Show file differences between staging  and the last file version

		$ git add [filename]
		~Creates a snapshot of the file in preparation for versioning

		$ git commit -m "[descriptive message about the change]"
		Records file snapshots permanently in version history


		$ git reset [filename]
		~Unstage a file but preserve its contents

## Synchronizing changes
Register a repo bookmark and exchange version history.

* Log in to [Github](https://github.com) and create a repo there.
* Copy the clone url for that repo
* To sync this online repo with a local repo open terminal and:
	
		$ git remote add [remote_branch_name] [clone_url]

* To publish local commits to your online repo open terminal and:

		$ git push -u [remote_branch_name] [master_branch]

		or

		git push

* Download online changes and incorporate changes to the local repo:

		$ git pull -u [remote_branch_name] [master_branch]

		or

		$ git pull



## Redo Commits
Erase mistakes and craft replacement history.

		$ git reset [commit_id]
		The commit_id is the hashed SHA1 40 digit character word.
		Only the first 7 characters are required though e.g.

		$ git reset [5de8d40]
		Undoes all commits after [commit], preserving changes locally.


		$ git reset --hard [commit]
		Discards all history and changes back to the specified commit



## Little hacks and tricks
Some shorthands to help quicken your gittiness :100:

		$ git commit -am "[descriptive message]"
		This adds new changes to the staging area and commits the changes at once

		$ git commit --amend -am "[descriptive message]"
		This commits changes made but overides the previous commit so that you only
		have one commit for say a change you forgot to add in the previous commit

		$ git add . ; git commit -m "[descriptive message]" ; git push
		Add all changes to staging area, commit them and push to the local remote at once









































