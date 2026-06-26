# Critical-Tectonic-Window
The code of Spatially Constrained Random Forest (SC-RF) is written in Python to predict the Mud Diapir Index (MDI) for the Makran Subduction Zone. The code uses 12 geophysical predictors and known mud diapir and mud volcano locations to train a Random Forest model with 5-fold cross-validation and bootstrap ensemble.

# Code support
The code is developed in Python. If you are using the data files (Accretionary-Wedge Thickness, Bulk Density, Cumulative energy release, Residual Gravity, Shear Stress, and Taper Angle), please contact me: umairkhanbku@mails.ucas.ac.cn

# Directory structure description
SC_RF_Makran.ipynb - Main Jupyter notebook

/data/raw/
- `Accretionary-Wedge Thickness (Km).dat`
- `Bathemetry (m).dat`
- `Bulk Density (Kg per m3).dat`
- `Cumulative energy release (log energy release (J)).dat`
- `Magnetic.dat`
- `Mud Diapirs Location.xlsx`
- `Residual Gravity.dat`
- `Shear Stress (MPA).dat`
- `Slab Dip (Deg.).dat`
- `Slab Tempreture (Deg.C).dat`
- `Slab Thickness (Km).dat`
- `Slab top Surface Depth (Km).dat`
- `Taper Angle (Deg.).dat`

# Data Sources
The slab surface depth, thickness, and dip angle are derived from the Slab-2 model (Hayes et al., 2018), accessed at https://www.usgs.gov/. The magnetic anomaly data are from the 2-arc-minute global grid EMAG2v3 (Meyer et al., 2017). The free-air gravity and bathymetric data are sourced from the global 1-arc-minute satellite datasets (Sandwell et al., 2014). The earthquake data are obtained from the USGS catalog and the IRIS database. The presence locations of mud diapirs and mud volcanoes are compiled from published literature (Delisle et al., 2002; Wu et al., 2021).

# Requirements
Python 3.10+
numpy, scipy, pandas, scikit-learn, matplotlib, openpyxl

## References
Delisle, G., von Rad, U., Andruleit, H., von Daniels, C., Tabrez, A. R., & Inam, A. (2002). Active mud volcanoes on-and offshore eastern Makran, Pakistan. International Journal of Earth Sciences, 91, 93-110.

Hayes, G. P., Moore, G. L., Portner, D. E., Hearne, M., Flamme, H., Furtney, M., & Smoczyk, G. M. (2018). Slab2, a comprehensive subduction zone geometry model. Science, 362(6410), 58-61.

Meyer, B., Chulliat, A., & Saltus, R. (2017). Derivation and error analysis of the earth magnetic anomaly grid at 2 arc min resolution version 3 (EMAG2v3). Geochemistry, Geophysics, Geosystems, 18(12), 4522-4537.

Sandwell, D. T., Müller, R. D., Smith, W. H. F., Garcia, E., & Francis, R. (2014). New global marine gravity model from CryoSat-2 and Jason-1 reveals buried tectonic structure. Science, 346(6205), 65-67.

Wu, T., et al. (2021). Distribution and development of submarine mud volcanoes on the Makran Continental Margin, offshore Pakistan. Journal of Asian Earth Sciences, 207, 104653.
