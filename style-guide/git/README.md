# Git 

## General

* Use [Git Flow](http://nvie.com/posts/a-successful-git-branching-model/)
>* master
>* develop
>* feature/
>* release/
>* hotfix/

* Squash multiple commits into a single commit.
* Write a good [commit message](http://tbaggery.com/2008/04/19/a-note-about-git-commit-messages.html).


## Maintain a Repo

* Avoid including files in source control that are specific to your development machine or process.
* Delete local and remote feature branches after merging.
* Perform work in a feature branch.
* Rebase frequently to incorporate upstream changes.
* Use a merge request for code review.

## Write a Feature

Create a local feature branch based off develop

    git checkout develop
    git pull 
    git checkout -b <feature/name>
    
Rebase frequently to incorporate upstreame changes
    
    git fetch origin
    git rebase orgin/develop
    
Resolve conflicts. When feature is complete stage changes.
    
    git add --all
    
When you've staged changes, commit them.
    
    git status
    git commit --verbose
    
Write a [good commit message](http://tbaggery.com/2008/04/19/a-note-about-git-commit-messages.html). Example:

    Present-tense summary under 50 characters
    
    * More information about commit (under 72 characters) 
    * More information about commit (under 72 characters)
     
    #TicketNumber approval
    
If you've created more than one commit, [use `git rebase` interactively](https://help.github.com/articles/about-git-rebase/) to squash them into cohesive commits with good messages:
    
    git rebase -i origin/develop
    
Share your branch 

     git push origin <feature/name>
     
Submit a merge request to the develop branch on Assembla.
     
## Review Code
     
A team member other that the author reviews the merge request. They follow [Code Review](../../code-review) guidelines to avoid miscommunication. 
     
They make comments and ask questions directly on lines of code un the Assembla web interface or in the project's chat room.
     
## Merge
     
Rebase interactively. Squash commits like "Fix whitespace" into one or small number of valuable commit(s). Edit commit message to reveal intent.
    
    git fetch origin
    git rebase -i origin/develop
            
Send a merge request. When merged delete local and remote feature branch.
 
    git push origin --delete <feature/name>
    git branch --delete <feature/name> 
            
     
    