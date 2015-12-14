# About Git And GitHub

## Basic instructions for the newbie Git user

**disclaimer**: I'm offering this page as some guidence to those just starting off with Git and GitHub. I'm not an expert (just a student like yourself). 

### some basic training and books that I've used in the past

[www.pluralshight.com](www.pluralsight.com) has some on-line training for Git and GitHub (and they offer a free 10 day trail so you can so all of these if you wish)

* Introduction to Git
* Git Fundamentals
* GitHub for Windows Developers

A book that I've found useful: *Version Control with Git*  by Jon Loeliger (first 88 pages)

### My invironment
I'm using Windows 7 and currently use R version 3.2.3.

I've also install GitHub Desktop (https://desktop.github.com/) but make use of the bash shell (see more about this below)

### Basic Steps (for getting some files up to GitHub)

Here is what I did to get started using Git and GitHub.

I'm using GitHub Desktop but I'm mostly using the Git Shell that comes with it versus
the GitHub GUI. Note that Git shell (at least for me) was installed with Windows Powershell instead of Bash for the
shell app. I needed to open the GitHub GUI and go to settings to get it to default to the bash shell.
The GUI has a little 'cog' icon in the upper right of the window. Click on it and select Options to set the Default
shell to Git Bash.

Get yourself a GitHub account (I assume this is not an issue for you)

I find it easier to always create a repository on GitHub and clone it to my local machine (versus starting at the local and going the other way):

1. create the repo on GitHub (or create a fork...depends on the course and project you are working on)
2. copy the repo https address (for use in your git bash on your local machine). Here is an image of what I'm talking about off a repo on GitHub:

![github repo page](./figureA.JPG)

3. open up your git bash shell and navigate to whereever you wish to put your new repo folder
4. type the following:
```
git clone <paste your https address from step b here>
```
5. Now you can just copy,paste files to his new folder on your local machine.
6. you will need to add these new files to your local git repo like so:
```
git add .
```
7. and you will need to commit these changes to your local repo like so (use some sort of reason why you are committing this change):
```
git commit -m "Initial Revision"
```
8. now you should be ready to push your changes up to your GitHub repo like so:
```
git push
```
NOTE: I've found using the status command very useful in keeping track of what is going on (and what I might have missed). So you might want to periodicly type this:
```
git status
```

Some basic notes about Git. It does not really care much about file names. It is looking at file contents.
So if you have already added a file foo.txt and you have changed foo.txt, you will need to 
add it again (since you are asking git to update your repo with new file contents)
