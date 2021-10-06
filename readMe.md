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
-- git checkout [file name.format]
to roll ack to previous version

-- git status
to see tracked files(shows in green) and untracked files(shows in red)

-- 
