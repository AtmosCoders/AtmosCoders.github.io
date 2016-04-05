---
layout: post
title: Second Meeting of PyCAS
---

In the first half of the meeting we discussed some questions about the best way of getting Python installed on your machine (or more specifically, NumPy, Matplotlib and other various Python modules for doing science with.)

To clarify, the main ways of installing Python packages for sciency things are:

- Install them with your package manager (Linux Users), i.e. `sudo apt-get numpy` or `yum install numpy-python` etc. You'll have to search your repository or google to find what the actually name of the relevant package is as they often vary slightly between linux distributions.

- Install with Python's own package manager, *pip*, i.e. `sudo pip install numpy`. Works on multiple platforms (Mac, Linux, Windows (I think..)

- Install a Python 'bundle' designed for science/data analysis. These are big packages that you can download and install, which include pretty much everything you need to do Python with, namely NumPy and Matplotlib, but also a whole range of other modules that might come in handy. This takes the most space on your PC, but is often the easiest way. Works on Windows/Linux/Mac. 

## Python Bundles

### Anaconda
Anaconda is a popular Python 'bundle' that includes most things you could possibly want to do Python-Science stuff with. You can download the appropriate installer here: [Anaconda Download](https://www.continuum.io/downloads). Linux, Mac, and Windows version available.

### Python(x,y)
Personally, this is my favourite Python bundle for Windows, it comes with a nice MATLAB-like user interface called Spyder, which we mentioned at the last meeting. [Here is Python(x,y)](http://python-xy.github.io/).

## From the Package manager
This is a good way to go if you don't want to install a massive bundle of Python stuff that you won't use, and like to know what's being installed on your computer. This method is just for linux users. 

NOTE: If you are running Python versions 2.7 and 3.x side by side, you may find that you have to install packages for both installations separately with your package manager: e.g

```
sudo yum install numpy-python
sudo yum install numpy-python3
```
in order to get NumPy available on both installations.

## Python 2 or 3?
This question comes up a lot. I don't think it really matters to be honest. For reasons I won't get into too much detail here, there are two versions of Python, Python 2.7 and Python 3.x (where x is an increasing number every few months). The reason Python 2.7 remains in use is that Python 3 introduced several features that made old programs non-backwards-compatible, and so it is still commonly found installed by default on some operating systems, instead of Python 3, which you have to _upgrade_ to. 
You can run them side by side if you wish. I won't explain how to do it here, but google will help you :). Typically, if you have both Pythons installed, you have to specify one or the other when you run a script or start a Python console. e.g.

```
python myPython2script.py
python3 myPython3script.py

IPython  # starts the default version of python (often 2.7)
IPython3  # starts a Python 3 session
```

Note that it varies which python is the default one. You can find out by typing `python --version` into the console/terminal.

### Any differences?

Not very many that we would probably worry about. Python 2.7 does integer division by default where it can. e.g.

#### Python 2.7
{% highlight python %}
x = 10
y = 3
print x/y

>> 3
{% endhighlight %}

This may not be the answer you were expecting, but you can provide some 'encouragement' to Python 2 to get what you want e.g.

{% highlight python %}
x = 10.0
y = 3
print x/y

>> 3.33333333335
{% endhighlight %}

This time, it spots that one of your variables is not an integer, so converts both of them to floating point numbers to do the arithmetic. However, *Python 3* will always opt for what some might call the "expected" answer e.g.

#### Python 3.x
{% highlight python %}
x = 10
y = 3
print( x/y )

>> 3.3333333333335
{% endhighlight %}

The example shows the other main difference between the two. In Python 2.7 `print` is a statement, whereas in 3 it is a function (with brackets around the thing you want to print).

## NetCDF

We discussed the NetCDF task, [suggested answers and tips are now on the original page](https://nbviewer.jupyter.org/github/AtmosCoders/PyCAS/blob/gh-pages/netCDF_example1.ipynb) with the exercise.
