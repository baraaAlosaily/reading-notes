# Git Intorduction :eyeglasses:

All of software developers should learn all aspects about Git because it is the key to publish of works online so be ready to start learn more and more about Git

![get](https://git-scm.com/images/logos/downloads/Git-Icon-1788C.png)

### At the begining we wil take about the benifit of the Git for develper

1. Git allows you to track file revisions, to show a change history.
2. Git enables collaboration between multiple developers on a software project.
3. Git reduces risk of data loss, since files are synchronized with remote repositories

### Local Repository Structure
The local Git repository has three components:

* Working Directory: The actual files reside here.
* Index: The area used for staging
* Head: Points to the most recent commit

![git components](https://cdn.educba.com/academy/wp-content/uploads/2019/03/Introduction-To-GIT.png)

### saving changes
**Tracked** Tracked files can be modified, unmodified, or staged; they were part of the most recent file snapshot.

**Untracked** Untracked files were not in the last snapshot and do not currently reside in the staging area.

***Note*** After cloning a repository, files have tracked status and are unmodified because they have been checked out but not edited.

**Also there is many termial commands that should use to finish your work easily that are:**

1. Get Clone ssh://something.com/[username]/[repository_name].git: Suppose developer needs to create one specific repository of GITHUB in their local copy from the specific remote location. Then they have to execute clone command for copying the same remote repository in the local environment in specific location

2. Git add [file_name.doc]: Used for adding one specific file in staging area.

3. Git commits –m [“message for commit”]: Commit all the required changes.

4. Git push origin [branch_name]: Helps for pushing one of the created branches in your local environment to a remote directory or repository.

And as you see above in the operation the git work following those steps.