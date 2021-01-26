# Installating packages

For this class you will need to install the Anaconda package, Git, and create an account in Github. We will write code using the web browser, so I recommend having Google Chrome installed.

## Anaconda Package

We will use the Anaconda environment, which is a set of curated python packages commonly used in science and engineering. The Anaconda environment is available for free by Continuum Analytics. The latest Anaconda package already has Python 3.7.

### Step 1: Download the Anaconda installer

* If you have a windows machine go to: <https://www.anaconda.com/download/#windows>
* If you have a mac go to: <https://www.anaconda.com/download/#macos>

### Step 2: Install Anaconda

* Double click on the installer and follow the steps. When asked, I highly suggest installing VS Code, which is a powerful editor with autocomplition, debugging capabilities, etc.

* In case you are having trouble, visit the Anaconda "Frequently Asked Questions" for some tips on how to troubleshoot most common issues: <https://docs.anaconda.com/anaconda/user-guide/faq/>

### Step 3: Open Anaconda Navigator

* In Windows go to the start up menu in the bottom left corner of the screen and then click on the Anaconda Navigator.

* In Macs go to Applications and double click on the Anaconda Navigator. Alternatively you can use the search bars (in Mac press Command + Space bar).

* **JupyterLab and Jupyter Notebook**: We will write most of our code using notebooks, which are ideal for reproducible research.

* **VS Code**: A powerful and modern code editor. You can download it and code here if you want.

* **Spyder**: An integrated development environment for scientific coding in Python. It features a graphical user interface similar to that of Matlab.

### Step 4: Update Anoaconda package

* Open Anaconda Navigator
* Click on the arrow next to "base(root)"
* Select "Open terminal"
* Type the following command in the terminal: `conda update --all`
* Wait few seconds and agree to the update by typing "`y`"
* The update process may take several minutes. Sometimes the computer will request your authorization for `python` to make changes in your drive. Agree to the changes in order to proceed.

### Step 5: Install additional libraries

You will also need the Holoviews, Rasterio, and Xarray libraries. All can be installed using with the conda commands: `conda install holoviews`, `conda install xarray`, and  `conda install -c conda-forge rasterio`

The Rasterio library can be tricky to install sometimes, particularly on Windows machines. Try following these steps if the previous approach did not work and you are in Windows machine:

* Open a terminal and check python version using `python --version`
* Make sure you have the latest version of the the pip installer with `pip install --upgrade pip`
* Remove libraries from your pip cache using: `pip cache purge`. This will prevent Python from searching an existing version of the libraries in the next steps (useful in case you've been trying several commands to install Rasterio already).
* Donwload the GDAL library for your Python version from [this website](https://www.lfd.uci.edu/~gohlke/pythonlibs/#gdal). Save the installer in Download or Desktop. For instance, the file `GDAL‑3.1.4‑cp38‑cp38‑win_amd64.whl` would work in a Windows computer of 64-bit with Python 3.8 (note that Rasterio may not need the latest release of this library)
* Donwload the Rasterio library for your Python version from [this website](https://www.lfd.uci.edu/~gohlke/pythonlibs/#rasterio). Save the installer in Download or Desktop. FOr instance the file `rasterio‑1.1.8‑cp38‑cp38‑win_amd64.whl` would work in a Windows computer of 64-bit with Python 3.8. 
* Install GDAL and Rasterio using `pip install GDAL-3.1.4-cp38-cp38-win_amd64.whl` and `pip install rasterio-1.1.8-cp38-cp38-win_amd64.whl`. If there is an error during the installation, read the console to see what GDAL library Python is trying to install with Rasterio. YOu may need to download a different version of GDAL (still with `cp38` for Python 3.8)


## Git

**What is Git?**

* Git is a version control system that tracks changes.

**How do I get started with Git?**

*If you have a mac, you most likely already have Git installed

1. Go to: https://git-scm.com
2. Select Windows/MacOS
3. Follow the installer and use default intallation settings
4. We will most use the command window (called Git Bash), but we need it in order to work with Github.

## Github

**What is Github?**

* Github is a web platform built around Git and has disrupted the software industry.

* In addition to Github there are other similar platforms such as Bitbucket and GitLab, each of them with a different business model.

**How do I get started with Github?**

1. Create a Github account at: https://github.com/
2. Create a repository. Make sure to add a **README** file.
3. Go to your computer and open the terminal
4. Navigate to a directory where you want to place the repository
5. Clone the Github repository using: git clone `<link>`