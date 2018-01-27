# Binder repo for the Jupyter 'Hello World' widget

[![Binder](https://mybinder.org/badge.svg)](https://mybinder.org/v2/gh/PierreMarion23/jupyter-widget-hello-world-binder/master?filepath=hello_world.ipynb)

The notebook is adapted from the official Jupyter [doc](https://ipywidgets.readthedocs.io/en/stable/examples/Widget%20Custom.html), and serves demonstration purposes. 
The Jupyter documentation describes in detail how to build a widget which prints in the output cell the contents of a string set from the back end. In this notebook, we summarize the doc and present the main steps leading to the construction of this widget. We also go a little further and add interactivity in this widget. 

The final version of the widget consists in a form and a title.  Both are synchronized with the Python kernel; the form accepts input, which updates both the title and the backend value.

This repo offers the possibility to test the widget using a [Binder](http://mybinder.readthedocs.io/en/latest/index.html#) image (by clicking on the 'launch binder' button, and waiting a little).

Yet, the way the code is organized is a little messy, since the JS is defined in the middle of the notebook. It would be much cleaner to have the code organized in a JS folder and a Python folder, that could be somehow called from the notebook. [This repo](https://github.com/ocoudray/FirstWidget) does exactly that, and is an example of the same widget, written in a way respecting the current best practices.
