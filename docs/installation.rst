===========
Installation guide
===========

SPARSE runs on Unix and requires Python >= version 2.7

System modules (Ubuntu 16.04) :

* pip
* gfortran
* llvm
* libncurses5-dev
* cmake
* xvfb-run (for malt, optional)

3rd-party software:
* samtools (>=1.2)
* mash (>=1.1.1)
* bowtie2 (>=2.3.2)
* malt (>=0.4.0) (optional)

See [requirements.txt](requirements.txt) for python module dependancies. 

### Ubuntu 

.. code-block:: bash
     
    sudo apt-get update
    sudo apt-get install gfortran llvm libncurses5-dev cmake python-pip samtools bowtie2
    git clone git clone https://github.com/zheminzhou/SPARSE
    cd SPARSE/EM && make
    pip install -r requirements.txt 

Change the [parameters](parameter.md) if needed. 


## Updating SPARSE
To update SPARSE, move to installation directory and pull the latest version:  
`cd SPARSE`  
`git pull` 