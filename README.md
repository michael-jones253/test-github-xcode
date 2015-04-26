# test-github-xcode
This project is empty except for the following instructions on how to set up an Xcode 6 project to work with Github. I have seen some instructions for Xcode 5 which involved a number of git commands in the shell, however the following is all I needed to do for Xcode 6 and uses just one git command line instruction:

Create Xcode project and select the option for Create git repository on local mac.

Login on the Github website and create a repository. I did not initialize with a README.md file, because of the hint "Skip this step if you're importing an existing repository".

Copy the remote add command - I used the https one. Then on the command line on local mac change directory into the project directory, paste in the remote add command which in this case was:

git remote add origin https://github.com/michael-jones253/test-github-xcode.git

Go back into Xcode and select the menu option: source control-> push. Choose the remote repo.

Can now add a README.md on the Github webpage. Then pull that README down to the local mac using source control -> pull.

Any changes that are done in Xcode need to be committed locally first before pushing up to Github. Any changes done on the Github repository webpage need to be pulled down first into Xcode before pushing further changes up - an error dialog will pop up otherwise.

