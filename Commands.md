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

- `git revert` -> Can revert files out of staging area. Can also revert a file thats been committed. See -help to see more option. HEAD refers to latest commit. Git won't allow to revert if any other files are still in the three. Can also revert a revert!

- 
