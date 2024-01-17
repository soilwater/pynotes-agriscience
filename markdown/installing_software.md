# Installing packages

To follow the material in this book you will need to install the Anaconda package, Git, and create an account in Github. We will write code using the web browser, so I recommend having Google Chrome installed.

## Anaconda package

We will use the Anaconda environment, which is a set of curated python packages commonly used in science and engineering. The Anaconda environment is available for free by Continuum Analytics.

### Step 1: Download the Anaconda installer

* Download the [Anaconda package for your platform (Windows, Mac, Linux)](https://www.anaconda.com/download)

### Step 2: Install Anaconda

* Double click on the installer and follow the steps. When asked, I highly suggest installing VS Code, which is a powerful editor with autocomplition, debugging capabilities, etc.

* In case you are having trouble, visit the Anaconda "Frequently Asked Questions" for some tips on how to troubleshoot most common issues: <https://docs.anaconda.com/anaconda/user-guide/faq/>

### Step 3: Open the Anaconda Navigator

* In Windows go to the start up menu in the bottom left corner of the screen and then click on the Anaconda Navigator.

* In Macs go to Applications and double click on the Anaconda Navigator. Alternatively you can use the search bar (press `Command + Space bar` and search for terminal).

* **JupyterLab and Jupyter Notebook**: We will write most of our code using notebooks, which are ideal for reproducible research.

* **VS Code**: A powerful and modern code editor. You can download it and code here if you want.

* **Spyder**: An integrated development environment for scientific coding in Python. It features a graphical user interface similar to that of Matlab.


::: {.callout-note}
## Note
If you open a notebook and run the `pip list` command, you can print all the installed packages in your Anaconda environment.
:::


## Git

**What is Git?**

Git is a distributed version control system that enables multiple users to track and manage changes to code and documents

**How do I get started with Git?**

If you have a Mac, you most likely already have Git installed. If you have a Windows machine or need to installed it for your Mac, follow these steps:

1. Go to: https://git-scm.com
2. Select Windows/MacOS
3. Follow the installer and use default intallation settings
4. We will most use the command window (called Git Bash), but we need it in order to work with Github.

## Github

**What is Github?**

* GitHub is a web platform that hosts Git repositories, offering tools for collaboration, code review, and project management. In addition to Github, there are other similar platforms such as Bitbucket and GitLab.

**How do I get started with Github?**

1. Create a Github account at: https://github.com/
2. Create a repository. Make sure to add a **README** file.
3. Go to your computer and open the terminal
4. Navigate to a directory where you want to place the repository
5. Clone the Github repository using: git clone `<link>`

These are just a few short instructions. Check out the detailed and more extensive tutorial to get started.


## Datasets

Most examples and exercises in the book use real datasets, which can be found in the `/datasets` directory of the [Github repository](https://github.com/andres-patrignani/harvestingdatawithpython). You can download the entire reporsitoy, a specific file, or simply read the file using the "Raw" URL link. For example, to read the daily weather dataset for the Kings Creek watershed named `kings_creek_2022_2023_daily.csv` you can run the following command:

`pd.read_csv(https://raw.githubusercontent.com/andres-patrignani/harvestingdatawithpython/main/datasets/kings_creek_2022_2023_daily.csv)`

