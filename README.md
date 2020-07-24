# My Quick Git Reference
Learning the ropes !!!

The following have been useful.

### Clone a Git Repo to a Specific tag
    # clone the repo
    $ git clone [repository_to_clone]

    # List and checkout tags
    $ git tag -l
    
    # switch to your chosen tag
    $ git checkout [tag]

Switching to a specific tag only will not save local commits as HEAD will still be at Master. For that you need to create a branch from the tag, eg.
    
    $ git checkout tags/[v1.10] -b [v1.10-new-feature]
    Switched to a new branch 'v1.10-new-feature'

Now HEAD is on the new branch 'v1.10-new-feature'. After working on your custom branch, push changes to your forked repo.
   
    $ git push origin [v1.10-new-feature]

You can then create a pull request to merge changes to master.
    
### View git Log
    
    $ git log --pretty --abbrev-commit
    $ git log --oneline
    
### Sync fork with original repo
First check origin and add upstream
    
    $ git remote -v
    $ git remote add upstream https://github.com/[OriginalOwner]/[OriginalProject].git

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
    

### Add/Update Origin (Similar to adding Upstream)
Add origin
 
    $ git remote add origin https://https://github.com/[gitusername]/[gitrepository].git
 
Update origin

    $ git remote set-url origin https://https://github.com/[gitusername]/[gitrepository].git


### Undo Commits to invert last commit
    $ git revert HEAD


### Sources
Setup Git

http://swcarpentry.github.io/git-novice/02-setup/

https://www.earthdatascience.org/workshops/intro-version-control-git/basic-git-commands/

https://dev.px4.io/master/en/contribute/git_examples.html#contributing_code

Learning markdown

https://guides.github.com/features/mastering-markdown/

Syncing with upstream/master

https://rick.cogley.info/post/update-your-forked-repository-directly-on-github/

Undoing changes

https://www.atlassian.com/git/tutorials/undoing-changes

