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

* Linux Users
	* Debian-based(e.g Ubuntu)
		* run *sudo apt-get install git*

	* Fedora
		* run *yum install git*

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

#### This creates a .gitconfig file in your home folder. You can view the details by running
			$ cat ~/.gitconfig



			
