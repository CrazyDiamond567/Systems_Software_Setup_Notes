### Vitali Taranto Notes
#### Repositories

The object that seperates a git project from a normal file directory is called a <b>repository</b>, which is stored in the <b>.git</b>
file in the project itself. The repository contains both <b>commit objects</b> and <b>heads</b>, which are references to 
commit objects.

commit objects are something like snapshots of the project at specific places in time. To save storage space, commits often
have parent commits such that child commits only contain information about a few changes while parent commits contain the whole
snapshot. Thus if I only edit a single file, a whole new parent commit does not need to be created, only a child commit. Every commit
excepts the first has a parent, so that it is something like a timeline of changes.

#### Branches

If the Commits are synonimous to a timeline, a branch is something like an alternate timeline. Say you submitted a peice of code to
your team that breaks the build, but you have made some changes to your code since then that are not yet complete. Essentially,
what you can do is go back to a previous commit that you sent to your team, and create a branch to fix the bug there while 
preserving your current unfinished work.

Ideally, if all team members are working inside branches, then the main branch will always be in a complete state even if 20 different coders 
are all working on new features.

#### Merging

So now you have finished implementing your shiny new feature, and you need to add it to the main branch without breaking everything others have done.
This is easy so long as you have not edited any files that others have edited. If a file changed in your branch, and it changed in the master branch,
then you have what is called a conflict, and you must edit your file with the changes made in the master.

The best way to avoid conflicts is to merge the master into your branch before you make changes.

[Reference](https://www.sbf5.com/~cduan/technical/git/)



