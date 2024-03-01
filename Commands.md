# Commands

- `git init` -> initialize my timeline (my git repo)

- `git add` -> put file in stage area 

- `git commit -m "meaningfull message"` ->

        Important:

        - Why

        - How

        - Effects

        - Limitations

- `git status` -> check in what conceptual area your file/folder is
  
  - Verify uncomitted changes
  - Verify staged unchanged files
  - verify untracked files (never added before in git)

- `git log` -> check history of every snapshot you have ever saved in you local repository. Contains, who, when, msg and commit ID. Press q for quit if many commits
  
  - `git log --help` 
  
  - `git log -n <n°>` -> if n = 5 you will see last 5 commits
  
  - `git log --abbrev-commit` -> 

- `git show <commit ID1> <commit ID2>` -> to compare two versions with eachother. Everything in green is added, in red is deleted. This shows what happend in ID1 and then what happend in ID2

- `git diff  <commit ID1> <commit ID2>` -> same but really comparing the difference between ID1 and ID2

- `git remote add <name> <ssh>`-> connect to a remote repository on github! 
  Creates a bridge between local repository and remote repository. 

- `git push`-> everything commited will be pushed to the remote github (if already pushed before, it will only push the new changes)

- `git rm <file>` -> remove file that has been committed. Still need to commit again and push in order to delete if from the githhub remote. (DELETES WHOLE FILE)

- `git reset <file>` -> to unstage a file that has been added.

- `git pull` to sync back from the github repository to local repository 
  Works both ways with push -> need to syncronise before you start adjusting. 

- `git rebase` -> Rebase a commit on current tip (work on older folder but it overwrites current file).

- `git revert` -> Can revert files out of staging area. Can also revert a file thats been committed. See -help to see more option. HEAD refers to latest commit. Git HEAD will revert 1, Git HEAD~1 will revert 2 back1.
  Git won't allow to revert if any other files are still in the three. Can also revert a revert!

- `git clone <ssh url (or HTTPS url) from github repository>` -> Will clone a repository from the github to your folder. 
  Use this if you want to retrieve github codes from someone else. 
  Can be usefull if you deleted the folder with Git inside. (In the same state it was last pushed before). 
  No need to git init or make bridge, it will be able to 'pull' everything. Just make sure you don't clone it into a folder where a git is already present.
  Can use HTTPS link if you use someone else his repository eg you want to use their code. This way you can't push changes to his github. 

- `git branch <name>` -> Create new branch. If you create new branch, first commit will be the commit you branched from the original one. <name> is the name you give the branch. 

- `git branch --list` -> Gives list of branches. Also lets you see in which you are (green highlighted)

- `git branch -a` -> more powerfull than git branch list as it lists everything. (Sometimes on first pull from github, you can't see all the branches).

- `git switch -c <name>` -> create branch

- `git switch <name> <ID>` -> Create branch from detached head (ID).

- `git checkout <branch_name>` -> Use to move through branches
  Also used to move between commits! (but be carefull)

- `git merge <branche name>` -> to merge branches. 

- `git branche -d <branche name>` -> to remove branch. If branch already merged. It still appears in branchlist because it contains the history log of the branch. If you delete it, it only deletes the history. 

- `git tag <name> `-> Will tag the commit you are in with <name> so its easy to find or checkout to via that name. You can give multiple tags to the same commit. 

- `git push --tags`-> to push the tags. `git push` won't push the tags.

- 
