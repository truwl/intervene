Introduction
============
InterVene is a tool for intersection and visualization of multiple genomic region sets


Installation
============

Prerequisites
-------------
InterVene requires:

	* Python (>= 2.7 or >= 3.3)
	* pybedtools (>= 1.6.1): https://daler.github.io/pybedtools/
	* R (>= )

If you already have a working installation of Python, the easiest way to install pybedtools and argparser is using pip::

	pip install pybedtools

	pip install argparser

or using conda::

	conda install -c bioconda pybedtools

Read more details about ''pybedtools'' installation: https://daler.github.io/pybedtools/main.html#

If you're setting up Python for the first time, we recommend to install it using Anaconda Python distribution http://continuum.io/downloads. These come with several helpful scientific and data processing libraries. These are available for platforms including Windows, Mac OSX and Linux. 


Install using `pip`
-------------------
You can install InterVene either from PyPi using pip or install it from the source. Please make sure you have already installed the above mentioned python libraries required to run InterVene.

Install from PyPi::

	pip install intervene

Install from `GitHub`
--------------------

1. `git` is installed
2. Cython is installed (`conda install cython` or `pip install cython`)

.. code-block:: bash

    git clone https://github.com/asntech/intervene.git
    cd intervene
    python setup.py install

Install from the source
-----------------------

.. code-block:: bash
	
	wget https://github.com/asntech/intervene/intervene-1.0.tar.gz
	tar -zxvf intervene-1.0.tar.gz
	cd intervene-1.0
	python setup.py install

How to use Intervene
====================
Once you have installed Intervene, you can type:

	intervene --help

to see the help for the three subcommands ``pairwise``, ``venn`` and ``upset`` type::
	
	intervene pairwise --help

	intervene venn --help

	intervene upset --help

Run Intervene on test data
--------------------------

To run Intervene using example data use the following command::

	intervene pairwise --test

	intervene venn --test

	intervene upset --test

This will save the results in the current working directory with a folder named ``Intervene_test``. If you wish to save the results in a specific folder, you can type::

	intervene upset --test --output ~/path/to/your/folder/file_name.pdf

Types of plots
==============
Intervene provides three types of plots to visualize intersections of genomic regions and list sets. These are pairwise heatmap of N genomic region sets, classic Venn diagrams of genomic regions and list sets of up to 6-way and UpSet plots.

Pairwise intersection heatmaps
------------------------------

Venn diagrams upto 6-way
------------------------

UpSet plots
-----------


Support
========
If you have questions, or found any bug in the program, please write to us at ``aziz.khan[at]ncmm.uio.no``

Cite Us
=========
If you use Intervene please cite us: ``Khan A. and Mathelier A., InterVene: a tool for intersection and visualization of multiple genomic region sets``