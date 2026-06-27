# Critical Tectonic Window of Mud Diapirs

The Geophysically Constrained Random Forest (GC-RF) model is written in Python to predict margin-scale mud diapir spatial distributions in the Makran subduction zone. Twelve geophysical predictors and known mud diapir and mud volcano locations were used to train a Random Forest model with 5-fold cross-validation and bootstrap ensemble to generate the Mud Diapir Index (MDI).

## How to Run in Google Colab (Recommended)

Simply click the link below to open the notebook in Google Colab and run all cells:

```
https://colab.research.google.com/github/Dr-UmairKhan/Critical-Tectonic-Window/blob/main/SC_RF_Makran.ipynb
```

No installation required.

## Code support

The code is developed in Python. If you are using the data files (Accretionary-Wedge Thickness, Bulk Density, Cumulative energy release, Residual Gravity, Shear Stress, Slab Tempreture and Taper Angle), please contact me: umairkhanbku@gmail.com

## Directory structure description

```
The repository contains the main Jupyter notebook (SC_RF_Makran.ipynb) and a data/raw/ folder with 13 input files: Accretionary-Wedge Thickness, Bathemetry, Bulk Density, Cumulative energy release, Magnetic, Mud Diapirs Location, Residual Gravity, Shear Stress, Slab Dip, Slab Tempreture, Slab Thickness, Slab top Surface Depth, and Taper Angle. The outputs/ folder is generated after running the notebook.
```

## Data Sources

The slab surface depth, thickness, and dip angle are derived from the Slab-2 model (Hayes et al., 2018), accessed at https://www.usgs.gov/. The magnetic anomaly data are from the 2-arc-minute global grid EMAG2v3 (Meyer et al., 2017). The free-air gravity and bathymetric data are sourced from the global 1-arc-minute satellite datasets (Sandwell et al., 2014). The earthquake data are obtained from the USGS catalog and the IRIS database. The presence locations of mud diapirs and mud volcanoes are compiled from published literature (Delisle et al., 2002; Wu et al., 2021).

## Requirements

```
Python 3.10+
numpy, scipy, pandas, scikit-learn, matplotlib, openpyxl
```

## References

Delisle, G., von Rad, U., Andruleit, H., von Daniels, C., Tabrez, A. R., & Inam, A. (2002). Active mud volcanoes on-and offshore eastern Makran, Pakistan. *International Journal of Earth Sciences*, 91, 93-110.

Hayes, G. P., Moore, G. L., Portner, D. E., Hearne, M., Flamme, H., Furtney, M., & Smoczyk, G. M. (2018). Slab2, a comprehensive subduction zone geometry model. *Science*, 362(6410), 58-61.

Meyer, B., Chulliat, A., & Saltus, R. (2017). Derivation and error analysis of the earth magnetic anomaly grid at 2 arc min resolution version 3 (EMAG2v3). *Geochemistry, Geophysics, Geosystems*, 18(12), 4522-4537.

Sandwell, D. T., Müller, R. D., Smith, W. H. F., Garcia, E., & Francis, R. (2014). New global marine gravity model from CryoSat-2 and Jason-1 reveals buried tectonic structure. *Science*, 346(6205), 65-67.

Wu, T., et al. (2021). Distribution and development of submarine mud volcanoes on the Makran Continental Margin, offshore Pakistan. *Journal of Asian Earth Sciences*, 207, 104653.
