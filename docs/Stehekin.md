# Stehekin Sample Dataset

## Files

### Image Driver

- `image/Stehekin/parameters/` - parameter files
    - Global Parameter Files:
        - `Stehekin_image_test.global.txt`
            - Domain File: `domain.stehekin.20151028.nc`
            - Parameter File: `Stehekin_test_params_20160327.nc`
            - Forcings: `Stehekin_image_test.forcings_10days.1949.nc`
        - `global_param.Stehekin.L2015.txt`
            - Domain File: `domain.Stehekin.0.0625_deg.nc`
            - Parameter File: `params.Stehekin.L2015.nc`
            - Forcings: `Stehekin_image_test.forcings_10days.0.0625_deg.1949.nc`
        - `global_param.Stehekin.MOD_IGBP.txt`
            - Domain File: `domain.Stehekin.0.0625_deg.nc`
            - Parameter File: `params.Stehekin.MOD_IGBP.nc`
            - Forcings: `Stehekin_image_test.forcings_10days.0.0625_deg.1949.nc`
            - fcanopy is ignored 
        - `global_param.Stehekin.MOD_IGBP.Fcanopy.txt`
            - Domain File: `domain.Stehekin.0.0625_deg.nc`
            - Parameter File: `params.Stehekin.MOD_IGBP.nc`
            - Forcings: `Stehekin_image_test.forcings_10days.0.0625_deg.1949.nc`
            - fcanopy is used 
    - Domain Files:
        - `domain.stehekin.20151028.nc`
            - 0.125 degree resolution
        - `domain.Stehekin.0.0625_deg.nc`
            - 0.0625 degree resolution
            - Taken from Bohn et al. (2018)
    - Parameter Files:
        - `Stehekin_test_params_20160327.nc`
            - 0.125 degree resolution
            - NLDAS soil, snow, and veg parameters
        - `Stehekin_test_params_20160327.FROZEN_SOIL.nc`
            - Same as `Stehekin_test_params_20160327.nc` but has `fs_active=1` in order to run option `FROZEN_SOIL=TRUE`
        - `params.Stehekin.L2015.nc`
            - 0.0625 degree resolution
            - Parameters taken from Livneh et al. (2015)
            - NLDAS soil, snow, and veg parameters
        - `params.Stehekin.MOD_IGBP.nc`
            - 0.0625 degree resolution
            - MOD-LSP MOD_IGBP parameters (Bohn and Vivoni, 2019)
            - Soils and snowbands from NLDAS
            - Land cover, LAI, fcanopy, and albedo from MODIS
    - RVIC Parameters:
        - `stehekin_parameters_01.rvic.prm.Stehekin.20150727.nc`

- `image/Stehekin/forcings/` - meteorological forcing files
    - From Livneh et al. (2015)
    - `Stehekin_image_test.forcings_10days.1949.nc`
        - 0.125 degree resolution
        - 1-hour time step
        - 10 days of records
    - `Stehekin_image_test.forcings_10days.0.0625_deg.1949.nc`
        - 0.0625 degree resolution
        - 1-hour time step
        - 10 days of records

### Classic Driver

- `classic/Stehekin/parameters/` - parameter files
    - Global Parameter Files:
        - `classic/Stehekin/parameters/Stehekin_classic_test.global.txt`
            - Soil Parameters: `Stehekin_soil.txt`
            - Snowband Parameters: `Stehekin_snowbands.txt`
            - Vegetation Library: `Stehekin_veglib.txt`
            - Vegatation Parameters: `Stehekin_vegparam.txt`
            - Forcings: `forcings_*`
    - Soil Parameters:
        - `Stehekin_soil.txt`
            - 0.125 degree resolution
            - NLDAS soil parameters
        - `Stehekin_soil.FROZEN_SOIL.txt`
            - same as `Stehekin_soil.txt` but parameter `fs_active=1` in order to run option `FROZEN_SOIL=TRUE`
    - Snowband Parameters:
        - `Stehekin_snowbands.txt`
            - 0.125 degree resolution
            - NLDAS snowband parameters
    - Vegetation Library:
        - `Stehekin_veglib.txt`
            - 0.125 degree resolution
            - NLDAS veglib parameters
    - Vegetation Parameters:
        - `Stehekin_vegparam.txt`
            - 0.125 degree resolution
            - NLDAS veg parameters

- `classic/Stehekin/forcings/` - meteorological forcing files
    - From Livneh et al. (2015)
    - `forcings_*`
        - 0.125 degree resolution
        - 1-hour time step
        - 10 days of records

## References
 - Bohn, T. J, and E. R. Vivoni, 2019: MOD-LSP: MODIS-Based Parameters for Variable Infiltration Capacity (VIC) Model over the Continental US, Mexico, and Southern Canada (Version 1.0) [Data set]. Zenodo, doi:10.5281/zenodo.2612560. https://zenodo.org/record/2612560.
 - Bohn, T. J., K. M. Whitney, G. Mascaro, and E. R. Vivoni, 2018: Parameters for PITRI Precipitation Temporal Disaggregation over continental US, Mexico, and southern Canada, 1981-2013 (Version 1.1) [Data set]. Zenodo, doi:10.5281/zenodo.2564019. http://zenodo.org/record/2564019.
 - Livneh, B., T. J. Bohn, D. W. Pierce, F. Munoz-Arriola, B. Nijssen, R. Vose, D. R. Cayan, and L. Brekke, 2015: A spatially comprehensive, hydrometeorological data set for Mexico, the U.S., and southern Canada 1950–2013. Nat. Sci. Data, 2, 150042, doi:10.1038/sdata.2015.42.
