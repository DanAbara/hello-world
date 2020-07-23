# hello-world
Learning the ropes !!!

Curiously seeking the truth, coding when I can, dancing whether or not I need to. 

Absolute madness.

The following have been helful

### Clone a Git Repo to a Specific tag
    # clone the repo
    $ git clone [repository_to_clone]

    # List and checkout tags
    $ git -l
    
    # switch head to your chosen tag
    $ git checkout [tag]

### View git Log
View entire log

    $ git log

View short log
    
    $ git log --oneline


### Undo Commits to invert last commit
    $ git revert HEAD


### Sync fork with original repo
First check origin and upstream
    
    $ git remove -v

Fetch from upstream
    
    $ git fetch upstream

Checkout your fork's master and then merge changes from upstream into it

    $ git checkout master
    $ git merge upstream/master
    
Add and commit new changes
    
    $ git add
    $ git commit -m "[commit message]

Push changes to your fork

    $ git push origin master
    

### Sources
Setup Git

http://swcarpentry.github.io/git-novice/02-setup/

https://www.earthdatascience.org/workshops/intro-version-control-git/basic-git-commands/

Learning markdown

https://guides.github.com/features/mastering-markdown/

Syncing with upstream/master

https://rick.cogley.info/post/update-your-forked-repository-directly-on-github/

Undoing changes

https://www.atlassian.com/git/tutorials/undoing-changes

Hoorah!!
