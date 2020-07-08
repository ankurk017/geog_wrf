# geog_wrf


#### A. USAGE
Minimum geographical data required for running WRFv3 and WRFv4.
* For WRF version 4 users, use `geog_data_min_v4.tar.bz2`.
* For WRF WRF version 3.9.1.1 (or lower), use `geog_data_min_v3.tar.bz2`

#### B. HOW TO USE GEOGRAPHICAL DATA
Unzip the `.tar.bz2` zipped file by using these commands:

```bash
bunzip2 geog_min.tar.bz2
tar xvf geog_min.tar
```
Move the `geog_min` folder to a specific folder in your linux, and set the corresponding path in the namelist.wps

#### C. CHANGES REQUIRED IN NAMELIST
Mention the geographical data path in the `namelist.wps`
```
geog_data_path = '/home/username/WRF_Model/WPS/geog'
```

As this is the minimum requirements for `geogrid.exe` to compile, one needs to modify `geog_data_res` in the wps.namelist
```
geog_data_res = '2deg+gtopo_10m+usgs_10m+nesdis_greenfrac+10m'

```
