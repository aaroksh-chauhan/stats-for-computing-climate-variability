# Statistics for Computing Climate Variability

## Overview
An end-semester project applying core statistical methods to detect and 
characterize climate change signals in a long-term global temperature record, 
combining time series analysis, hypothesis testing, and frequency-domain 
(FFT) analysis.

## Objective
- Compute and visualize the global mean surface air temperature time series 
  (1948–2025)
- Quantify sampling variability by comparing two 30-year periods and computing 
  95% confidence intervals for their means
- Statistically test whether observed warming between the two periods is 
  significant (T-test) and whether variability has changed (F-test)
- Use FFT to identify dominant periodicities (seasonal and interannual cycles) 
  in the temperature signal

## Data
- **Source:** Gridded monthly mean air temperature reanalysis data (NetCDF)
- **Time period:** 1948–2025
- **Periods compared:** 1948–1977 ("Period A") vs 1995–2024 ("Period B")

## Tools & Methods
- **Language:** Python
- **Key libraries:** xarray, numpy, scipy (stats, fft), matplotlib
- **Method:** Computed a latitude-weighted global mean temperature time series, 
  extracted annual means for two 30-year periods, calculated 95% confidence 
  intervals using the T-distribution, ran a two-sample T-test and an F-test to 
  compare means and variances between periods, and applied FFT (with a 
  cycles-per-year frequency axis) to identify dominant cycles in the signal

## Results
- The global mean temperature time series showed a clear long-term warming 
  trend with expected seasonal fluctuation
- The two-sample T-test found the difference in mean temperature between the 
  two 30-year periods to be statistically significant at the 5% level, 
  indicating real warming rather than natural sampling variability
- The F-test also found a significant difference in variance between the two 
  periods
- FFT analysis of the temperature signal revealed its dominant periodic 
  components, consistent with expected seasonal and interannual climate cycles

## Skills Demonstrated
- Time series analysis of long-term climate data
- Statistical inference: confidence intervals, hypothesis testing (T-test, F-test)
- Signal processing (FFT) for climate data
- Python for scientific data analysis and visualization

## Author
Aaroksh Chauhan — M.Sc. Atmospheric and Oceanic Sciences, IIT Bhubaneswar
