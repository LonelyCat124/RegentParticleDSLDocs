============================
Installing RegentParticleDSL
============================

Downloading the repository
--------------------------

Currently RegentParticleDSL is not open for general access, once we have some initial testing completed, this will be available.
If you have access to the repository, it can be downloaded through git as usual.

Requirements
------------
RegentParticleDSL requires nothing special other than a working version of Regent, and a HDF5 installation.
The easiest way to have this is to use the Dockerfile available in the repository, and mount the DSL into the docker image. 
On linux, this will build and run the docker image, and mount the currently directory as ``/DSL``.::
  docker build -t regentparticle
  docker run -it -v $PWD:/DSL regentparticle

Alternatively, these libraries can be built yourself on linux. Instructions for Regent are available on http://regent-lang.org/install/, 
and HDF5 is available at https://www.hdfgroup.org/solutions/hdf5/. Regent needs to be built with the ``--hdf5`` option.
