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
/////////////////////////////////////////////////

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
