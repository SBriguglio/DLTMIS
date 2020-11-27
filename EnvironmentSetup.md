# Environment Setup

This document is aimed at users looking to setup their own environment to begin working with deep learning and AI. Though setup may vary between AI applications, for blackbox deep learning applications, I have found a Python environment with Numpy, SciPy, Keras and Jupyter Notebook to be the most ideal for learning, especially for users who are still relatively new to Python. Below, a slightly condensed guide to preparing your own environment is provided. In the future, a guide of how to prepare a GPU accelerated environment will be provided.

## Installing Anaconda and Python 3

If you're new to Python, or a seasoned veteran, Anaconda is a convenient way to manage and use multiple Python environments. This is especially important because packages can sometimes have conflicting dependency requirements. A prime example of this when using TensorFlow 2, which sometimes lags behind the latest official Python release. This guide will begin by setting up a basic deep learning environment which uses Keras and Tensorflow, in addition to other packages like Numpy and scikit-learn.

### Downloading and Installing Anaconda

> With over 20 million users worldwide, the open-source Individual Edition (Distribution) is the easiest way to perform Python/R data science and  machine learning on a single machine. Developed for solo practitioners,  it is the toolkit that equips you to work with thousands of open-source  packages and libraries.

True to their word, Anaconda provides an easy way to manage environments for all your Python data science needs. Begin by selecting the correct installer for your operating system and [downloading Anaconda Individual Edition](https://www.anaconda.com/products/individual) from anaconda.com. Installation is relatively straightfoward using the provided installer's GUI. For detailed installation instructions, visit the Anaconda Documentation's installation instructions:

- Windows: https://docs.anaconda.com/anaconda/install/windows/
- MacOS: https://docs.anaconda.com/anaconda/install/mac-os/
- Linux: https://docs.anaconda.com/anaconda/install/linux/

![](https://github.com/SBriguglio/DLTMIS/blob/main/Images/Screenshot%202020-11-26%20185758.png?raw=true)

<br />

### Creating Your Environment

With Anaconda installed, now we can begin setting up the environment. Open *Anaconda Navigator*. Note that a base environment has already been installed. We'll leave this alone and create our own environment titled *DeepLearning.* You can name the environment anything you'd like, but this is the name that will be refered to throughout this guide. 

You'll notice four tabs on the left hand side of the GUI. The *Home* tab shows all of the installed applications on the currently selected environment. The *Environments* tab contains a list of the Anaconda environments installed on your computer. The third tab, *Learning*, contains links to videos, documentation and other resources to learn about various packages, applications and more. Finally, the *Community* tab contains links to events, forums and other resources. 

We need to create a new environment, so select the *Environments* tab (yellow), and click create (blue). Note that my system contains some environments that I have already created, but you will likely only see the *base (root)* environment.

![](https://raw.githubusercontent.com/SBriguglio/DLTMIS/main/Images/Screenshot%202020-11-26%20191401.png?token=ANH3754EWJEGO7H63HIQVYK7YBCWI)

A popup will appear. Insert *DeepLearning* into the *Name* field and select Python version 3.7 from the dropdown menu. If you plan on using R in your work, you can also select to add this package to your environment as well. Click the green *Create* button and wait for Anaconda to finish creating the new environment.

![](https://raw.githubusercontent.com/SBriguglio/DLTMIS/main/Images/Screenshot%202020-11-26%20192030.png?token=ANH375ZWMBSWNRAFQ473X627YBDKW)

When Anaconda has finished creating your *DeepLearning* environment it should be visible in the *Environments* tab and there should be no blue progress bar present at the bottom of Anaconda Navigator.

![](https://raw.githubusercontent.com/SBriguglio/DLTMIS/main/Images/Screenshot%202020-11-26%20192805.png?token=ANH375YLB6GSV7SRX2HOGZC7YBFEM)

### Adding Applications

With the environment installed, we can now add some useful applications. I recommend installing JupyterLab and Jupyter Notebook in addition to the Conda CLI (for Windows users, you can choose your preference of CMD.exe prompt or the Powershell Prompt). If you're not familiar with [Jupyter Notebooks](https://jupyter.org/), they are a very good way to learn, experiment with, and share Python code. It allows you to run and walkthrough Python code without needing a more robust IDE. To install the applications, simply click the *Install* button below each selection.

![](https://raw.githubusercontent.com/SBriguglio/DLTMIS/main/Images/Screenshot%202020-11-26%20192924.png?token=ANH3757GZS7URN6G4Y7OXZ27YBFE4)

When they are finished installing, the green *Install* button will be replaced with a blue *Launch* button. 

### Adding Packages

There are a few way to add packages to your environment. For those who are comfortable using a CLI, you can simply launch the one you installed from the *Home* tab. From the CLI, packages can be installed using the `conda search [package]` and `conda install [package]` commands. You can read more about using the CLI of Anaconda [here](https://docs.conda.io/projects/conda/en/latest/user-guide/tasks/manage-pkgs.html). With simplicity and ease of use in mind, we will continue using Anaconda Navigator, though the CLI is a more efficient approach that many familiar with working from a terminal will favour.

Select the *Environments* tab and ensure that the *DeepLearning* environment is selected. We need to install some basic packages which we will be using in the future, Numpy, Keras, Pandas, Scikit-learn, and Tensorflow. To do this, search each package using the *Search Packages* search field, select the package and (when all the packages below have been selected) click *Apply*. To check your selections, you can change *Not Installed* to *Selected*. Note that you may need to ensure that *Not Installed* is selected from the dropdown menu instead of *Installed*. Select the following packages before clicking apply:

- numpy
- pandas
- keras
- tensorflow
- scikit-learn
- scikit-image
- opencv

![](https://raw.githubusercontent.com/SBriguglio/DLTMIS/main/Images/Screenshot%202020-11-26%20200703.png?token=ANH3755GZJVJKWWCHG5JNDK7YBIZK)

Wait for Anaconda Navigator to solve package specifications and press *Apply* in the *Install Packages* window which will appear.

Once the packages have finished installing, your environment is setup and ready to go!

#### Command Line Interface Instructions

If you prefer using the command line to install packages, the instructions are much more brief and very easy to do. After launching your Conda CLI from the *Home* tab of the *DeepLearning* environment, use the following command and you'll be ready to go:

`conda install numpy pandas keras tensorflow scikit-learn scikit-image opencv`

### Adding Other Packages

You may need to install more packages at a later time. This can be done in much the same way by using the either the Anaconda Navigator GUI or the Conda CLI with the following:

`conda install [package name]`.

## Updating Environments

### Updating Anaconda

Keeping Anaconda up to date is important and easy to do. This can be quickly accomplished by opening the Conda CLI and using the following command:

`conda update -n base -c defaults conda`

### Updating Packages

Updating pakages can be done most efficiently using the CLI via the following command(s):

To update a single package: `conda update [package name]`

To update all packages: `conda update --all`

Note that the latter command may cause some dependency conflicts in your environment. **It is also suggested to ensure that Anaconda itself is updated to the latest version before using either of these commands**.
