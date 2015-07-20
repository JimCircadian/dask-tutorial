Dask Tutorial
=============

Dask provides multi-core execution on larger-than-memory datasets.

We can think of dask at a high and a low level

*  **High level collections:**  Dask provides high-level Array, DataFrame
   collections that mimic NumPy, and Pandas but can operate in parallel on
   datasets that don't fit into main memory.  Dask's high-level collections are
   alternatives to NumPy and Pandas for large datasets.
*  **Low Level schedulers:** Dask provides dynamic task schedulers that
   execute task graphs in parallel.  These execution engines power the
   high-level collections mentioned above but can also power custom workloads.
   These schedulers are low-latency (around 1ms) and work hard to run
   computations in a small memory footprint.  Dask's schedulers are an
   alternative to direct use of `threading` or `multiprocessing` libraries in
   complex cases or other task scheduling systems like `Luigi` or
   `IPython parallel`.

Different users operate at different levels but it is useful to understand
both.  This tutorial will interleave between high-level use of `dask.array` and
`dask.dataframe` (even sections) and low-level use of dask graphs and
schedulers (odd sections.)

Links
-----

*  [Code](https://github.com/ContinuumIO/dask/)
*  [Docs](https://dask.pydata.org/en/latest/)

Outline
-------

0.  Dask Arrays

    *  [Arrays](00-Array.ipynb)

1.  Dask graphs and other fundamentals

    *  [Foundations](01-Foundations.ipynb)

2.  Tabular compuations with DataFrames

    *  [DataFrames](02-DataFrame.ipynb)
    *  [DataFrame Storage](03-DataFrame-Storage.ipynb)

3.  Imperative Programming

    *  [Imperative - `do`](04-Imperative.ipynb)

4.  Semi-structured data with Bag

    *  ...

5.  Graph analysis, optimization, and diagnostics

    *  ...
