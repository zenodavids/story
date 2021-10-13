///////////// CREATING A GIT LOCAL REPOSITORY



1 --initalize git using the terminal
-make sure you are in the project root directory and initalize git.
=git init=

2 --to show the status of your files.
=git status=
-tracked files will be shown in green, untracked files will be shown in red.

3 --to start tracking the files in the project directory, we add the file(s) to a staging area(here, we decide if to send all or some of our files to the repository - what files git should add and git should ignore).
=git add chapter1.txt= (for one file)
=git add .= (for all files in the project directory)
- if we check the git status again (git status) the specific file(s) becomes green.

4 --next, we commit the file under VERSION CONTROL
=git commit -m "commit mesage"
-the '-m' in the command line above stands for message.
-the commit message is a compulsory description that is attached to that specific file version, saying what was changed or what was added. this helps keep track of what changes was made.
-it is advisable to use prsent tense when typing out the commit mesage.

5 --to see what commits we have made, we use the ;
=git log=

we can use steps 3 - 5 to keeping updating and adding files.
/////////
say we are writing a book, we completed chapter 1 and added chapter 2 and 3.
//////////////////////
//// other GIT commands

-- git init
this initalizes git and it was be done in the terminal of the working diectory.

-- git status
to see what is in the staging area (after intializing git).
tracked files(shows in green) are in the stage area and untracked files(shows in red) are not in the stage area.

-- git add [filename.fileformat]
-- git add .
fist one adds a paticular file to the stage area
second adds all the files in the working diectory to the stage area.

-- git commit -m 'description of the commit version'
this saves a particular version of the specific file on git.
and the message is written in present tense.

-- git log
to see what commits you have made, the name of the author and time the commit was saved.

-- git checkout [filename.format]
to roll ack to previous version

-- git rm --cached -r .
to remove all the files from staging area(just before you commit them)
/////////////////////////////////////////////////////////////////////

////////////// MOVING THE GIT LOCAL REPOSitory TO GITHUB REMOTE REPOSITORY.
-- sign in to your github acount
-once in, at the top right, click on the '+' sign and select 'new repository'
-give the repository a name, preferably the name of the web app.
-next, type the description in the description box.
-check the 'public' box.
-click on 'create repository'

--moving the local repostory to the github repository.
-copy the address of the github repository,
-go to the command line, make sure you are in the working directory and type this code to create a remote repository in your github profile;
=git remote add origin [the copied address of the github repository]=
-add follow the instructions.
-next we use;
=git push -u origin master=
-what this code does is it pushes all your local repository to the to your github remote repository using the '-u' flag to basically link the local and the remote repositories.
and we push it towards the remote called 'origin' and push it to the branch called 'master '.
-refresh the page and all of our files will be shown on github.
-click on 'insights' and 'network' and you will see the master branch and the number of save points.
-hover over them to see the commit messages of each one.

///// UPDATING THE FILES AND ADDING THE UPDATE
--saving up on local repository
-git add [filename.fileformat]
-git commit -m [commit-message]

--saving it on the remote repository (GITHUB)
-git push

/////////////////////////////////////////////////////////////

///// GITIGNORE

this hides sensitive information that we dont want to be hosted, ie;
-API keys,
-Ds_Store :- this is a settings file that saves seting things i.e the arrangement of files/pictures/images in your folder. this is also a hidden file.

--SETTING UP GITIGNORE
--create the file.
-in your terminal, make sure you are in your working directory and type this code;
= touch .gitignore =
-to confirm if it is there, use this code below and what it does is it lists out all the files and folder in that directory, including hidden ones;
=ls -a=
-then we open gitignore.
=open .gitignore=
-next we add/type the file names of the files/folders we dont want to be added to git - exactly the same upper and lower letter casing the name of the file will hsve and their format.


///// GITINORE CODES
-- #
we can use the pound sign (#) to comment,

-- *
say we want to hide all the files with the format '.txt', we use '*.txt' to easily  add them all, instead of typing them one by one.

////////////////////////////////////////////////////////////////////////////////////////


//////// GIT CLONE

this is when a repository/poject is download from github website to your local device.
-go to the repository that you want to download.
- click on it and at the top left corner, you will see a green button named 'download' or 'code' and you will be given the option to download the ZIP file and a url will also be shown there.
- copy the url, go to your terminal and cd into the directory that you want the project to be, then clone the project using;
=git clone [the copied url]=
this downloads all the files into your pc.

////////////////////////////////////////////////////////////////////////

////// BRANCHING AND MERGING

-by default, all projects have a branch named the 'master' branch. say we are working on a project and we want to test other options outside of the usal project but still maintain the original project, we create a different branch to store the test files seperate from the original files and we can still merge themif the test files actually makes sense.

-to create a new branch,
=git branch [name of new branch]=

-to see the branches in a project,
=git branch=
this shows all the branches in that project and the branch you are currently on will have the star sign(*) just before it.

-to switch between branches,
=git checkout [branch name you want to switch to]=
once youve switced, you ccan edit the files (note that the original files are still in the master branch) and to save the to the branch;
git add .
git commit -m [commit message]

