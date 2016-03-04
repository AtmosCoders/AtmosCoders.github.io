---
layout: post
title: First Meeting of PyCAS
---

## Summary

The First Meeting of PyCAS took place today. We discussed the various ways people in CAS are using Python, or intend to use it. There was a range of applications including:

1. Plotting data with matplotlib, data visualisation
1. Raw data processing
1. Processing data in common formats (e.g. netCDF)
1. Machine learning techniques
1. Calculating the properties of organic molecules
1. Harvesting twitter data
1. Auto-tweeting fictional tabloid weather headlines
1. An open source alternative to Matlab

It was good to see so many people interested in learning/using Python!

After the brief introductions, we had an informal Q&A session where we tried between us all to solve some Python problems brought in. This was followed by a discussion of useful resources for learning python.

At the end we had a discussion about the best format for future meetings. It was decided to hold brief discussion sessions at the start of each meeting, where any Python topic could be discussed, and people could show code and results from using python, hopefully to get feedback on how to fix problems.

The second half of meetings would be devoted to a pre-arranged topic a week or so before. Some task or short challenge would be set in advance, and then we would go through the problem together in the second half of the meeting. Matplotlob and netCDF were set as the topics for the next meeting.

We'll meet every two-weeks or so.

## Python Editors/IDE's

You don't need a specific python IDE or Editor (you can just run scripts from the command line/terminal e.g. `python myScript.py`, but having an IDE makes it a whole lot easier. [Spyder](http://pythonhosted.org/spyder/) was mentioned, (and I personally recommend it!).

IDLE is also a very simple Python editor/IDE, and usually comes bundled with a python installation.

## NumPy

As many people are coming to Python from matlab, the subject of NumPy came up. NumPy is an add-on module for the Python language, offering features that involve manipulation of arrays/matrices of data. Obviously, this is common to a lot of what we do in Atmospheric Sciences. 

You might not already have numpy installed on your computer. For Linux users, I would recommend installing it either with your package manager, e.g. `sudo yum install numpy` or, preferably installing it with Python's own package manager, pip, e.g. `sudo pip install numpy`. 

## Matplotlib

Matplotlib is a plotting module that creates nice looking plots. You may also need to install it seperately using your package manager or the pip installer (see above). 

## Installing the whole lot together..

[Anaconda](https://www.continuum.io/downloads) was also mentioned as another alternative for installation. This is a good option if you are using Windows/Mac.

[Python (x,y)](http://python-xy.github.io/) is another great package that includes NumPy, matplotlib etc., as well as the Spyder IDE. 






