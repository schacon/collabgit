!SLIDE

# Merge vs Rebase #

!SLIDE bullets incremental

# Advantages of Merging #

* can undo the merge
* more data for analysis later
* easy continuous re-integration

!SLIDE bullets incremental

# Advantages of Rebasing #

* it's prettier

!SLIDE code

# git pull --rebase #

!SLIDE code

# git fetch origin #

# git rebase origin/master #

!SLIDE

# Otherwise, merge #

!SLIDE code

# git merge --no-ff #

!SLIDE commandline incremental

    $ (code code code)
    $ git fetch
    $ git log origin/master ^master
    $ git [merge|rebase] origin/master
    $ (test)
    $ git push origin master

!SLIDE bullets incremental

# Possible Team Rules #

* always --no-ff merge topic branches into master
* always rebase work onto master




