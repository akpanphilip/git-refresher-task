#initialises git repo
git init

#add a file/files to staging ready for commit
git add filename | .

#commit file to staging
git commit -m "message"

#commit and update file content. git add + git commit
git commit -am "message"

#shows untracked files
git status 

#see commits made
git log --oneline

#retore to last commit
git restore filename

#remove files from staging area but keeps your actual edits
#example --- git add file.txt git restore --stage file.txt
git restore --staged filename

#creates a new commit that reverses previous commit
git revert 

#returns to last commit
git reset --hard Head~1

#switch to another branch
git switch branchname

#switch and create a new branch
git switch -c branchname

#branch to main
git branch -M main

#add remote origin
git add remote origin path

#push to remote origin main
git push -u origin main