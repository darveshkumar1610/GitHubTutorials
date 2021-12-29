# GitHubTutorials
This respository contains the learning documents for GitHub components.

- **Git** is a tool that tracks the changes over time. 
- Terminology Used: Directory & Change Directory (cd) , Terminal, CLI, Code Editor
- Reporsitory: Project or folder where project is kept
- **GitHub**: Website where we host all of our git repositories. Being online it is easy to work in groups with other people and organize our projects into a portfolio to show potential employers.
- **GitLab** and Team Foundation Server are the tools integrating **project management** and **build pipeline** features.
- For **on-premise setup**, teams can use Git, Subversion, CVS, etc.

## Git and PyCharm Installation
- Download and install git from https://github.com/git-for-windows/git/releases/download/v2.34.1.windows.1/Git-2.34.1-64-bit.exe
- Download and Install PyCharm Community Version from https://www.jetbrains.com/pycharm/download/download-thanks.html?platform=windows&code=PCC

**On Windows Machine.**
```
git --version
git init
git clone https://github.com/darveshkumar1610/Python.git
cd Python
git branch
* main
```

**On PyCharm**

Open the folder in Pycharm. Create a new file in the same folder and save it.
```
git config --global user.email "darveshkumar1610@gmail.com"           # To set your account's default identity.
git config --global user.name "Darvesh"

git status
git add <file(s)>
git commit -m "message"
git branch
git push origin main
```

# Mostly used Git Commands:

- **init**: Initialize empty git repository in any new folder/directory.
- **clone**:Bring a repository into a folder on our local machine from GitHub
- **add**: Track our files and changes in Git
- **commit**: Save our files locally.

-- SSH-Key need to generate & setup for access to git.
  - ssh-keygen -t rsa -b 4096 -C "email@example.com"
  - Copy the content of key.pub to GitHub > Settings > SSH and GPG Keys and use other private key on local machine to access Git repository.

- **push**: Upload Git commits to a remote repo like GitHub
- **pull**: Download changes from remote repo to local machine.

```
git remote add origin <new git-repo>		 # To add new repo as new origin to push/pull
git remote -v								             # To verfiy git push/pull repo.
git push -u origin master					       # To set upstream or default origin as master to avoid using "origin master" again n again.
```

## Steps to use Git
1. Signup on GitHub.
2. Create a Repository (Project)
3. Create a README.md (md - markdown) file (contains text to describe what the project is about, what it does and other relevant informatoin)
4. Commit new file.


#### GitHub Workflow
  Write Code > Commit Changes > Make a Pull request
#### Local Git Workflow 
  Write Code > Stage Changes (git add) > Commit Changes (git commit) > Push Changes (git push) > make a pull request

# Git Branching

- **Master Branch** (main/Default): Commit#1 > Commit#2 > Commit#3
- **Feature Branch** (Pull a branch from main > make changes > Commit & Push > Review and Merge with Main)
- **Hot Fix Branch** (For any Bug Fix > Merge with Main)

```
git branch								                            # To check the current branches. * is the current branch we are working in.
git checkout -b <feature-branch-name>	        # To create new <feature> branch.
git branch								                            # To check the current branches.
git checkout <feature-branch-name>
git push
git push -u origin <feature-branch>
Now anyone can review our code, comment or ask us to make changes

git checkout master						                     # To switch to master branch
git diff <feature-branch-name>			             # To track the changes different in master and feature branch.

git branch -d <branch-name>				               # To delete any unused branch

git add -am <msg>						                       # To add and commit together but for modified files and not for new files

# Merge Conflicts

git merge
git rebase
git pull
git cherry-pick
git stash apply


git reset								                             # To undo the changes 
git reset HEAD~1						                        # To reset the last changes to one commit back

git log

git reset <commit-hash>
git reset --hard <commit-hash> 			# Remove the changes.
  ```

# Fork

To get a copy and make the changes like we want.
