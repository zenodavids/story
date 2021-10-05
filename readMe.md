///////////// CREATING A GIT LOCAL REPOSITORY

--initalize git using the terminal
-make sure you are in the project root directory and initalize git.
=git init=

--to show the status of your files.
=git status=
-tracked files will be shown in green, untracked files will besshown in red.

--to start tracking the files in the project directory, we add the file(s) to a staging area.
=git add chapter1.txt= (for one file)
=git add .= (for all files in the project directory)
- if we check the git status again (git status) the specific file(s) becomes green.

--next, we commit the file under VERSION CONTROL
=git commit -m "commit mesage"
-the '-m' in the command line above stands for message.
-the commit message is a compulsory description that is attached to that specific file version, saying what was changed or what was added. this helps keep track of what changes was made.
-it is advisable to use prsent tense when typing out the commit mesage.

--to see what commits we have made, we use the ;
=git log=


