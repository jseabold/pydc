# Statsmodels talk for Statistical Programming DC Meetup
## April 8, 2014

To run offline
--------------

You'll need to make sure that the first two code cells in the Notebook run for you without problems. They are listed below.

Run this from the Notebook or in (I)Python from this directory or after fixing the paths below. 

    from IPython.external.mathjax import install_mathjax
    install_mathjax("./MathJax-2.2.tar.gz")

And

    import statsmodels.api as sm

    _ = sm.datasets.get_rdataset("Guerry", "HistData", cache=".cache")
    _ = sm.datasets.get_rdataset("Duncan", "car", cache=".cache")


Requirements
------------

* [IPython 2.0](http://ipython.org/) with [notebook dependencies](http://ipython.org/install.html)
* [Statsmodels](http://statsmodels.sourceforge.net/)
  * This notebook was written using statsmodels master branch on github as of April 8, 2014. If you cannot install master, the last release should be fine, but some parts of the notebook will not work.

Necessary Statsmodels Dependencies: 

* [NumPy](http://numpy.org)
* [SciPy](http://scipy.org)
* [Pandas](http://pandas.pydata.org)
* [Patsy](http://patsy.readthedocs.org/en/latest/)
* [Matplotlib](http://matplotlib.org)
