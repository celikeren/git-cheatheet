# git-cheatheet

## basic
- `git init`  
    > _new git repo_  
    _creates the .git file_
    
- `git status`  
   > _info about the repo_  
   _current branch, staged files, if it's up to date etc._

- `git config user.email`  
   > _shows the configured email_  
   
- `git config user.name`  
   > _shows the configured name_  

- `git config --global user.name "<username>"`  
   > _sets the username_  
   
- `git config --global user.email "<email>"`  
   > _sets the email address_  

- `git config --list`  
   > _lists all properties_  


## intro
- `git clone <url>`
    > _downloads an existing repo_  

- `git pull` 
    > _gets the latest state_  

- `git add <file>`  
   > _stages the given file_  
     _more than one file can be given;_  
         `git add <file> <file> <file>`
- `git add -A`  
   > _stages all modified files_ 

- `git commit -m "<message>"`  
   > _commits with the given message, changes are still in local_  

- `git commit --amend -m "bla bla bla"`  
   > _updates the latest commit and/or message_  
   
- `git push`  
   > _sends changes to remote_  
  
## branches
- `git branch`  
   > _lists all branches and marks the current one_  
   
- `git branch <branch_name>`  
   > _creates a new branch with given name_ 
   
- `git checkout <branch_name>`  
   > _switches to given branch_ 

- `git checkout -b <branch_name>`  
   > _creates new branch and switch_  
      _same with:_  
        `git branch <branch_name>`  
        `git checkout <branch_name>`  
      
- `git push -u origin <branch_name>`  
  `git push --set-upstream origin <branch_name>`  
   > _push specific branch to remote_  

- `git checkout --track origin/<branch_name>`  
   > _gets the new remote branch and switches_  
   _in case of error, try:_  
            `git fetch --all`  

- `git branch -d <branch_name>`  
   > _deletes local branch_  
    
 - `git push origin --delete <branch_name>`  
   > _deletes remote branch_  

## tag
- `git tag`  
   > _lists existing tags_  
- `git tag <tag_name>`  
   > _creates a new tag_   
- `git tag -d <tag_name>`  
   > _deletes the tag_  
- `git push origin <tag_name>`  
   > _creates the tag in remote_  

## log
- `git log`  
   > _shows commit history_  
- `git log --oneline`  
   > _shows every commit as one line_   
- `git log -3`  
   > _shows the latest 3 commits_  
- `git log --author="eren"`  
   > _shows the commits by a specific author_  
   _(lists all names including 'eren')_  
- `git log --grep="<message>"`  
   > _shows the commits with a specific message_  

## merge
- `git checkout <receiving_branch>`  
   > _first checkout to receiving branch_  
- `git merge <merging_branch>`  
   > _merging branch's changes will be applied to receiving branch_  
- `git push`  
   > now you can push your changes_     
