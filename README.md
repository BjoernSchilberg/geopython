# geopython

## Inhalte

- [Arbeiten mit Geo Vektordaten](bsh.ipynb)
- [Verschiedene Möglichkeiten Shapefiles zu laden/öffnen](shapefiles.ipynb)
- [Koordinatentransformation mittels pyproj](proj4.ipynb)
- [Arbeiten mit GPS Daten](bsh.ipynb)
- [Arbeiten mit Landsat-Daten](Landsat.ipynb)
- [Arbeiten mit dem Network Common Data Format (NetCDF) Dateiformat](netcdf.ipynb)
- [Arbeiten mit Meereisdaten](meereisdaten.ipynb)

## Essential Python Geospatial Libraries

- fiona - For making it easy to read/write geospatial data formats
- ipython - For a wondering interactive environment in which to play
- matplotlib - For all my plotting needs
- numpy - For pretty much anything that involves arrays
- ogr/gdal - For reading, writing, and transforming geospatial data formats
- pyproj - For conversions between projections
- rasterio - For raster handling
- shapely - For geometry handling

## Books on Python Geospatial Development
- https://www.packtpub.com/application-development/python-geospatial-development-third-edition
- https://www.manning.com/books/geoprocessing-with-python

## Installation

### GNU/Linux with Miniconda
- [Miniconda Download](https://conda.io/miniconda.html)
- [Linux Miniconda install](https://conda.io/docs/install/quick.html#linux-miniconda-install)

#### Miniconda in PATH aufnehmen.
```
export PATH=/home/bjoern/miniconda3/bin:$PATH
```

#### conda-forge channel hinzufügen
```
conda config --add channels conda-forge
conda config --set ssl_verify false
conda update openssl cryptography
conda config --set ssl_verify true
```

#### Benötigte Biblotheken aus dem conda-forge channel installieren

- Für BSH Tutorial
```
conda install rasterio shapely fiona jupyter matplotlib
```
- Für GPS Tutorial
```
conda install gpxpy pandas
```
srtm rdp nicht in Miniconda.
- Für NetCDF Tutorial
```
conda install netcdf4 xarray
```
- Für Meereis Tutorial
```
conda install basemap-data-hires
```

#### Jupyter Notebook starten
```
jupyter notebook
```

#### Weiterführende Hinweise zu den verwendeten Biblotheken in Miniconda
- https://github.com/conda-forge/rasterio-feedstock
- https://github.com/conda-forge/shapely-feedstock
- https://github.com/conda-forge/fiona-feedstock

#### Debugging of conda enviroment
```
conda info

conda info rasterio

cat ~/.condarc
```
### Install in Miniconda in Windows
TODO

### Unofficial Windows Binaries for Python Extension Packages (Alternative to Miniconda under Windows)
- http://www.lfd.uci.edu/~gohlke/pythonlibs/

- Download GDAL from: http://www.lfd.uci.edu/~gohlke/pythonlibs/#gdal
- Download Rasterio from: http://www.lfd.uci.edu/~gohlke/pythonlibs/#rasterio
- Download Fiona from: http://www.lfd.uci.edu/~gohlke/pythonlibs/#fiona
- Download Pyproj from: http://www.lfd.uci.edu/~gohlke/pythonlibs/#pyproj

Install binaries:

```
pip install -U pip
pip install GDAL-2.0.2-cp35-none-win32.whl
pip install rasterio-0.31.0-cp35-none-win32.whl
pip install Fiona-1.6.3-cp35-none-win32.whl
pip install pyproj-1.9.5-cp35-none-win32.whl
```

