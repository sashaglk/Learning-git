Practical task

The following list of actions diplays cases that can occur in real-life scenarios while working on a project.
The commands shown below each action are command line insructions that help complete a corresponding action above them.
The creation of these commands have been the goal of this practical task.


1. Create a GitHub account. 

2. Create a repository on your github (smth with the name about learning Git). 

3. Add a file to your repository via GitHub web UI. 

4. Install Git on your PC/laptop. 

5. Write a command to create a local copy of the GitHub repository from Step 2 (clone) - via CLI (command line interface). 
git clone git@github.com:sashaglk/Learning-git.git 

6. Make changes to the local copy of the file from Step 3. 
cd Learning-git
nano 1stFile.py

7. Add one more file to your local repository. 
touch 2ndFile.py

8. Check the changes between the local file from Step 6 and that in the repository (from Step 3) - via CLI. 
git fetch
git add 1stFile.py
git diff --staged

9. Check the files that are different in your local repository in comparison with the remote one on GitHub, commit and push changes to the remote repository - via CLI. 
git fetch
git add .
git diff --staged
git commit . -m 'Step 9 - done' 
git push 

10. Create a branch in the remote repository and make some changes in the file from Steps 3, 6 so that it was different from master branch - via GitHub web UI. 

11. Clone the remote branch to your local copy of the repository - via CLI. 
git fetch

12. Make some changes in the file in the branch and "stash" them so that they were not visible to Git - via CLI.
git switch other
git nano 1stFile.py
git stash 

13. Switch to the master branch and "unstash" the changes from Step 12, commit and push them to the file in master branch - via CLI. 
git switch main
git stash apply
git add .
git commit . -m 'Step 13 - done'
git push

14. Add the list of commands from all previous steps to one more file and commit it to master branch. 
touch listOfCommands.txt
nano listOfCommands.txt
git add .
git commit . -m 'Step 14 - done'

15. Add a few files with the names test1.txt, test2.txt, test_aaa.txt to your local repository and update it so that they were invisible to Git (ignored). 
touch test1.txt test2.txt test_aaa.txt .gitignore
nano .gitignore

16. Add an .md file to your repository with the description of the task (all Steps above this one) and maybe a few more sentences describing its purpose.
touch task.md
nano task.md
