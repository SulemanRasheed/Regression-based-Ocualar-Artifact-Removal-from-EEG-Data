# Regression-based-Ocualar-Artifact-Removal-from-EEG-Data
Regression based Ocualar Artifact Removal from EEG Data


## Key Points
- In this notebook, we will implement linear regression based artifact removal method to remove ocular artifacts from simulated EEG data. 
- from calibration run, we predicted contaminated eeg coefficients from eog data and then for testing phase we subtracted the contaminated eeg from recorded eeg. The contaminated eeg was found by multiplying the new eog with calibrated contamination coeffs (betas)
- ***close plotting window by escape bar and don't close it manually otherwise mne crashes, jupyter lab seems to be better in notebook for plotting***
- Four class motor imagery (001-2014) data set 2a of the BCI Competition IV. http://bnci-horizon-2020.eu/database/data-sets
- simulated eeg eog dataset link https://data.mendeley.com/datasets/wb6yvr725d/4
- scipy's loadmat is much faster than mat4py's loadmat (about 10 times or more)**


## Some Observations
- SNR of contaminated signal was about 7dB which increased to about 44dB after removing ocular artifact.
- About 37dB increase in SNR after applying artifact correction
- Performance of custom implementation is equivalent to standard library implementation (Strictly Speaking mine is slightly Better!)

Things to Consider
- Assumption is that there is linear relationship between eog and eeg eye artifact
- what if eog channels can't pick all the time, whole assumption is broken and results would be effected
