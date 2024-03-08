### scRNA-seq analysis in python tutorial

We gratefully acknowledge Seurat’s and Scanpy's authors for the tutorial!

Teaching session are divided into 3 session:

* 1. `teaching_session_1_clustering`:  Preprocessing and clustering 3k PBMCs of Seurat’s analsis, and scanpy's clustering tutorial for 3k PBMCs from 10x Genomics, containing preprocessing, clustering and the identification of cell types via known marker genes.

#### Environment required for notebooks

We suggest using a separate conda environment for installing scanpy and relevant packages for these tutorials.

Create conda environment and install packages 

`conda create -n teaching`
`conda activate teaching`

To use this environment in jupyter notebook, add jupyter kernel for this environment:
`conda install ipykernel -y -q`
`python -m ipykernel install --user --name teaching`

Install scanpy package and harmony required for integration
`conda install -c conda-forge scanpy python-igraph leidenalg`
`pip install harmonypy`
`pip install --user scikit-misc`
`pip install openpyxl`

Before installing this environment, scanpy and it's dependencies, it could be necessary to make sure that you are creating a fully isolated conda environment by telling python to NOT use user site for installing packages by running this line before creating conda environment and every time before activatin conda environment in a new terminal session:

`export PYTHONNOUSERSITE="literallyanyletters"