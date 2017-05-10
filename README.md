# Git Cheat Sheet
Miscellaneous list (for all intents and purposes) of all the Git commands I've commonly used

## Git update local from master -> Push changes:
*git pull origin master<br>
git status<br>
git add -A<br>
git commit -m "MESSAGE"<br>
git push origin master<br>*

## Git push remote local repo to master:
*git init<br>
git add -A<br>
git commit -m "Initial commit"<br>
git remote add origin project-url<br>
git push -f origin master<br>*

## Git delete local repo:
*git fetch --all<br>
git reset --hard origin/master<br>*

## Git remove file from master:
*git rm classes/file.pyc<br>
git commit -m "bla bla bla"<br>
git push<br>*

## Git Synch Fork:
*git fetch upstream<br>
git checkout master<br>
git merge upstream/master<br>*

## Git upstream vs. Git origin:
#### Git upstream:
(You will use upstream to fetch from the original <br>
repo in order to keep your local copy in sync <br>
with the project you want to contribute to)<br>
*git remote add upstream git link<br>*

#### Git origin:
(You will use origin to pull and push since <br>
you can contribute to your own repo.)<br>
*git remote add origin git link<br>*

## Git Remove directory from git and local:
*git rm -r one-of-the-directories<br>
git commit -m "Remove duplicated directory"<br>
git push origin your-git-branch<br>*

## Switching remote URLs from SSH to HTTPS:
*git remote set-url origin whatever.git<br>*

## Check Current Version of Repository (HEAD):
*git log -1<br>*

## Move File to Directory in Local Repo:
*mkdir dir_name<br>
git mv hello.html dir_name<br>
git status<br>*
