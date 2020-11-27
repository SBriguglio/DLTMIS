# Environment Setup

This document is aimed at users setup their own environment to begin working with deep learning and AI. Though setup may vary between AI application, for blackbox deep learning applications, I have found a Python environment with Numpy, SciPy, Keras and Jupyter Notebook to be the most ideal for learning, especially for users who are still relatively new to Python. Below, a slightly condensed guide to preparing your own environment is provided. In the future, a guide of how to prepare a GPU accelerated environment will be provided.

## Installing Anaconda and Python 3

If you're new to Python, or a season veteran, Anaconda is a convenient way to manage and use between multiple Python environments. This is especially important because libraries and APIs can sometimes have conflicting dependency requirements. A prime example of this when using TensorFlow 2, which sometimes lags behind the latest official Python release. We will begin this guide by setting up a basic deep learning library which uses Keras and Tensorflow, in addition to other frameworks and libraries like Numpy and scikit-learn.

### Downloading and Installing Anaconda

> With over 20 million users worldwide, the open-source Individual Edition (Distribution) is the easiest way to perform Python/R data science and  machine learning on a single machine. Developed for solo practitioners,  it is the toolkit that equips you to work with thousands of open-source  packages and libraries.

True to their word, Anaconda provides an easy way to manage environments for all your Python data science needs. Begin by selecting the correct installer for your operating system and [downloading Anaconda Individual Edition](https://www.anaconda.com/products/individual) from anaconda.com. Installation is relatively straightfoward using the provided installer's GUI. For detailed installation instructions, visit the Anaconda Documentation's installation instructions:

- Windows: https://docs.anaconda.com/anaconda/install/windows/
- MacOS: https://docs.anaconda.com/anaconda/install/mac-os/
- Linux: https://docs.anaconda.com/anaconda/install/linux/

![](https://raw.githubusercontent.com/SBriguglio/DLTMIS/main/Images/Screenshot%202020-11-26%20185758.png?token=ANH3756UCKW7O2P34UXM35K7YBA3E)

<br />

### Setting Up Your Environment

With Anaconda installed, now we can begin setting up the environment. Note that a base environment has already been installed. We'll leave this alone and create our own titled *Deep Learning.* You can name the environment anything you'd like, but this is name that will be refered to throughout this guide. 

You'll notice four tabs of the left hand side of the GUI. The *Home* tab shows all of the installed applications on the currently selected environment. The *Environments* tab contains a list of the Anaconda environments installed on your computer. The third tab, *Learning* contains links to videos, documentation and other resources to learn about various libraries and more. Finally, the *Community* tab contains links to events, forums and more. 

We need to create a new environment, so select the *Environments* tab (yellow), and click create (blue). Note that my system contains some environments that I have already created, but you will likely only see *base (root)*.

![](https://raw.githubusercontent.com/SBriguglio/DLTMIS/main/Images/Screenshot%202020-11-26%20191401.png?token=ANH3754EWJEGO7H63HIQVYK7YBCWI)



