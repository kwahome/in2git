# Dive into Git
Quick guide to the basics of using git | github. 

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



















































