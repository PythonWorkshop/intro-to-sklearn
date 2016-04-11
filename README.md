## What's in this tutorial

The material is in jupyter notebook format and using a python 3 kernel.  

The notebooks cover introductory material to ML, ML with sklearn and tips.  The big module is Intro_ML_sklearn.  This module is broken down into submodules.

Also, included is a brief introductory guide to jupyter notebooks in Notebook_anatomy.

## Installation Notes

###  Installing jupyter notebook locally

#### This is the easiest way (conda install):

> Note:  Install miniconda3 to get python3 (python2 may be installed as well, see below) - http://conda.pydata.org/miniconda.html
  * This will install the latest python
  * recommended to install 32-bit
  * Gets added to path, but not registered as default (on Windows)

1. Conda install jupyter (in command terminal)
  * `conda install jupyter` (may need `sudo` for unix or OS X)
* To install python 2.7
  * `conda create --name python2 python=2`
  * This installs into C:\Miniconda3\envs\python2\ so I added this to system path (on Windows)
  * See [here](http://conda.pydata.org/docs/py2or3.html) for more detailed instructions
* Add python2.7 to kernelspec for jupyter
  *  Get into python 2 environment
    * Windows: `activate python2`
    * Linux/OSX: `source activate python2`
  * ensure ipython/ipython2 is installed in python2 env (do `pip install ipython ipykernel`)
	  * Windows: `c:\Miniconda3\envs\python2\Scripts\ipython2.exe kernel install --name python2 --display-name "Python 2"`
	  * Linux/OSX: `ipython2 kernel install --name python2 --display-name "Python 2"` (may need `sudo`)
  * on cmd line: `deactivate` (to get out of python 2 env)
* `jupyter notebook` will start a notebook service for accessing notebooks in your browser (wherever you run this, it will be the base directory for the notebook service)

## Installing python packages

This tutorial requires the following packages:

 * numpy version 1.5 or later: http://www.numpy.org/
 * scipy version 0.10 or later: http://www.scipy.org/
 * matplotlib version 1.3 or later: http://matplotlib.org/
 * scikit-learn version 0.14 or later: http://scikit-learn.org
 * jupyter http://jupyter.readthedocs.org/en/latest/install.html

The easiest way to get these is to use the [conda] (https://www.continuum.io/why-anaconda) environment manager. We suggest downloading and installing [miniconda] (http://conda.pydata.org/miniconda.html) (see above). Once this is installed, the following command will install all required packages in your Python environment:
	
	$ conda install numpy scipy matplotlib scikit-learn jupyter

