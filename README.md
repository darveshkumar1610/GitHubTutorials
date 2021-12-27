# GitHubTutorials
This respository contains the learning documents for GitHub components.

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
