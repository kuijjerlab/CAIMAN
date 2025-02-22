.. _installation:

Installation
============

Environment Setting
-------------------
It is highly recommended to use the `conda <https://docs.conda.io/projects/conda/en/latest/index.html>`_ virtual environment to install this package. After installation of conda, create a virtual environment for PySNAIL using the following command:

.. code-block:: bash

    $ conda create -n pysnail python=3.7.7
    $ conda activate pysnail

Install Package
---------------
Download the source code from :code:`git@github.com:kuijjerlab/PySNAIL.git` and install the package using :code:`pip`:

.. code-block:: bash

    $ git clone git@github.com:kuijjerlab/PySNAIL.git
    $ cd PySNAIL
    $ pip install -e .

To reproduce the analysis we provide in the manuscript:

.. code-block:: bash

    $ git clone git@github.com:kuijjerlab/PySNAIL.git
    $ cd PySNAIL
    $ conda activate pysnail
    $ conda config --add channels anaconda
    $ conda config --add channels defaults
    $ conda config --add channels bioconda
    $ conda config --add channels conda-forge
    $ conda config --add channels bokeh
    $ conda install --file conda_requirement.txt
    $ pip install -r pip_requirement.txt
    $ pip install -e .

Example Dataset
---------------
The PySNAIL packages includes an example dataset for users to test the method on. This can be found under the :code:`sample_data` directories. The `expression.tsv` contains 10,000 randomly selected genes from `the Mouse ENCODE Project Consortium <https://www.encodeproject.org/reference-epigenome-matrix/?type=Experiment&related_series.@type=ReferenceEpigenome&replicates.library.biosample.donor.organism.scientific_name=Mus+musculus>`_. The :code:`groups.tsv` contains the tissue information for each sample.

.. code-block:: bash

    $ sample_data/expression.tsv
    $ sample_data/groups.tsv
