---
layout: single
title: 'Why Open Science'
excerpt: "This tutorial walks you through the importance of open science and how to use Jupyter Notebooks for reproducible work."
authors: ['Leah Wasser', 'Martha Morrissey',  'Software Carpentry']
category: [courses]
class-lesson: ['open-science-python']
permalink: /courses/earth-analytics-python/python-open-science-tool-box/why-open-science/
nav-title: "Why Open Science"
dateCreated: 2018-02-08
modified: 2018-02-09
module-title: 'Open Science Python'
module-nav-title: 'Open Science Python'
module-description: 'This module reviews why open science and best practices in python.'
module-type: 'class'
class-order: 3
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

In this lesson you will learn how the importance of open science and how to use Jupyter Notebooks for reproducible work.
<div class='notice--success' markdown="1">

## <i class="fa fa-graduation-cap" aria-hidden="true"></i> Learning Objectives

At the end of this activity, you will be able to:

 * List benefits of using Jupyter Notebooks to create reports. 
 * Explain how Jupyter Notebooks are a useful tool in Open Science approaches. 
 * Explain one way that Jupyter Notebooks can benefit your research. 
 
 
## <i class="fa fa-check-square-o fa-2" aria-hidden="true"></i> What you need
 be sure that you have Python and  the earth analytics python environment installed on your computer.  You should also have an `earth-analytics` directory setup on your computer with a `/data` directory with it
 
 </div>
 
 

## Why Open Science 
Open science in a nutshell is about making scientific methods, data and outcomes
available to everyone. It can be broken down into several parts ([Gezelter 2009)](http://www.openscience.org/blog/?p=269):
* Transparency in experimental methodology, observation, and collection of data.
* Public availability and reusability of scientific data.
* Public accessibility and transparency of scientific communication.
* Using web-based tools to facilitate scientific collaboration.

In this tutorial, you are not going to focus on all aspects of open science as listed above. However, you will be introduce one tool that can be used to make our workflows:
1. More transparent and
2. More available and accessible to the public and our colleagues.

In this tutorial, you will learn how to document your work - by connecting data,
methods and outputs in one or more reports or documents. You will learn about Jupyter Notebooks as a tool to make your work more open and reproducible. Jupyter notebooks allow you to connect data, code (methods used to process the data) and outputs. Jupyter Notebooks can be saved and shared in different formats such as  html or pdf.


### Open Science Slide Show 

Click through the slideshow below to learn more about open science.
<a class="btn btn-info" href="{{ site.baseurl}}/slide-shows/share-publish-archive/" target= "_blank">
View Slideshow: Share, Publish & Archive Code & Data </a>



## About Jupyter Notebooks

The `.ipynb` file format allows you to combine descriptive text, code blocks and code output. You can run the code in python and you can export the .ipynb file to a nicely rendered, shareable format like `.pdf` or html. When render your file to `.html` or pdf the code is run and so your code outputs including plots, and other figures appear in the rendered document. You will use Jupyter Notebooks (.ipynb files) to document workflows and to share data processing, analysis and visualization code & outputs.


### Why Combine Markdown and Code in Jupyter Notebooks

Mixing markdown with code in Jupyter Notebooks provides many advantages:

* Human readable: it's much easier to read a web page or a report containing text and figures.By adding markdown or text around your code, your project becomes more user friendly and easier to understand.
* Simple syntax: markdown is a simple language to learn and can be learned quickly. This makes the learning curve for well-documented Jupyter Notebooks smaller. 
* Helpful Reminder for Your Future Self: When you code, consider your future self. If you leave your future self a well documented set of jupyter notebooks that both run your code and describe the steps, then all components of your work are clearly documented. You and your future self then don't have to remember what steps, assumptions, tests were used to complete the workflow.
* Easy to Modify: You can easily extend or refine analyses contained within a Jupyter notebook by modifying existing or adding new code blocks.
* Flexible export formats: Analysis results stored in Notebooks can be disseminated in various formats including HTML, PDF and slideshows.
* Easy to share: If all of your analysis is contained and described in a one or more notebooks, it makes it easy to share with a colleague. Your colleague can also easily replicate your workflow.


<i fa fa-star></i>**Data Tip:**
You can easily create fully reproducible jupyter notebooks that can be run online using [my binder](https://mybinder.org/). 
{: .notice--success }

### Jupyter Notebooks are beneficial to your colleagues

The link between data, code and results makes Jupyter Notebooks powerful. You can share your entire workflow with your colleagues and they can quickly see your process. You can also write reports using .ipynb files which contain code and data analysis results. To enrich the document, you can add text, just like you would in a word document that describes your workflow, discusses your results and presents your conclusions - along side your analysis results.

### Jupyter Notebooks are beneficial to you & your future self

Jupyter notebooks (.ipynb) as a format is an efficient tool. If you need to make changes to your workflow, you can simply modify the report and re-render the report.This creates an efficient workflow. Your future self will appreciate it too. Jupyter Notebook provides documentation for you to see what code you used to create a figure or to analyze the data.

<i fa fa-star></i>**Data Tip:**
Many of the Earth Lab lessons, including this one, were created using Jupyter Notebooks!
{: .notice--success }


### Use convert .ipynb to .html
You can save Jupyter Notebooks containing code and markdown as .html files. When you save a notebook as .html, it creates a nicely rendered web page with the code and outputs visible along with the markdown rendered as nicely formatted text. You will learn how how to save to .html and other formats later in this course.