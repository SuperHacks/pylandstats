PyLandStats documentation!
======================================

Open-source Pythonic library to compute landscape metrics within the PyData stack (NumPy, pandas, matplotlib...)

**Citation**: Bosch M. 2019. "PyLandStats: An open-source Pythonic library to compute landscape metrics". *PLOS ONE, 14(12), 1-19*. `doi.org/10.1371/journal.pone.0225734 <https://doi.org/10.1371/journal.pone.0225734>`_

.. toctree::
   :maxdepth: 1
   :caption: Reference Guide:
             
   landscape
   spatiotemporal
   zonal
   spatiotemporal-buffer

.. toctree::
   :maxdepth: 1
   :caption: Development:
             
   changelog
   contributing

This documentation is intended as an API reference. See also:

* `pylandstats-notebooks <https://github.com/martibosch/pylandstats-notebooks>`_ repository (tutorial/thorough overview of PyLandStats)
* `swiss-urbanization <https://github.com/martibosch/swiss-urbanization>`_ repository (example application of PyLandStats to evaluate the spatiotemporal patterns of urbanization in three Swiss urban agglomerations)
             
Features
--------

* Compute pandas DataFrames of landscape metrics at the patch, class and landscape level
* Analyze the spatiotemporal evolution of landscapes
* Analyze landscape changes accross environmental gradients (zonal analysis)

Using PyLandStats
-----------------

The easiest way to install PyLandStats is with conda:

    $ conda install -c conda-forge pylandstats

which will install PyLandStats and all of its dependencies. Alternatively, you can install PyLandStats using pip:

    $ pip install pylandstats


Nevertheless, note that the `BufferAnalysis` and `SpatioTemporalBufferAnalysis` classes make use of `geopandas <https://github.com/geopandas/geopandas>`_, which cannot be installed with pip. If you already have `the dependencies for geopandas <https://geopandas.readthedocs.io/en/latest/install.html#dependencies>`_ installed in your system, you might then install PyLandStats with the `geo` extras as in:

    $ pip install pylandstats[geo]
    
and you will be able to use the `BufferAnalysis` and `SpatioTemporalBufferAnalysis` classes (without having to use conda).

   
Indices and tables
==================
* :ref:`genindex`
* :ref:`modindex`
