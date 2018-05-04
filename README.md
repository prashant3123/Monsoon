# Monsoon

Climate scientists use methods of decomposition of Outgoing Longwave Radiation (OLR) signal obtained through satellite imagery in terms of orthogonal basis functions which are determined from the data and find both time series and spatial patterns to construct Monsoon Intraseasonal Oscillation (MISO) phases. In this project, I reconstructed MISO index without providing temporal information through the use of Support Vector Machine. Having been able to predict MISO phases using Support Vector Machine by providing less information suggests the possibility that we would be able to construct long term time series of MISO phases using rain gauge data for years before 1975 when the OLR data was not available.

I used daily mean OLR dataset obtained from National Oceanic and Atmospheric Administration. You can access the 'olr.day.mean.nc' file in the following webpage:
https://www.esrl.noaa.gov/psd/data/gridded/data.interp_OLR.html

OLR datasets was classified into differnt phases as defined in the following paper:
C. T. Sabeerali, R. S. Ajayamohan, D. Giannakis, and A. J. Majda, “Extraction and prediction of indices for monsoon intraseasonal oscillations: an approach based on nonlinear Laplacian spectral analysis,” Climate Dynamics, Dec 2017.
https://link.springer.com/content/pdf/10.1007%2Fs00382-016-3491-y.pdf

I obtained MISO1 and MISO2 data computed using Nonlinear Laplacian Spectral Analysis of OLR in the Indian region from Dr. R.S Ajayamohan, one of the co-authors of the paper mentioned above. MISO1 and MISO2 data is in 'miso.nc' file in this repository. I then computed MISO phases (1-8) when the amplitude was greater than 1.5 as defined in the paper. I labelled the phase as phase 0 when the amplitude was less than 1.5

