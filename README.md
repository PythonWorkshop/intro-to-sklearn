## What's in this tutorial

The material is in jupyter notebook format and using a python 3 kernel.  

The notebooks cover introductory material to ML, ML with sklearn and tips.

Also, included is a brief introductory guide to jupyter notebooks in Notebook_anatomy notebook.

## Installation Notes

### Setting up a development environment

It is generally best practice to have a distinct development environment for various Python projects. There are multiple options available to do this such as virtualenv and Conda. For this project, we will be using the [Conda](https://www.continuum.io/why-anaconda) environment.

To get started, you can install [miniconda3](http://conda.pydata.org/docs/install/quick.html) to get python3 as well as python2.

If you already have Python installed, you can install Conda via `pip`:

```
pip install auxlib conda
```

### Initializing a Conda environment

* To setup a specific development environment for this project, you can run:
  * `conda create --name sklearn python=2`
  * This installs into `C:\Miniconda3\envs\python2\` so I added this to system path (on Windows)
  * On Linux and OS/X, this depends on where the Python Framework is installed. On OS/X using Homebrew, this installs into `/usr/local/Cellar/python/2.7.10_2/Frameworks/Python.framework/Versions/2.7/envs/python2/bin`
  * See [here](http://conda.pydata.org/docs/py2or3.html) for more detailed instructions

* To activate the development environment, from the `bin` folder of your conda environment, run
  * Windows: `activate sklearn`
  * Linux/OSX: `source activate sklearn`

* Ensure ipython/ipython2 is installed in the Python environment
  * Windows: `c:\Miniconda3\envs\python2\Scripts\ipython2.exe kernel install --name python2 --display-name "Python 2"`
  * Linux/OSX: `ipython2 kernel install --name python2 --display-name "Python 2"` (may need `sudo`)

* If, at any point, you desire to exit the development environment, simply type the following:
  * Windows: `deactivate`
  * Linux/OSX: `source deactivate`


###  Installing jupyter notebook locally

The easiest way to install [jupyter notebook](http://jupyter.org/) is via `conda install`
* Run `conda install jupyter` from your terminal. Linux/OSX may require `sudo` permissions.
* Navigate to the directory containing this repository, and execute `jupyter notebook`. <b>This will start a notebook service</b> locally for accessing notebooks in your browser. Drill down on the home page to your notebook of interest.

For a notebook primer go to `Notebook_anatomy.ipynb` on this repo.  The very short story is: to execute a cell just hit <b>Shift-Enter</b>.  There are many more shortcuts in primer.

## Installing python packages

This tutorial requires the following packages:

 * numpy version 1.5 or later: http://www.numpy.org/
 * scipy version 0.10 or later: http://www.scipy.org/
 * pandas http://pandas.pydata.org/
 * matplotlib version 1.3 or later: http://matplotlib.org/
 * scikit-learn version 0.14 or later: http://scikit-learn.org
 * jupyter http://jupyter.readthedocs.org/en/latest/install.html

You can use your development environment of choice, but if you used `conda` as described above, simply run:
```
	$ conda install numpy scipy matplotlib scikit-learn jupyter
```

## Other install options

There are many different ways to install python and the package ecosystem for machine learning.  They are not all going to be covered here, but essentially you have the following choices:

1. anaconda/miniconda aka conda
2. download python and pip install packages
3. use a docker image ([this](https://hub.docker.com/r/wi3o/skflow-jupyternb/) is one for jupyter+sklearn+skflow+tensorflow)
4. [Google cloud platform](https://cloud.google.com/) has a jupyter notebook service called Datalab.  It has tensorflow pre-installed (needed for next tutorial).

Or a combination of the above.

A quick tip if you are installing in a non-conda way with `pip` and are on Windows, many of the data analysis packages are tricky (compiled dependencies) to install.  A nice "unofficial" repository for binaries of packages like `numpy` and a myriad of others was created and maintained by Christoph Gohlke.  This site is [here](http://www.lfd.uci.edu/~gohlke/pythonlibs/).

## What's next

The next tutorial in this workshop is on `tensorflow` and the installation instructions are in this [README](https://github.com/PythonWorkshop/intro-to-tensorflow/blob/master/README.md)

[![Binder](http://mybinder.org/badge.svg)](http://mybinder.org/repo/PythonWorkshop/intro-to-sklearn)
