# Regression-based-Ocualar-Artifact-Removal-from-EEG-Data
Regression based Ocualar Artifact Removal from EEG Data

## Task at Hand
- In this notebook, we implemented a custom linear regression based artifact removal method to remove ocular artifacts from semi-simulated EEG data.
- Performance of Custom Implementation was compared with a standard EEG Signal Processing Library i.e. MNE-Python

## Result
- Signal to noise ratio (SNR) of contaminated signal was about 7dB which increased to about 44dB after removing ocular artifact.
- About 37dB increase in SNR after applying artifact correction
- Performance of custom implementation is equivalent to standard library implementation (Mine has even Better SNR)


## How to Run
Download the dataset from this link https://data.mendeley.com/datasets/wb6yvr725d/4 and place .mat files in "semi-simulated EEG-EOG dataset" folder. This folder also contains original article describing the dataset so check it out.

You will need following Python Libraries to execute this program
- MNE-Python
- Numpy
- Scipy
- Mat4py
- OS

## Need Help
Reach me out at: SulemanRasheedEngr@gmail.com
