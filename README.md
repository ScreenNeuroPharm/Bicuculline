# Bicuculline

[![License](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/ScreenNeuroPharm/Bicuculline/blob/master/LICENSE)

> The repository contains the data and the functions needed to reproduce the analysis reported in the article "Lack of epileptogenic effects of the creatine precursor guanidinoacetic acid on neuronal cultures in vitro"


## Details
All uploaded scripts work with a .mat format. 
To reproduce our analysis is necessary to convert the ```.txt``` format file in ```.mat``` format file using the function ```TxT2Mat.m``` in the folder Conversion. 
All electrophysiological recordings are long 8 minutes and sampled at 10 KHz. 
```TxT2Mat.m``` function allows obtaining for each electrode (60) the peak train .mat file. 
Peak_train file is a sparse vector that reports the spike occur, saving the spike amplitudute.

### Code folder architecture:
- Conversion folder:
    * Txt2Mat: function to convert ```.txt``` format file in ```.mat``` format file

- DoseResponseCurve folder: function to estimate the dose-response curve and the relative parameters.

- SpikeAnalysis folder:
    * MFR: function to compute the Mean Firing Rate


- Utilities: supplementary functions
