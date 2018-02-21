---
layout: single
title: 'Set up Conda Envrionment'
excerpt: 'This tutorial walks you through installing a conda environment designed for this class.'
authors: ['Leah Wasser', 'Martha Morrissey',  'Data Carpentry']
modified: 2018-02-15
category: [courses]
class-lesson: ['setup-python-jupyter']
permalink: /courses/earth-analytics-python/get-started-with-python-jupyter/setup-conda-earth-analytics-environment/
nav-title: 'Set up Conda'
week: 1
sidebar:
    nav:
author_profile: false
comments: true
order: 3
course: "earth-analytics-python"
topics:
    reproducible-science-and-programming: ['python']
---
{% include toc title="In This Lesson" icon="file-text" %}

In this lesson you will learn how to install a conda environment designed specifically for this class called earth-analytics-python from a yaml file

<div class='notice--success' markdown="1">


## <i class="fa fa-graduation-cap" aria-hidden="true"></i> Learning Objectives

At the end of this activity, you will be able to:

* install anaconda
* install a new environment 
* view the available environments 



## <i class="fa fa-check-square-o fa-2" aria-hidden="true"></i> What you need


You should have Shell and the Anaconda distribution of python 3.x setup on your computer and an Earth Analytics working directory. Use the lessons below to help you get setup:

* Completed the setup shell and conda lesson
* Have an Earth Analytics Directory on your computer 


</div>


Information below is adapted from materials developed by the Conda documentation for [installing conda](https://conda.io/docs/user-guide/install/index.html) and [managing packages](https://conda.io/docs/user-guide/tasks/manage-pkgs.html). 


## Set up A Conda Python Environment 

### Install the Earth Lab Conda Environment

Anaconda allows you to have different environments installed on your computer to access different versions of python and different libraries. Sometimes libraries conflict which causes errors and packages not to work. To avoid conflicts, we created an environment specifically for this earth analytics course that contains all of the spatial libraries that you will need.

<i fa fa-star></i>**Data Tip:**
For more information about conda environments check out the [conda documentation](https://conda.io/docs/user-guide/tasks/index.html).  
{: .notice--success }

To install the earth lab environment you will be working in the terminal. 


### Where to Install Python Libraries From

There are many different python repositories that house  libraries like geopandas. To access each repository, you use a command at the terminal.
* pip install installs libraries using pip from a pip specific repo
* Conda install installs libraries using the conda repo


For this class, most python libraries will be installed with `conda-forge` to reduce the potential of installation conflicts.

### About the Conda Environment

Let’s take a minute to explore the Conda python environment! Notice at the top of the file there is the environment name. This file has a few key parts: 

1. NAME: the name of the environment that you will call when you wish to activate the environment. The name earth-analytics-python is defined in the environment.yml file.

2. Channels: this lists where packages will be installed from. There are many options including conda, conda-forge and pip. You will be predominately using conda-forge for all of the earth-analytics courses. 

3. Dependencies: Dependencies are all of the things that you need installed in order for the environment to be complete. In the example, python version 3.6 is specified because this is because it works best with gdal. The order in which the libraries should be installed is also specified. 


### Use a Pre-configured Installation Script
When you work with Anaconda, you can create custom lists that tell anaconda where to install libraries from, and in what order. You can even specify a particular version. You write this list using [yaml](http://yaml.org/) (Yet Another Markup Language).  

There is a custom yaml list that you can use to  install all of the python libraries that you will need to complete the lessons in this course. This yaml list is customized to install libraries from the repositories and in an order that minimizes conflicts. If you run into any issues installing the environment from the yaml leave a comment at the bottom of the page. 

### Here’s what part of the yaml file looks like:

```
name: earth-analytics-python
channels:
  - conda-forge
dependencies:
  # Core scientific python libraries
  - numpy
  - matplotlib
  - python=3.6
  - pyqt
  - seaborn

  # spatial libraries
  - rasterstats
  - geopy
  - cartopy
  - geopandas
  
```

Follow these steps below to get your environment ready.
An environment for conda has been created specifically for this course. To load this:

1. Download the custom yaml list from <link>/download button
2. Move this file into your earth-analytics directory 
3. Open your favorite bash envt. This may cygwin or gitbash on windows or terminal on a mac. 
4. Navigate to your earth-analytics directory on your computer. (remember the cd command in terminal means change directory) 
5. conda env create -f environment.yml

Note that it takes a bit of time to run this setup as it needs to download and install each library
IMPORTANT: you need to have internet access for this to run! 

<i fa fa-star></i>**Data Tip:**
The instructions above will only work if you run them in the directory where you placed the environment.yml file
{: .notice--success }


## Manage Your Conda Environment

You can have different python environments on your computer. Anaconda allows you to easily jump between environments using a set of commands that you run in your terminal. To manage your conda environments, use the following commands:


### View a list of all installed environments

```bash

conda info --envs

```

### Activate the environment that you'd like to use
If you want to jupyter notebooks to use a particular environment that you have setup on your computer, you need to activate it. For example if you geopandas is only installed in the earth-analytics-python environment, and not the default anaconda environment, you will not be able to load it in jupyter unless you have the earth-analytics-python environment activated.

To active an environment, first navigate to your earth-analytics working directory.  Then use the following code at the command line to activate the environment that you want. In this case you will want to activate the earth-analytics-python environment:

```
source activate earth-analytics-python

```


### Deactivate the environment 

```
Source deactivate earth-analytics-python

```

Deactivating the environment switches you back to the default environment in your computer. 
Before doing work for this class always make sure that the earth analytics-python environment is activated. The name of the activate environment will appear in parentheses on the left side of your terminal. 



<i fa fa-star></i>**Data Tip:**
Notice how after you restart the terminal, the Earth Analytics environment is no longer active. 
Activate the earth-analytics-python environment by running:

```

source activate earth-analytics-python

```
{: .notice--success }



