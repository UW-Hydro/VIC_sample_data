# VIC_sample_data
Sample datasets for the Variable Infiltration Capacity (VIC) model.

The following datasets are currently available:
- [Stehekin](docs/Stehekin.md)
- [WalnutGulch](docs/WalnutGulch.md)
- [FindleyLake](docs/FindleyLake.md)

## Directory Structure (for dataset `$DATASET`)
- `docs/$DATASET.md` - documentation describing dataset `$DATASET`
- `classic/$DATASET/` - classic-driver data for dataset `$DATASET`
  - `forcings/` - ascii-format meteorological forcing files
  - `parameters/` - ascii-format parameter files (global, soil, snowband, veg)
- `image/$DATASET/` - image-driver data for dataset `$DATASET`
  - `forcings/` - NetCDF-format meteorological forcing files
  - `parameters/` - NetCDF-format parameter files (domain, parameters) plus ascii-format global parameter file
