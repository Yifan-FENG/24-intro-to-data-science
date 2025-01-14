### Table of contents
#### [Python installation](#python-installation)
#### [Create and run a virtual environment, and install libraries](#create-venv)
#### [Git setup](#git-setup)
#### [Install libraries](#install-libraries)

### Python installation <a name="python-installation"></a>
1. Check if you have Python installed.<br><br>

2. Depending on your case: <br><br>
    a. If you have Python version 3.11 installed - skip to step 4.<br><br>

    b. If you do not have Python installed - skip to step 3.<br><br>
c. If you have Python installed and it is NOT Python 3.11:** 
   - install pyenv (Mac OS / Ubuntu) or pyenv-win (Windows):
   Mac OS / Ubuntu linK:
   https://github.com/pyenv/pyenv
   Windows link:
   https://github.com/pyenv-win/pyenv-win

   - restart your computer
   - Open the terminal/console/cmd and run:
   ``pyenv --version`` to check if it is installed correctly.<br><br>
   - Install Python 3.11 with pyenv:
      ``pyenv install 3.11``
   - go to the parent folder of your repositories:
   ``cd {MY_FOLDER_NAME}``
   - Set up the local OR global or local version of Python to 3.11
   "Global" will set it up for all folders
   "Local" will set it up for the current folder
   ``pyenv global 3.11`` OR ``pyenv local 3.11``

3. Install Python - version 3.11.
https://www.python.org/downloads/release/python-3119/ <br><br>

4. Check the installation. Open the terminal and run the following:<br>
**Windows:**<br>
   ``where python`` - to ensure Python is installed correctly <br>
   ``where pip`` - to ensure pip is installed correctly. Pip is a command line programme used for managing Python libraries. <br><br>
**Mac OS / Ubuntu:**<br>
   ``which python`` - to ensure Python is installed correctly <br>
   ``which pip`` - to ensure pip is installed correctly. Pip is a command line programme used for managing Python libraries. <br><br>
5. You've successfully installed Python!

### Create and run a virtual environment <a name="create-venv"></a>
#### Virtual environments ensure your library versions and Python versions do not get mixed up between different projects. Sometimes, you may want to use an older library version for compatibility reasons or to not update the whole project after a new library version has been released.

1. Open the terminal and go to a selected folder:<br>
Suggestion: Make a new folder for all coding projects. Set up the virtual environment int here. It's easier to navigate from the console if the folder name does not have spaces or '-'.
``cd path/to/your/directory``<br><br>
2. Make a new virtual environment. Use the ``pyenv`` command if you installed pyenv. Otherwise, use the first version.<br>
``python -m venv daz-venv`` <br> OR  ``pyenv exec python -m venv daz-venv``
**note:** "daz-venv" is the name of the environment. Please note you can change it.<br><br>
4. Run the virtual environment:<br>
**Windows**:<br>
``daz-venv\Scripts\activate.bat``<br><br>
**Mac OS / Ubuntu**: <br>
``source ./daz-venv/bin/activate``<br><br>
**note:** the "-r" option indicates that we're using a requirements file and not listing libraries


### Set up git and GitHub <a name="git-setup"></a>

1. Install git: https://git-scm.com/downloads
2. Set up your account on your machine: https://linuxize.com/post/how-to-configure-git-username-and-email/
3. Set up a GitHub account: https://github.com/
4. Clone the repository: Open VSCode, select 'Clone a repository', and paste the link: https://github.com/peckham-daz/24-intro-to-data-science
5. Create your own repository on GitHub, and clone it to your computer.
6. Make a change and Push to GitHub. VSCode will ask you to log into your GitHub account.

### Install libraries <a name="install-libraries"></a>

1. Install the libraries listed in the ``requirements.txt``file:<br>
``pip install -r ./24-intro-to-data-science/requirements.txt`` - NOTE: this might be a different path if you have a different folder structure!<br>
note: the "-r" option indicates that we're using a requirements file and not listing libraries <br><br>
2. If you ever want to install libraries by listing them in the console. You do NOT need to run this command now, it's a reference for the future :)
``pip install numpy pandas matplotlib``<br>
**note:** "numpy", "pandas" and "matplotlib" are names of Python libraries



