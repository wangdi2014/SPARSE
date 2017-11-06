# Strain Prediction and Analysis using Representative SEquences (SPARSE)

SPARSE indexes >100,000 reference genomes in public databases in to hierarchical clusters and uses it to predict origins of metagenomic reads. 


[![Build Status](https://travis-ci.org/zheminzhou/SPARSE.svg?branch=master)](https://travis-ci.org/zheminzhou/SPARSE)
[![License: GPL v3](https://img.shields.io/badge/License-GPL%20v3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)

## Installation 

SPARSE requires, Operating system: Unix and Python >= version 2.7

System modules (Ubuntu 16.04) :

* pip
* gfortran
* llvm
* libncurses5-dev
* cmake
* xvfb-run (for malt, not essential)

Python modules (installed via pip):

* msgpack-python (>=0.4.8)
* numpy (>=1.13.1)
* pandas (>=0.20.3)
* pycapnp (>=0.6.0)
* ujson (>=1.35)

3rd-party softwares:
* samtools (>=1.2)
* mash (>=1.1.1)
* bowtie2 (>=2.3.2)
* malt (>=0.4.0) not essential

### Ubuntu 
     
    sudo apt-get update
    sudo apt-get install gfortran llvm libncurses5-dev cmake python-pip
    git clone git clone https://github.com/zheminzhou/SPARSE
    cd SPARSE/EM && make`
    pip install -r requirements.txt 

Change the [parameters](parameter.md) if needed. 


### Update SPARSE
To update SPARSE, move to installation directory and pull the latest version:  
`cd SPARSE`  
`git pull` 

## Next step
[Step-by-step tutorial](tutorial.md)

## Table of Contents
1. Getting started
 * [Installation](docs/installation.md)  
 * [Step-by-step tutorial](docs/tutorial.md)  
2. Reference cluster database 
 * [default database derived from NCBI RefSeq](docs/refseq.md)  
 * [insert new genomes](docs/insert.md)
3. Representative databases (MapDB)
 * [default MapDB](docs/representative.md)  
 * [Build your own representative database](docs/custom.md)
4. [Run SPARSE on assembled sequences or the whole readset](docs/mash.md)
5. [Run SPARSE on read-level prediction](docs/map.md)
 * [Extract reference-specific reads](docs/extract.md)
6. [Scripts for benchmark datasets]
7. [Citing](docs/citing.md)
