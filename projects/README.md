# M2POC Projects Guidline

## Github Procedure
- Fork this github repository to your own account
- Add a folder under m2poc2019/projects, name it with your last name
- Work out your project codes/documentation and stage/push it to your folder
- Once finalised, create a pull request to the main branch

## Evaluation
You will be evaluated against the quality (description & objectives) and degree of achievement of your project.
You are expected to present your work during a 15 mins presentation at the end of the class.

Your project repository folder will need to contain at least:
- a readme file with the description of your objectives, dataset used and methods applied
- at least one jupyter notebook showcasing your methodology

## Dataset used in 2019 projects

### Argo (334Mb)
Argo temperature and salinity profiles interpolated on standard depth levels from 0 to 1500m are available here:

Direct zarr download:
``https://storage.googleapis.com/sonific01/ARGO/GLOB_HOMOGENEOUS_variables.tar.gz``

Through GCS/zarr:
``https://storage.googleapis.com/sonific01/ARGO GLOB_HOMOGENEOUS_variables.zarr``

### ISAS15 Mixed Layer (377Mb)
Global Mixed layer depth, temperature and salinity on a regular grid.

Direct netcdf download:
``https://storage.googleapis.com/sonific01/ISAS15/ISAS15_ARGO_2002_2015_MLDT.nc``

### NCEP1 (657Mb)
Southern Hemisphere Atmospheric Sea Level Pressure (6 hourly):

Direct download:
``https://storage.googleapis.com/sonific01/NCEP/ncep1_slp_hem_south.tar.gz``

Through GCS/zarr:
``https://storage.googleapis.com/sonific01/NCEP/ncep1_slp_hem_south.zarr``