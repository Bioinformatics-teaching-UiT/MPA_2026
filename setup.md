# Setting up CobraPy for constraint-based modeling tasks

## Setup GSMM

To run constraint based modeling - or in short COBRA - tasks, there are several toolboxes available. We will make advantage of open source software and python virtual environments. In brief, virtual environments are encapsulated workspaces that allow you to install project specific packages and avoid version conflicts with your regular operating system. Specifically, we will make use of  Miniconda. Miniconda is a conda installer provided by Anaconda and allows us to conveniently install all the data science and modeling packages we need.  
The setup includes the following steps (details below):

1. Install python miniconda (minimal number of packages from Anaconda [https://docs.anaconda.com/](https://docs.anaconda.com/)) on your system
2. Download "cobra_venv_config.yml" to your working directory.
3. Start Jupyter notebook and load the notebook "2603_norge_intro.ipynb" with the introduction to the cobra toolbox 

If not mentioned otherwise, each given command is to be executed on the command-line (*console* or *terminal* in linux/apple, *command prompt*, or *CMD* in Windows).

---

### 1.)

Follow the instructions provided at [https://docs.conda.io/projects/miniconda/en/latest/](https://docs.conda.io/projects/miniconda/en/latest/) for downloading and installing miniconda on your machine.

A helpful **cheat sheet** of common commands can be found here: [https://docs.conda.io/projects/conda/en/4.6.1/user-guide/cheatsheet.html?highlight=cheat%20sheet](https://docs.conda.io/projects/conda/en/4.6.1/user-guide/cheatsheet.html?highlight=cheat%20sheet)

Verify your installation by running e.g. “conda info” in your command line window.

---

### 2.) 

In principle, we will follow the instructions as described here: [https://github.com/opencobra/cobrapy/blob/devel/INSTALL.rst](https://github.com/opencobra/cobrapy/blob/devel/INSTALL.rst).

Download the yml file ''cobra_venv_config.yml'' for the **conda virtual environment** we will be using throughout this course. You may review the packages we use by opening the yml file with a simple text editor (e.g. editor in Windows). More information on the yml file format e.g. on wikipedia: [https://en.wikipedia.org/wiki/YAML](https://en.wikipedia.org/wiki/YAML)

Install and setup cobrapy, the python version of the COBRA toolbox, by running 

```bash
$ conda env create -f cobra_course_config.yml
```
After successful configuration, you can start the virtual environment, e.g. by running

```bash
$ conda activate cobra_course
```

---

### 3.)
Within your active python virtual environment run

```bash
(cobra_course) $ jupyter notebook
```
A jupyter notebook welcome window should open in your internet browser.  
From here on we will be working with jupyter notebooks.  
Within the browser jupyter window, navigate to your working directory of choice for this course.  
Open the introduction jupyter notebook and follow the instructions.

If you are new to jupyter notebooks, a helpful cheat sheet with many useful shortcuts is available here: [https://www.edureka.co/blog/wp-content/uploads/2018/10/Jupyter_Notebook_CheatSheet_Edureka.pdf](https://www.edureka.co/blog/wp-content/uploads/2018/10/Jupyter_Notebook_CheatSheet_Edureka.pdf)
