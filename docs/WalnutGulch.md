# WalnutGulch Sample Dataset

### Image Driver

- `image/WalnutGulch/parameters/` - parameter files
    - Global Parameter Files:
        - `global_param.WalnutGulch.L2015.txt`
            - Domain File: `domain.WalnutGulch.0.0625_deg.nc`
            - Parameter File: `params.WalnutGulch.L2015.0.0625_deg.nc`
            - Forcings: `livneh_NAmerExt_15Oct2014.WalnutGulch.2008.nc`
        - `global_param.WalnutGulch.MOD_IGBP.txt`
            - Domain File: `domain.WalnutGulch.0.0625_deg.nc`
            - Parameter File: `params.WalnutGulch.MOD_IGBP.0.0625_deg.nc`
            - Forcings: `livneh_NAmerExt_15Oct2014.WalnutGulch.2008.nc`
            - fcanopy is ignored 
        - `global_param.WalnutGulch.MOD_IGBP.Fcanopy.txt`
            - Domain File: `domain.WalnutGulch.0.0625_deg.nc`
            - Parameter File: `params.WalnutGulch.MOD_IGBP.0.0625_deg.nc`
            - Forcings: `livneh_NAmerExt_15Oct2014.WalnutGulch.2008.nc`
            - fcanopy is used 
    - Domain Files:
        - `domain.WalnutGulch.0.0625_deg.nc`
            - 0.0625 degree resolution
            - Taken from Bohn et al. (2018)
    - Parameter Files:
        - `params.WalnutGulch.L2015.0.0625_deg.nc`
            - 0.0625 degree resolution
            - Parameters taken from Livneh et al. (2015)
            - NLDAS soil, snow, and veg parameters
        - `params.WalnutGulch.MOD_IGBP.0.0625_deg.nc`
            - 0.0625 degree resolution
            - MOD-LSP MOD_IGBP parameters (Bohn and Vivoni, 2019)
            - Soils and snowbands from NLDAS
            - Land cover, LAI, fcanopy, and albedo from MODIS

- `image/WalnutGulch/forcings/` - meteorological forcing files
    - `livneh_NAmerExt_15Oct2014.WalnutGulch.2008.nc`
        - 0.0625 degree resolution
        - 3-hour time step
        - 366 days of records

### Classic Driver

Currently there are no classic driver inputs for this dataset.

## References
 - Bohn, T. J, and E. R. Vivoni, 2019: MOD-LSP: MODIS-Based Parameters for Variable Infiltration Capacity (VIC) Model over the Continental US, Mexico, and Southern Canada (Version 1.0) [Data set]. Zenodo, doi:10.5281/zenodo.2612560. https://zenodo.org/record/2612560.
 - Bohn, T. J., K. M. Whitney, G. Mascaro, and E. R. Vivoni, 2018: Parameters for PITRI Precipitation Temporal Disaggregation over continental US, Mexico, and southern Canada, 1981-2013 (Version 1.1) [Data set]. Zenodo, doi:10.5281/zenodo.2564019. http://zenodo.org/record/2564019.
 - Livneh, B., T. J. Bohn, D. W. Pierce, F. Munoz-Arriola, B. Nijssen, R. Vose, D. R. Cayan, and L. Brekke, 2015: A spatially comprehensive, hydrometeorological data set for Mexico, the U.S., and southern Canada 1950–2013. Nat. Sci. Data, 2, 150042, doi:10.1038/sdata.2015.42.
