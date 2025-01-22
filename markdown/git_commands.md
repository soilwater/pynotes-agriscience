# Useful Git commands

Some of the most widely used git terminal commands. You can run the commands below anywhere, you don't need to be inside any specific directory or repository. Some of these commands will change information in Git's configuration file, so that you don't have to re-type your username and email everytime you make a commit.

`git config --global user.name "john-doe"` In this case my username is: john-doe. The dash in the middle is part of the username.

`git config --global user.email johndoe@abc.org` In this case see that I did not include the email between quotation marks as I did with the username.

`git config --global core.editor "nano"` changes the default editor from "vim" to "nano". In my opinion **nano** is a bit more friendly for beginners. Exit nano by pressing `ctrl + X`

`.gitignore` contains file and folder names that you don't want to keep track of version control. In other words, they will not sync with Github. If you added a rule in the .gitignore file after the file or folder has been added to your Github, you will need to erase the cache of the repository and then add the files again, so that changes take effect. You can do this following these commands: `git rm --cached -r .` and then `git add .`

`git clone <repository link>`: Clone repository into your local computer or a remote server. You only clone your repository once. If you work on a server or supercomputer, cloning a repository from a cloud-based platform like Github is much easier than transferring files using the terminal or copy pasting files using a graphical user interface like FileZilla. 

`git status`: This command provides the state of the current repository in the local computer (or server) relative to Github's remote repository.

`git add .`: Adds and removes **all** new file additions/deletions from repository. Remember, when you add or remove a new file to a folder in your local computer, it does not get automatically added to your repository. You have to execute the command for this to happen.

`git add <filename>` In case you want to add a single file to your repository. `<filename>` could be `mytextfile.txt`

`git commit -a -m "<write here a short descriptive message>"`: Send changes to remote repository. **Messages are mandatory** and should be short and descriptive. Don't accumulate too many changes before committing, otherwise your message/comment will not be meaningful to all the changes you made.

`git push origin master` Upload changes to master branch in the Github repository. To see changes make sure you refresh the Github webpage.

`git pull origin master`: Downloads updates in the master branch.

`git checkout -- .`: Disregard changes.

`git checkout <branch name>`: Changes scope to any branch, including the master branch. This command assumes that you have a branch.