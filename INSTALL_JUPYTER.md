##  Installing jupyter

1. Install miniconda3 - http://conda.pydata.org/miniconda.html
  a. This will install python 3.5
  * recommended to install 32-bit
  * Gets added to path, but not registered as default (Windows)
* Conda install jupyter
  a. `conda install jupyter`
* To install python 2.7
  a. `conda create --name python2 python=2`
  * This installs into C:\Miniconda3\envs\python2\ so I added this to system path (Windows)
* Add python2.7 to kernelspec
  a. `activate python2`
  * ensure ipython2 is installed in python2 env
  * `c:\Miniconda3\envs\python2\Scripts\ipython2.exe kernel install --name python2 --display-name "Python 2"`
  * on cmd line: `deactivate` (to get out of python 2 env)
* on cmd line: `jupyter notebook`

