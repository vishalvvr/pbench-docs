.. pbench documentation master file, created by
   sphinx-quickstart on Fri Nov  6 22:27:57 2020.
   You can adapt this file completely to your liking, but it should at least
   contain the root `toctree` directive.

Pbench
######

A a Benchmarking and Performance Analysis Framework.

Sub-systems:
************

.. dropdown:: Pbench Agent
   :animate: fade-in-slide-down

    The Agent is responsible for providing commands for running benchmarks across one or more systems, while properly collecting the 
    configuration of those systems, their logs, and specified telemetry from various tools (sar, vmstat, perf, etc).
   
   :doc:`src/agent/index`
   
.. dropdown:: Pbench Server
   :animate: fade-in-slide-down

    The second sub-system included here is the Server, which is responsible for archiving results and indexing them to 
    allow the dashboard to prepare visualizations of the results.
   
   :doc:`src/server/index`

.. dropdown:: Dashboard
   :animate: fade-in-slide-down

    Lastly, the Dashboard is used to display visualizations in graphical and other forms of the results that were collected 
    by the Agent and indexed by the Server.

   :doc:`src/dashboard/index`

.. toctree::
   :maxdepth:2
   :caption: Table of Contents
   :hidden:
   :titlesonly:
   :glob:

   src/getting_started
   src/agent/index
   src/server/index
   src/dashboard/index
