# geog_wrf
Minimum geographical data required for running WRF

Unzip the .tar.bz2 zipped file by using these commands:

```bash
bunzip2 geog_min.tar.bz2
tar xvf geog_min.tar
```
Move the *geog_min* folder to a specific folder in your linux, and set the corresponding path in the namelist.wps

```
geog_data_path = '/home/ankur/WRF_Model/wrf/WPS_del/geog'
```

As this is the minimum requirements for geogrid.exe to compile, one needs to modify *geog_data_res* in the wps.namelist
```
geog_data_res = '2deg+gtopo_10m+usgs_10m+nesdis_greenfrac+10m'

```
