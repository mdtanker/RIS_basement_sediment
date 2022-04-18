# Depth to magnetic basement beneath Antarctica's Ross Ice Shelf  

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.6363912.svg)](https://doi.org/10.5281/zenodo.6363912)  ![GitHub top language](https://img.shields.io/github/languages/top/mdtanker/RIS_basement_sediment)  

<!-- <p align="center">
    <img src="https://github.com/mdtanker/readme_stuff/blob/main/ROSETTA.png" width=20%/>
    <img src="https://github.com/mdtanker/readme_stuff/blob/main/VUW.png" width=20%/>
    <img src="https://github.com/mdtanker/readme_stuff/blob/main/ANZ.png" width=20%/>
    <img src="https://github.com/mdtanker/readme_stuff/blob/main/GNS.png" width=20%/>
</p> -->

|   |   |   |   |
|:--:|---|---|:--:|
| <img width="200" src="https://github.com/mdtanker/RIS_basement_sediment/blob/main/ROSETTA.png"> | <img width="200" src="https://github.com/mdtanker/RIS_basement_sediment/blob/main/VUW.png"> | <img width="200" src="https://github.com/mdtanker/RIS_basement_sediment/blob/main/ANZ.png"> | <img width="200" src="https://github.com/mdtanker/RIS_basement_sediment/blob/main/GNS.png"> |





<p align="center">
    <img src="https://github.com/mdtanker/RIS_basement_sediment/blob/main/Figures/outputs/cover_fig.png" width="600">
</p> 

This repository accompanies our 2022 Geophysical Research Letters article *Basement topography and sediment thickness beneath Antarctica's Ross Ice Shelf*.

Here we document our scientific workflow in a Jupyter notebook, present our gridded results as netCDF files, and showcase our figures created using PyGMT.

The main body of this work centers on the Werner deconvolution of airborne magnetics data from a 10km grid of flight line data (ROSETTA-Ice) over the Ross Ice Shelf. The deconvolution and subsequent filtering/binning of the results give a magnetic basement surface, which represents to contact between non-magnetic sediments/sedimentary rocks and underlying crystalline basement. These results are also hosted at [PANGAEA](https://doi.pangaea.de/10.1594/PANGAEA.941238).

To view the main notebook without downloading it use [nbview.org](https://nbviewer.org/github/mdtanker/RIS_basement_sediment/blob/main/Tankersley2022_GRL.ipynb).

<!---[Basement Depths for Ross Ice Shelf](https://github.com/[username]/[reponame]/blob/[branch]/image.jpg?raw=true)--->

## Installation

### Download a copy of this repository
**Option 1:** use git to clone this to you computer.  
If you have windows, download [Git-bash](https://gitforwindows.org/) (through Git for windows). In the command prompt enter:

    git clone https://github.com/mdtanker/RIS_basement_sediment
  
**Option 2:** Click the green button above and download the .zip file.    
Unzip the folder where you want the repository stored.

### Setup Python and conda environment
If you don't have Python setup on your machine, I suggest downloading [*mini-forge*](https://github.com/conda-forge/miniforge) which is a easy-install, open-source alternative to *Anaconda* for using Python.

Next you need to create a new environement and download the necessary Python packages, using the .yml file.   

In *miniforge prompt*, cd into the RIS_basement_sediment folder:  

    cd RIS_basement_sediment
    
and enter the following: (replace "my_env" with a new name, I used "basement")

    conda env create --name my_env -f basement.yml

Now add a kernel for this environment to Jupyter lab. In *miniforge prompt*:

    ipython kernel install --name my_env

If this gives an error enter the following and retry:
	
	conda install ipython jupyter 
  
## Running Jupyter lab
In *miniforge prompt* 

    activate pygmt06
    jupyter lab
    
Open the *Tankersley2022_GRL.ipynb* to follow through our workflow. Use the *Table of Contents* button on the left to show the notebook outline. Note there are a few files needed to be downloaded seperately, as shown in the notebook.

## Citing
This *Geophysical Research Letters* paper can be cited with the following citation or BibTex code:

Tankersley, M. D., Horgan, H. J., Siddoway, C. S., Caratori Tontini, F., & Tinto, K. J. (2022). Basement topography and sediment thickness beneath Antarctica’s Ross Ice Shelf imaged with airborne magnetic data. Geophysical Research Letters.

    @article{tankersleybasement2022,
      title = {Basement Topography and Sediment Thickness beneath {{Antarctica}}'s {{Ross Ice Shelf}} Imaged with Airborne Magnetic Data},
      author = {Tankersley, M.D. and Horgan, H. J. and Siddoway, C. S. and Caratori Tontini, F. and Tinto, K. J.},
      year = {2022},
      journal = {Geophysical Research Letters}
    }
