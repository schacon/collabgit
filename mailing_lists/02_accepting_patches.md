!SLIDE

# Accepting Patches over Email #

!SLIDE bullets incremental

# Accepting Patches over Email #

* extract to files or mbox
* apply patches to branch
* inspect and merge branch

!SLIDE commandline incremental

    $ git am 0001-limit-log-function.patch 
    Applying: add limit to log function
    
    $ git am 0002-seeing-if-this-helps-the-gem.patch 
    Applying: seeing if this helps the gem
    error: patch failed: ticgit.gemspec:1
    error: ticgit.gemspec: patch does not apply
    Patch failed at 0001.
    When you have resolved this problem run "git am --resolved".
    To skip this patch, instead run "git am --skip".
    To restore and stop patching run "git am --abort".
    
    $ (fix the file)
    $ git add ticgit.gemspec 
    $ git am --resolved
    Applying: seeing if this helps the gem