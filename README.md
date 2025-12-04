# Timing Tutorials

This repository contains tutorials for X-ray timing analysis, focusing on different types of astronomical sources and analysis techniques.

Different versions of these tutorials were done at 
+ [ASI School on IXPE data analysis for General Observers at ASI headquarters, Rome, February 20-23 2024](https://www.asi.it/formazione_esterna/alta-formazione/asi-school-on-ixpe-data-analysis-for-general-observers/)
+ [NICER-IXPE workshop July 29 to August 1 2024 in Washington, DC](https://heasarc.gsfc.nasa.gov/docs/ixpe/analysis/workshop/joint2024.html)
+ ACME tutorial on Spectral Timing, Toulouse, November 13th, 2025
+ [ASTRAL-X X-ray astronomy school, La Plata, Argentina, 1-12 December 2025](https://congresos.unlp.edu.ar/astralx/)

## Directory Structure

### `SlowPulsar`
Tutorial on slow pulsar search and polarimetry analysis.

**Contents:**
- Slow_pulsar_search_and_polarimetry_tutorial.ipynb - Jupyter notebook demonstrating pulsar timing and polarimetry techniques
- README.md - Documentation for the slow pulsar tutorial

**Software Requirements:**
- Python 3.11+
- astropy, h5py, netcdf4, numba, pint-pulsar
- stingray, hendrics
- jupyter, ipympl
- optional: ixpeobssim (requires HEASOFT)

### `Spectraltiming`
Tutorial on spectral timing exploration of accreting black holes using NICER data.

**Contents:**
- Spectral Timing Exploration.ipynb - Comprehensive tutorial analyzing MAXI J1820+070 outburst data
- epoch_0_data.csv - Epoch 0 hardness-intensity data from Wang et al. 2021
- wang_data.csv - Complete outburst hardness-intensity data from Wang et al. 2021
- README.md - Detailed documentation and data information

**Tutorial Topics:**
- Hardness-intensity diagrams and spectral colors
- Power density spectra (PDS) analysis
- Power colors for understanding spectral states
- Lag spectra and covariance spectra
- Energy-dependent timing properties

**Data:**
The tutorial analyzes a NICER observation of MAXI J1820+070 from the 2018 outburst. Data can be downloaded from [Zenodo](https://zenodo.org/records/13149195) in three formats:
- Original ~2.4GB FITS file
- Reduced ~720MB HDF5 file
- Further reduced ~370MB HDF5 file

**Disclaimer:** The dataset is for demonstration purposes only and is not science-ready. It contains instrumental artifacts and has not been processed through the complete NICER pipeline.

## References

The spectral timing tutorial reproduces results from:
- [Wang et al. 2021](https://ui.adsabs.harvard.edu/abs/2021ApJ...910L...3W/abstract)
- [De Marco et al. 2021](https://ui.adsabs.harvard.edu/abs/2021A%26A...654A..14D/abstract)
- [Heil et al. 2015](https://ui.adsabs.harvard.edu/abs/2015MNRAS.448.3339H/abstract) (power colors)
- [Kara et al. 2019](https://www.nature.com/articles/s41586-018-0803-x) (spectral timing properties)

## Additional Resources

- [NICER Analysis Threads](https://heasarc.gsfc.nasa.gov/docs/nicer/analysis_threads/)
- [Notes on Timing Analyses and NICER Data](https://heasarc.gsfc.nasa.gov/docs/nicer/data_analysis/workshops/nicer_wkshp_timing_5_4_21.pdf)
