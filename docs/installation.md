### Requirements

* Operating system: Unix 
* Python >=2.7

System modules (Ubuntu 16.04) :

* gfortran
* wget
* curl
* llvm
* libncurses5-dev
* cmake
* capnproto

Python modules (installed via pip):

* msgpack-python (>=0.4.8)
* numpy (>=1.13.1)
* pandas (>=0.20.3)
* psycopg2 (>=2.6)
* pycapnp (>=0.6.0)
* ujson (>=1.35)

3rd-party softwares:
* samtools (>=1.2)
* mash (>=1.1.1)
* bowtie2 (>=2.3.2)
* malt (>=0.4.0) not essential

### Download and install the software
`git clone https://github.com/zheminzhou/SPARSE`
`cd SPARSE/EM && make`

### Update SPARSE
To update SPARSE, move to installation directory and pull the latest version:  
`cd SPARSE`  
`git pull` 

## Next step
[Step-by-step tutorial](docs/tutorial.md)