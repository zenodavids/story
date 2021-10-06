///////////// CREATING A GIT LOCAL REPOSITORY



1 --initalize git using the terminal
-make sure you are in the project root directory and initalize git.
=git init=

2 --to show the status of your files.
=git status=
-tracked files will be shown in green, untracked files will besshown in red.

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

-- git checkout [file name.format]
to roll ack to previous version
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

///// 


