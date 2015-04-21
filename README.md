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

## Configuring Git
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


## Creating Repos
Create a new repository which you want git to track changes. :footprints:
### New repos
* Change directory to the newly created folder
		$ cd [path_to_folder]
* Initialize git. Tell git to track changes :footprints:
		$ git init 

		This creates a .git folder which now helps in keeping track of every change made in that folder alone.

### Existing repos
* Online repos
		$ git clone [url_to_the_repo] "name_of_folder"[optional]

		This downloads a project and it's entire version history.




















