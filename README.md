# git-github
Git & Github

git config
This is the command used to get or set configuration variables in Git.
--global
This flag indicates that the configuration should be applied globally, affecting all Git repositories on your machine.
user.name
This is the configuration key for setting the user's name.
“GitHub UserName”
This is the value you are setting for the user name. Replace "GitHub UserName" with your actual GitHub username or the name you want to associate with your Git commits.



git config --global user.name



This will display the currently configured user name in the terminal.
user.email
This is the configuration key for setting the user's email address.
"your_email@example.com"
Replace this with your actual email address. This email address will be associated with your commits as the author's email.



git config --global user.email
This will display the currently configured user email in the terminal.
git config --list
The command is used to display the configuration settings for Git.It shows a list of all the configuration settings, including those at the system, global, and local levels
git init
The command is used to initialize a new Git repository. Run this command in a directory, Git creates a new repository, which is a hidden subfolder. 
git add filename


Add specific file(s) to the staging area.
git add .


Add all changes in the working directory to the staging area.
git add -i


ls -lart
Show hidden folders  in the command line.
git commit -m "message"



The command is used to create a new commit in your Git repository with a commit message. The commit message is a brief description of the changes you are committing.
git config --global core.editor <editor-name>


git status
The command is used to show the status of changes as untracked, modified, or staged in your Git working directory.
git log
View git commit history. 
git log -p
Git log -p -1








git diff
Compare Changes in the Working Directory.
git diff -- staged
Compare Changes in the Staging Area.
git diff ‘comit_has1’ ‘comit_has2’
Compare Changes Between Two Commits.
git diff filename 
Compare Changes in a Specific File.
git diff branch1..branch2
Compare Changes Across Branches.
git difftool
Compare Changes With External Tools.
git reset
Unstage Changes. This command unstaged changes that have been added to the staging area but not yet committed. It does not discard changes in your working directory.
git reset filename
Unstage a Specific File.
git reset --hard
Discard Changes in Working Directory and Unstage.
git reset <commit>
Move HEAD to a Previous Commit.Changes from the specific commit onward are unstaged, but the changes are kept in the working directory.
git reset --soft <commit>
Move HEAD and Unstage Changes.
Changes from the specific commit onward are staged.
git reset --soft HEAD^
Undo the Last Commit (Soft Reset). This undoes the last commit, keeping the changes in the working directory and staging area.
git reset --hard HEAD^
Undo the Last Commit and Discard Changes (Hard Reset). This undoes the last commit and discards the changes in both the working directory and staging area.
git rm 
The command is used to remove a file from both the working directory and the Git repository.
git rm filename
The file is removed not only from your working directory but also from the version history in the Git repository.
After using ‘git rm’ you need to commit the changes to make the removal permanent:
git commit -m”remove filename”


git rm --cached filename
Untrack a file from Git without deleting it from your working directory. 
git commit -m”stop tracking filename”


git rm -f filename
Force Removal.
git rm -r directory_name
Remove a Directory.
git rm *.log
Remove Files Matching a Pattern.
git mv old_filename new_filename 
Rename or Move Files.
git branch
Show git branches. 
git branch branchname
Create a new branch.
git checkout branch_ename
Switch to a different branch.
git checkout -b newbranch_ename
Single command to create and switch to a new branch.
git branch -m oldbranch_name newbranch_name
Rename a Branch.
git branch -d branchNam
Delete a Branch.
git branch -r
List Remote Branches.
git branch -a
List All Branches (Local and Remote).
git merge
The command in Git is used to combine changes from one branch into another.
git merge feature_branch
Merge a branch into the current branch.
git remote
List Remote Repositories.
git remote -v
Show Detailed Information about Remotes.
git remote add remoteName url
Add a New Remote.
git remote rename oldrmt newrmt
Rename a Remote.
git remote rm remotNam
Remove a Remote.
git push remoteNam branchNam
Pushing Changes to a Remote Branch.
git push --force remoteNam branchNam
This forcefully pushes changes, overwriting the remote branch with your local branch. Use with caution, as it rewrites the commit history.
git push remoteNam --delete branchNam
Deleting a Remote Branch.
git clone url
Clone a remote repository.
git pull
Git pull combines the git fetch and git merge operations
git pull rmtNm brcNam
Pulling Changes from a Specific Branch.
Git pull --all
Updating All Branches.
git fetch 
The command in Git is used to retrieve changes from a remote repository without automatically merging them into your working directory.




