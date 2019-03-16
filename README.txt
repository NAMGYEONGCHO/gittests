Hello!
Some other line

Some empty file..

Hot to create branches:
- git branch branchName

How to switch to a branch:
- git checkout branchName

How to create and change immediately to that branch:
- git checkout -b branchName

How to delete a branch:
- git branch -d branchName

You can't change to another branch before commiting your current changes

How to download an remote branch:
// Im on master and I know there is some "branchName" branch
- git fetch origin branchName
And then:
- git checkout branchName
// Now you are on "branchName" branch
// Now another person pushes more commites on that branch
- git pull origin branchName
// Someone else pushes changes to master and you want to "pull" them
- git pull origin master
// Now you have the branch updated on your local files
// This is not only useful if you are working with someone else
// but also if you are working from differente places

Pull is shortcut/combination for:
git fetch
git merge

master
fixesBranch // lets merge fixesBranch into master

// Now you are on master and you want to merge that branch
git fetch origin fixesBranch
git merge fixesBranch

// or!
git pull origin fixesBranch

// Lets suppose that first you need to check if fixesBranch is ok
// You are on master'lets change to fixesBranch
git checkout fixesBranch
git pull origin fixesBranch
// now you take a look to the new changes, and if everything is fine
// you go back to master to merge the branch
git checkout master && git merge fixesBranch

This is very similar to git pull and git merge:
- git pull origin master
Here git is fetching master from the remote repository and then merging that fetch into your "current master"
Conflicts may (because you are merging files!)

To push your local branch to the repo:
- git push origin branchName

The recommendation is to open a new branch when you want to add a new functionality to your app!
Try this :)

And add some content at the end