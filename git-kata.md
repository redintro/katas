### Git Kata

### Initial Commit

- Create a practice project directory: mkdir myproject

- Move to that directory: cd myproject

- Create a file: cat > myfile

- Add some content: This is some file content

- Save content: CTRL + D

- Exit file: CTRL + C

- Initialise git: git init

- Add all to git: git add .

- Check status of local repository: git status

- Commit file to git: git commit -m "Initial commit"

- Check status of local repository: git status

### Edit 

- Open file in Vim: vim myfile

- Add new line and enter insert mode: o

- Add additional content: This is some additional file content

- Save and exit Vim: ESC :wq ENTER

- Check status of local repository: git status

- Stage file: git add myfile

- Check status of local repository: git status

- Unstage file: git rm --cached myfile

- Check status of local repository: git status

- Stage file: git add myfile

- Commit file: git commit -m "Added additional content"

### Diffs 

- Open file in Vim: vim myfile

- Add new line and enter insert mode: o

- Add additional content: This is some more additional file content

- Save and exit Vim: ESC :wq ENTER

- Stage file: git add myfile

- View the difference between staged changes and the repository: git diff --staged

- Open file in Vim: vim myfile

- Add new line and enter insert mode: o

- Add additional content: This is even more additional file content

- Save and exit Vim: ESC :wq ENTER

- View the difference between the current working tree and the staging area: git diff

- View the difference between the current working tree and the repository: git diff HEAD

- View git log: git log

- View the difference between the current working tree and a commit in the repository: git diff commit-id

- View difference between two commits (commit ID, branch name or tag to reference commit): git diff commit-id-1 commit-id-2

- View last N commits: git log -2

- View changes made by last commit: git log -1 -p HEAD 

### Branch

- Create a new branch and switch to it: git checkout -b development

- View branches: git branch

- Open file in Vim: vim myfile

- Add new line and enter insert mode: o

- Add additional content: This is some additional file content from the development branch

- Save and exit Vim: ESC :wq ENTER

- Stage file: git add myfile

- Commit file: git commit -m "Added additional content from development branch"

- Compare branches: git diff master..development

### Merge

- Check out master branch: git checkout master

- Merge content from development: git merge development 

- Delete development branch: git branch -d development

- View branches: git branch

### Finish

- Switch to parent directory: cd ..

- Delete the practice project directory: rm -Rf myproject

- Finish
