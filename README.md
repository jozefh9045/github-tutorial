# GitHub Tutorial

_by Jozef Hernandez_

---
## Git vs. GitHub

Git and Gihub are tools that not only coders, but anyone who wants to keep track of a project, use to keep previous versions of a file and allow others to make their own version of a file.  
  
###Git
* Git is a tool on the command line that allows you to keep track of previous version of a file or project using snapshots.  
  
###Github
* Github is a website that allows you to upload screenshots of your file or project where you can clone your work from the website into another computer and work on it from there.

---
## Initial Setup

###How to Start Using Git
1. First off, you'll need to go to a command line workspace, like [Cloud9](https://c9.io), for example. You'll have to make an account to be able to work on it, but you can use a Github account to log onto Cloud9, so make a Github account first and log onto Cloud9 with the Github account.
2. Then you'll have to put your c9 SSH key into your Github. Go to your settings page in Github and click SSH keys. Click "Sdd SSH Key" and name it Cloud9. To get your Cloud9 SSH key, go to c9.io and click on the gear icon at the top right and at the left, click "SSH Keys". Copy the block of characters and paste it into your Github.
3. Next, once you make your workspace, it'll be good to make a new directory, so you can use this command:
```
mkdir learning_git
```  
_mkdir_ stands for "make directory", the command line will then make a directory and name it the second word in the command, which is *learning_git* in this case.  
4. So you've made the directory, but you don't want to make a repository in the root folder, you want it in the *learning_git* directory, so you'll have to move into it using _cd_:
```
cd learning_git
```  
_cd_ means "change directory". It moves you into the folder name you put after _cd_, here it'll move us into the *learning_git* directory.  
5. You'll want a file to keep track of, so let's make a README file. This command will make the file:
```
touch README.txt
```  
The _touch_ command makes files, here you made a text file named _README.txt_. Text files can be edited to contain a message. To edit the text file, look at the left of your command line and you'll see a folder named "learning_git". Click on it to reveal your README text file, then click on the file to edit it on the window above the command line. After typing something, remember to save it in the "File" tab!

---
## Repository Setup

###How to Start Using Github

1. Before you do anything, you should set up your name and email so commits you make will have your name and be linked to your Github account. The commands to do this are:
```
git config --global user.name "[Your Name]"
git config --global user.email "[Your email]"
```
In the first command, put your name in the place of [Your Name] (replace the brackets, too). This will put your name on any commits you make to give you credit.  
In the second command, your email should be in the place of [Your email] (like the first command, replace the bracktes). This command will link any commits you've made to your Github account.  
2. Next, use:
```
git init
```
This will start a new repository in your current folder, *learning_git*. Think of a repository as a photo album that keeps all of your snapshots.
3. Next, you'll have to use:
```
git add *
```
This command, _git add *_, will metaphorically put all files onto the stage so that you can take a picture of them (you can add indivisual files by putting their name instead of the *). You can screenshot thm using:
```
git commit -m "[message]"
```
The _commit_ part will take a metaphorical picture of your code to put in the metaphorical photo album so that you can go back to it later. The _-m "[message]"_ will leave a message on the snapshot. Replace the [message] part with your own message about the snapshot in the present tense.
3. To link this repository to a repository in your Github, you'll have to click the plus at the top right, and click new repository. Name it the same as your folder (learning_git) and click continue. In the section called "Quick setup — if you’ve done this kind of thing before", make sure it has SSH selected. Then follow the commands in the "…or push an existing repository from the command line" section. The first one will link the repositories and the 2nd one will put your README.txt into the Github Repository.

---
## Workflow & Commands

* Congratulations! You've set up your repository and it's on Github! Here's some notes if you want to work on your repository in the future.
* So, maybe you'll want to edit the text file or add something into the repository. When working in the command line, it'll be useful to use:
```
git status
```
* This command will tell you if you have unadded files (red), added files (green), or if nothing has changed (it'll say "nothing to commit").
* When the  message is red, use this command: _git add *_.
* When the message is green, use _git commit -m "[message]"_.
* When you've edited a file but it shows "nothing to commit", it's probably because you didn't save. You can save manually by clicking "File" at the top left and clicking save. You can turn autosave on by clicking the gear icon on the top right, go to "User Settings", click "Save", and turn on "Enable Auto-Save".