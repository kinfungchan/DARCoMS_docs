Usage
=====

.. _installation:

Installation
------------

To use DARCoMS, first go to the Impact Shock Mechanics Lab Gitlab Repo:

.. code-block:: console

   git chceckout DARCoMS

Creating a DARCoMS .dms Input File
----------------

To run a DARCoMS Multiscale simulation, you must create a ``.dms`` input file:


Currently DARCoMS supports the following keywords in its input file ``NDBASES``,
``FILES``, and ``COUPLING_SURFACES``. Otherwise, an exception will be raised.

An Example .dms Input File is:
.. code-block:: console

   NDBASES
   2
   FILES 
   C:\Users\DARCOMS\Benchmarks\Testing\B_LargeDomain125.dat
   C:\Users\DARCOMS\Benchmarks\Testing\B_SmallDomain250.dat
   COUPLING_SURFACES
   CONST_ACCEL
   2
   4
   1 126 252 378 504
   2 1   252 503 754
   
For running Monoscale simulations (single .dat file), the ``COUPLING_SURFACES``
should not be used.


