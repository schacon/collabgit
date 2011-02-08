!SLIDE

# Accepting a Pull Request #


!SLIDE smaller

    The following changes since commit 97679e5bdab5f2494d6f444d995ae79dd4ccb3ca:

     [DoctrineAbstractBundle] added test for new Loader (2011-02-08 04:11:47 +0100)

    are available in the git repository at:
     git://github.com/schacon/symfony.git my_feature

    Scott Chacon (2):
         add contributing link to readme
         updated licence file

    LICENSE |    2 +-
    README  |    5 +++++
    2 files changed, 6 insertions(+), 1 deletions(-)
    
!SLIDE

# Two Options #

!SLIDE

# 1. Add them as a remote #

!SLIDE commandline incremental

    $ git remote add scott git://github.com/schacon/symfony.git

    $ git fetch scott
    From git://github.com/schacon/symfony
     * [new branch]      master     -> scott/master
     * [new branch]      my_feature -> scott/my_feature

    $ git merge scott/my_feature
    Merge made by recursive.
     LICENSE |    2 +-
     README  |    5 +++++
     2 files changed, 6 insertions(+), 1 deletions(-)

!SLIDE

# 2. One-time pull #

!SLIDE commandline incremental

    $ git pull git@github.com:schacon/symfony.git my_feature
    From github.com:schacon/symfony
     * branch            my_feature -> FETCH_HEAD
    Merge made by recursive.
     LICENSE |    2 +-
     README  |    5 +++++
     2 files changed, 6 insertions(+), 1 deletions(-)
     
!SLIDE bullets incremental

# Mailing Lists vs Pull Requests #

* conversations on code
* sending merges
* changing SHAs
* visibility