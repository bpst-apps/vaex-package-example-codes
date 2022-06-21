## What is Vaex?
Vaex is a python library for lazy `Out-of-Core DataFrames` (similar to Pandas), to visualize and explore big tabular datasets. It can calculate statistics such as mean, sum, count, standard deviation etc, on an N-dimensional grid up to a billion () objects/rows per second. Visualization is done using histograms, density plots and 3d volume rendering, allowing interactive exploration of big data. Vaex uses memory mapping, a zero memory copy policy, and lazy computations for best performance (no memory wasted).

## Why vaex?
* **Performance:** works with huge tabular data, processes  rows/second
* **Lazy / Virtual columns:** compute on the fly, without wasting ram
* **Memory efficient** no memory copies when doing filtering/selections/subsets.
* **Visualization:** directly supported, a one-liner is often enough.
* **User friendly API:** you will only need to deal with the DataFrame object, and tab completion + docstring will help you out: ds.mean<tab>, feels very similar to Pandas.
* **Lean:** separated into multiple packages
   * **vaex-core:** DataFrame and core algorithms, takes numpy arrays as input columns.
   * **vaex-hdf5:** Provides memory mapped numpy arrays to a DataFrame.
   * **vaex-arrow:** Arrow support for cross language data sharing.
   * **vaex-viz:** Visualization based on matplotlib.
   * **vaex-jupyter:** Interactive visualization based on Jupyter widgets / ipywidgets, bqplot, ipyvolume and ipyleaflet.
   * **vaex-astro:** Astronomy related transformations and FITS file support.
   * **vaex-server:** Provides a server to access a DataFrame remotely.
   * **vaex-distributed:** (Deprecated) Now part of vaex-enterprise.
   * **vaex-qt:** Program written using Qt GUI.
   * **vaex:** Meta package that installs all of the above.
   * **vaex-ml:** Machine learning

* **Jupyter integration:** vaex-jupyter will give you interactive visualization and selection in the Jupyter notebook and Jupyter lab.

## Installation
Using conda:

  ```conda install -c conda-forge vaex```
Using pip:

  ```pip install --upgrade vaex```
