# VIC_sample_data
Sample datasets for the Variable Infiltration Capacity (VIC) model.

###1. Stehekin

**Image Driver**
- Domain: `Stehekin/image/parameters/domain.stehekin.20151028.nc`
- 10day Forcings: `Stehekin/image/forcings/Stehekin_image_test.forcings_10days.1949.nc`
- Global Parameters: `Stehekin/image/parameters/Stehekin_image_test.global.txt`
- Parameters: `Stehekin/image/parameters/Stehekin_test_params_20160327.nc`
    - `Stehekin/image/parameters/Stehekin_test_params_20160327.FROZEN_SOIL.nc` for the version where parameter `fs_active=1` in order to run option `FROZEN_SOIL=TRUE`

**Classic Driver**
- 10day Forcings: `Stehekin/classic/forcings/forcings_*`
- Global Parameters: `Stehekin/classic/parameters/Stehekin_classic_test.global.txt`
- Soil Parameters: `Stehekin/classic/parameters/Stehekin_soil.txt`
    - `Stehekin/classic/parameters/Stehekin_soil.FROZEN_SOIL.txt` for the version where parameter `fs_active=1` in order to run option `FROZEN_SOIL=TRUE`
- Vegetation Parameters: `Stehekin/classic/parameters/Stehekin_vegparam.txt`
- Vegetation Library: `Stehekin/classic/parameters/Stehekin_veglib.txt`
- Snowband Parameters: `Stehekin/classic/parameters/Stehekin_snowbands.txt`
