# Steps to create, clone, and push your first Github repository

Right off the bat I will define few Github commands to avoid confusion:
`clone`: Means to download or copy an entire repository.
`push`: Send updates/changes to Gihub repository. You need to clone the repository first.
`pull`: Get updates from Github repository

1. Install the latest version of Git in your computer.

2. Create a Github account at github.com and log in.

3. Create a new repository
    - Typical repository naming convention is: this-my-first-repo
    - Make sure to add a README file
    
4. Then, copy the download link.

5. In your computer, open the terminal or GitBash and navigate to the directory in which you would like to download (`clone`) your repository.

6. Write: `git clone <link>` to clone the repository to your computer. Replace `<link>` with the link that you copy in the previous step using `cmd + v` in macs and `ctrl + insert` in Windows machines.

7. Now the repository is in your computer (and of course in Github, we did it in step 3).
> **Important**: To do the following push or pull commands you first need to clone your repository.

8. At this point there is only one file in the repository, the README.md file. `md` files are basically text files with some markup formatting. Github will render Markdown text in this file and display it as the landing page of your repository.
9. As an example, let's try to edit the README file. This statement is tricky because it is unclear whether I'm asking you to edit the README file in your local computer or to do so in Github. Yes, you can edit files in Github (at least text files). Let's edit the README file in your computer.
10. Open the README file in a Jupyter Lab, Jupyter Notebook, or a regular text editor. Add some text to it. Don't worry about adding Markdown format, just add some content.
11. Save the modifications.

12. Now the README file in your computer has modifications that the README file in Github doesn't. Github does not sync automatically (like Dropbox). So, we need to find a way to send the changes to Github.

13. In your computer, use the terminal to navigate inside your repository.

14. Run the following commands in the terminal. Press the `enter` key after writing each command. Enter Github account credentials if needed:
```
git add .
git commit -a -m "Updated README file"
git push
```
> We didn't really add a new file, so the first command is not required here, but it does not hurt to add it (at least in most scenarios when you are getting started).

15. Go to your Github account and refresh the page. Since Github renders the content in the README file as the landing page of your repository, you should be able to see the changes right in front of your eyes. 

16. Follow step 13 and 14 to send future updates yo your Github repository.

17. If in in step 9 you decided to edit the README file directly in Github, then the situation would be the opposite. You would have changes in the README file in your Github account that aren't in your local computer. To get the updates into your local computer, open the terminal and navigate to your repository and type `git pull`. Open the README file with a text editor and you should see the changes you made in the Github website.

18. Sometimes there are files that you don't want to upload to your Github reposity. You just want to have them in your local computer. These files involve sensitive data, heavy files (Github has a max of 100 MB), or temporary files created by applications. A clear example is the .DS_Store file in Macs and the .ipynb folder when using Jupyter Lab or Jupyter Notebooks. So, to prevent Git syncing these files we a list of files that we want Git to ignore. This file is called the `.gitignore` file.  To create a `.gitignore` file open a Jupyter Lab and go to: File -> New -> Text File. Click rename, delete the entire filename (make sure you also delete the .md part), and then name it `.gitignore`. The leading period is important. Make sure that there isn't a trailing `.txt` extension. This means that this is hidden file. The Jupyter Lab navigation panel will not display hidden files. Just search on the web how to make hidden files visible in Windows Explorer or Mac Finder. The `.gitignore` file will appear in both your local directory and your Github repository. 
> Note that if you first add undesirable files to your repository (using git add, commit, and push), adding the .gitignore will not delete them from your Github account. If you are in this situation just insert: `git rm --cached -r .` and then `git add .`

**Example .gitignore file**
Text between square brackets is a comment and you shouldn't write it into your .gitignore file.
```
.DS_Store               
**/.ipynb_checkpoints/  
/Private notebooks
```


