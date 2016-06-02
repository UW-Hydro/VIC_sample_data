# VIC_sample_data
Sample datasets for the Variable Infiltration Capacity (VIC) model.

### Image Driver

**1. Stehekin**
- Domain: `image/Stehekin/parameters/domain.stehekin.20151028.nc`
- 10day Forcings: `image/Stehekin/forcings/Stehekin_image_test.forcings_10days.1949.nc`
- Global Parameters: `image/Stehekin/parameters/Stehekin_image_test.global.txt`
- Parameters: `image/Stehekin/parameters/Stehekin_test_params_20160327.nc`
    - `image/Stehekin/parameters/Stehekin_test_params_20160327.FROZEN_SOIL.nc` for the version where parameter `fs_active=1` in order to run option `FROZEN_SOIL=TRUE`

### Classic Driver

**1. Stehekin**
- 10day Forcings: `classic/Stehekin/forcings/forcings_*`
- Global Parameters: `classic/Stehekin/parameters/Stehekin_classic_test.global.txt`
- Soil Parameters: `classic/Stehekin/parameters/Stehekin_soil.txt`
    - `classic/Stehekin/parameters/Stehekin_soil.FROZEN_SOIL.txt` for the version where parameter `fs_active=1` in order to run option `FROZEN_SOIL=TRUE`
- Vegetation Parameters: `classic/Stehekin/parameters/Stehekin_vegparam.txt`
- Vegetation Library: `classic/Stehekin/parameters/Stehekin_veglib.txt`
- Snowband Parameters: `classic/Stehekin/parameters/Stehekin_snowbands.txt`
