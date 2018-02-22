---
layout: single
title: 'Setup Git, Bash, and Anaconda on Your Computer'
excerpt: "Learn how to install Git, GitBash (a version of command line Bash) and Python Anaconda distribution on your computer."
authors: ['Leah Wasser', 'Martha Morrissey',  'Software Carpentry']
category: [courses]
class-lesson: ['setup-python-jupyter']
permalink: /courses/earth-analytics-python/setup-your-python-earth-analytics-environment/setup-git-bash-anaconda/
nav-title: "Install Git, Bash & Anaconda"
dateCreated: 2018-02-08
modified: 2018-02-09
module-title: 'Setup Python'
module-nav-title: 'Intro Setup Python'
module-description: 'This module reviews how to set up Python.'
module-type: 'class'
class-order: 1
course: "earth-analytics-python"
week: 1
sidebar:
  nav:
author_profile: false
comments: true
order: 1
topics:
  reproducible-science-and-programming: ['python']
---
{% include toc title="In This Lesson" icon="file-text" %}

In this lesson you will learn how to install Git, GitBash (a version of command line Bash) and Python Anaconda distribution on your computer.

<div class='notice--success' markdown="1">


## <i class="fa fa-graduation-cap" aria-hidden="true"></i> Learning Objectives

At the end of this activity, you will be able to:

* Install Bash

* Open a terminal 

* Install anaconda using the terminal 



## <i class="fa fa-check-square-o fa-2" aria-hidden="true"></i> What you need



Before you start this tutorial, be sure that you have a computer with internet access. 


Information below is adapted from materials developed by [Data Carpentry](https://github.com/swcarpentry/workshop-template) and the [Conda documentation](https://conda.io/docs/user-guide/install/index.html). 


</div>


## Bash Setup 

### Install Bash for Windows

Download the Git for Windows installer.
Run the installer and follow the steps bellow:

1. Click on "Next".
2. Click on "Next".
3. Click on "Next".
4. Click on "Next".
5. Click on "Next".
6. Select "Use Git from the Windows Command Prompt" and click on "Next". If you forgot to do this programs that you need for the workshop will not work properly. If this happens rerun the installer and select the appropriate option.
7. Click on "Next". Keep "Checkout Windows-style, commit Unix-style line endings" selected.
8. Select "Use Windows' default console window" and click on "Next".
9. Click on "Next".
10. Click on "Finish".


This will provide you with both Git and Bash in the Git Bash program.

### Install Bash for Mac OS X
The default shell in all versions of Mac OS X is bash, so no need to install anything. You access bash from the Terminal (found in /Applications/Utilities). You may want to keep Terminal in your dock for this workshop.

### Install Bash for Linux
The default shell is usually Bash, but if your machine is set up differently you can run it by opening a terminal and typing bash. There is no need to install anything.



## Git Setup

Git is a version control system that lets you track who made changes to what when and has options for easily updating a shared or public version of your code on [GitHub](https://github.com/). You will need a [supported](https://help.github.com/articles/supported-browsers/) web browser (current versions of Chrome, Firefox or Safari, or Internet Explorer version 9 or above).

Git installation instructions borrowed and modified from [Software Carpentry](http://software-carpentry.org/).

### Git for Windows
Git should be installed on your computer as part of your Bash install.


### Git on Mac OS X
[Video Tutorial](https://www.youtube.com/watch?v=9LQhwETCdwY)
Install Git on Macs by downloading and running the most recent installer for "mavericks" if you are using OS X 10.9 and higher -or- if using an earlier OS X, choose the most recent "snow leopard" installer, from [this list](http://sourceforge.net/projects/git-osx-installer/files/). After installing Git, there will not be anything in your /Applications folder, as Git is a command line program.


<i class="fa fa-star"></i>**Data Tip:**
If you are running Mac OSX El Capitan, you might encounter errors when trying to use git. Make sure you update XCODE. [Read more - a Stack Overflow Issue](http://stackoverflow.com/questions/32893412/command-line-tools-not-working-os-x-el-capitan).
{: .notice--success }




### Git on Linux
If Git is not already available on your machine you can try to install it via your distro’s package manager. For Debian/Ubuntu run `sudo apt-get install git` and for Fedora run `sudo yum install git`.


## Setup Anaconda 
We will use the Anaconda Python 3.x distribution for this course. Anaconda is a distribution of python that comes with many of the libraries that we need to work with scientific data. Anaconda also comes with Jupyter Notebooks and several other tools that are useful for working in Python.


 
### Windows
1. Download the installer: [Anaconda installer for Windows](https://www.anaconda.com/download/). Be sure to download the python 3.x version!

2. Double-click the .exe file.

3. Follow the instructions on the screen.

4. If you are unsure about any setting, accept the defaults. You can change them later.

5. When installation is finished, from the Start menu, open the Anaconda Prompt.



### Mac
1. Download the installer: [Anaconda installer for macOS](https://www.anaconda.com/download/). Be sure to download the python 3.x version!

2. Install: Anaconda—Double-click the .pkg file.

3. Follow the prompts on the installer screens.

4. If you are unsure about any setting, accept the defaults. You can change them later.

5. To make the changes take effect, close and then re-open your Terminal window.



### Linux
1. Download the installer: [Anaconda installer for Linux](https://www.anaconda.com/download/). Be sure to download the python 3.x version!

2. In your Terminal window, run: `bash Anaconda-latest-Linux-x86_64.sh`

3. Follow the prompts on the installer screens.

4. If you are unsure about any setting, accept the defaults. You can change them later.

5. To make the changes take effect, close and then re-open your Terminal window.
