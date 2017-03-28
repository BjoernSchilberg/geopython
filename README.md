# geopython

#Windows
[Miniconda](https://conda.io/miniconda.html)

#Miniconda in PATH aufnehmen.
export PATH=/home/bjoern/miniconda3/bin:$PATH

#conda-forge channel hinzufügen
conda config --add channels conda-forge

##Benötigte Biblotheken aus dem conda-forge channel installieren

#Für BSH Tutorial
conda install rasterio shapely fiona jupyter matplotlib

#Für GPS Tutorial
conda install gpxpy pandas (srtm rdp)
srtm rdp nicht in anaconda.

#Für NetCDF Tutorial
conda install netcdf4

#Jupyter Notebook starten

jupyter notebook

#Weiterführende Hinweise zu den verwendeten Biblotheken
https://github.com/conda-forge/rasterio-feedstock
https://github.com/conda-forge/shapely-feedstock
https://github.com/conda-forge/fiona-feedstock

#Debugging of conda enviroment

conda info

conda info rasterio

cat ~/.condarc
