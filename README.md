# Regression-based-Ocualar-Artifact-Removal-from-EEG-Data
Regression based Ocualar Artifact Removal from EEG Data


## Key Points
- In this notebook, we will implement linear regression based artifact removal method to remove ocular artifacts from simulated EEG data. 
- from calibration run, we predicted contaminated eeg coefficients from eog data and then for testing phase we subtracted the contaminated eeg from recorded eeg. The contaminated eeg was found by multiplying the new eog with calibrated contamination coeffs (betas)
- ***close plotting window by escape bar and don't close it manually otherwise mne crashes, jupyter lab seems to be better in notebook for plotting***
- Four class motor imagery (001-2014) data set 2a of the BCI Competition IV. http://bnci-horizon-2020.eu/database/data-sets
- simulated eeg eog dataset link https://data.mendeley.com/datasets/wb6yvr725d/4
- scipy's loadmat is much faster than mat4py's loadmat (about 10 times or more)**
