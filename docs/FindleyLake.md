# FindleyLake Sample Dataset

## Documentation
For details on Findley Lake, explanation of how parameters were estimated, illustration of example simulations, and ideas for future improvements, see: [Preparation of VIC Parameters for Findley Lake.pdf](Preparation\ of\ VIC\ Parameters\ for\ Findley Lake.pdf).

## Files

### Image Driver

- `image/FindleyLake/parameters/` - parameter files
    - Global Parameter Files:
        - `global_param.FindleyLake.txt`
            - Domain File: `domain.FindleyLake.nc`
            - Parameter File: `params.FindleyLake.nc`
            - Forcings: `livneh_NAmerExt_15Oct2014.FindleyLake.*.nc`
            - fcanopy is used 
    - Domain Files:
        - `domain.FindleyLake.nc`
            - 0.0625 degree resolution
            - Taken from Bohn et al. (2018)
    - Parameter Files:
        - `params.FindleyLake.nc`
            - 0.0625 degree resolution
            - MOD-LSP MOD_IGBP parameters (Bohn and Vivoni, 2019)
            - Soils and snowbands from NLDAS
            - Land cover, LAI, fcanopy, and albedo from MODIS

- `image/FindleyLake/forcings/` - meteorological forcing files
    - `livneh_NAmerExt_15Oct2014.FindleyLake.*.nc` where `*` = years 1970-1979
        - Yearly files
        - 1-hour time step
        - From Livneh et al. (2015)
        - Disaggregated to hourly via MetSim (Bennett et al., 2018) v2.0.0 using "mix" precipitation option and parameters from Bohn et al. (2018)

### Classic Driver

- `classic/FindleyLake/parameters/` - parameter files
    - Global Parameter Files:
        - `global_param.FindleyLake.txt`
            - Soil Parameter File: `soil_param.FindleyLake`
            - Snowband Parameter File: none
            - Veg Library File: `veg_lib_IGBP`
            - Veg Parameter File: `veg_param.FindleyLake`
            - Lake Parameter File: `lake_param.FindleyLake`
            - Forcings: `livneh_NAmerExt_15Oct2014.FindleyLake_47.3188_-121.5853`
            - Fcanopy is used
    - Soil Parameters:
        - `soil_param.FindleyLake`
            - 1 grid cell
            - MOD-LSP MOD_IGBP parameters (Bohn and Vivoni, 2019)
    - Vegetation Library:
        - `veg_lib_IGBP`
            - MOD-LSP MOD_IGBP veglib parameters (Bohn and Vivoni, 2019)
    - Vegetation Parameters:
        - `veg_param.FindleyLake`
            - MOD-LSP MOD_IGBP veg parameters (Bohn and Vivoni, 2019)
            - Contains fcanopy

- `classic/FindleyLake/forcings/` - meteorological forcing files
    - `livneh_NAmerExt_15Oct2014.FindleyLake_47.3188_-121.5853`
        - 10 years of data, 1970-1979
        - 1-hour time step
        - From Livneh et al. (2015)
        - Disaggregated to hourly via MetSim (Bennett et al., 2018) v2.0.0 using "mix" precipitation option and parameters from Bohn et al. (2018)

## References
 - Bennett, A., J. J. Hamman, B. Nijssen, E. A. Clark, and K. M. Andreadis, 2018: UW-Hydro/MetSim: Version 1.1.0 (version 1.1.0). Zenodo, doi:10.5281/zenodo.1256120. http://doi.org/10.5281/zenodo.1256120 (Accessed June 7, 2018).
 - Bohn, T. J, and E. R. Vivoni, 2019: MOD-LSP: MODIS-Based Parameters for Variable Infiltration Capacity (VIC) Model over the Continental US, Mexico, and Southern Canada (Version 1.0) [Data set]. Zenodo, doi:10.5281/zenodo.2612560. https://zenodo.org/record/2612560.
 - Bohn, T. J., K. M. Whitney, G. Mascaro, and E. R. Vivoni, 2018: Parameters for PITRI Precipitation Temporal Disaggregation over continental US, Mexico, and southern Canada, 1981-2013 (Version 1.1) [Data set]. Zenodo, doi:10.5281/zenodo.2564019. http://zenodo.org/record/2564019.
 - Livneh, B., T. J. Bohn, D. W. Pierce, F. Munoz-Arriola, B. Nijssen, R. Vose, D. R. Cayan, and L. Brekke, 2015: A spatially comprehensive, hydrometeorological data set for Mexico, the U.S., and southern Canada 1950–2013. Nat. Sci. Data, 2, 150042, doi:10.1038/sdata.2015.42.
