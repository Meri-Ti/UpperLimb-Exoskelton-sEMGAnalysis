# sEMG Data Analysis

This repository contains MATLAB live scripts for analyzing sEMG (surface Electromyography) signals collected from three different subjects (`S1`, `S2`, and `S3`). Each subject has a dedicated folder that contains the data and scripts specific to their acquisition sessions.

## Repository Structure

The repository is organized into three main folders, each corresponding to a different subject:

- **S1/**: Contains data and scripts for Subject 1.
- **S2/**: Contains data and scripts for Subject 2.
- **S3/**: Contains data and scripts for Subject 3.

### Folder Contents

Each folder (`S1`, `S2`, `S3`) contains the following files:

- **`sEMG_S1.mlx`, `sEMG_S2.mlx`, `sEMG_S3.mlx`**: MATLAB live scripts used to process and analyze the sEMG data for each subject. The scripts also supports the analysis of various angles (30°, 60°, 90°) for horizontal abduction exercises, in addition to the different modes for the upper limb exoskeleton usage (Assistance, Resistance, and Transparency). All the plot are stored in SVG file for a good resolution and the figures of the Pect. Major muscle have a higher dimension since it has been taken as the sample muscle for the Thesis purpose. 
- **Collected Data Files**: Raw data collected from EMG and Motion Tools software (these files are unique for each subject and stored in folders named accordingly, respectively S1_C3D, S1_ASCIII etc...).

## Data Collection Tools

The data has been collected using the following tools:

1. **sEMG Electrodes**: Used for capturing electrical activity produced by skeletal muscles.
2. **EMG and Motion Tools** software: Used for tracking motion data (such as accelerometer and gyroscope data) during the experiments.

## How to Use

1. **Clone the repository**:
    ```bash
    git clone https://github.com/Meri-Ti/UpperLimb-Exoskelton-sEMGAnalysis.git
    ```

2. **Navigate to the folder** of the desired subject (`S1`, `S2`, or `S3`).

3. **Open the MATLAB live script** (`.mlx` file) corresponding to the subject to view, modify, and run the analysis.

## Live Script Functionality

Each MATLAB live script (`sEMG_S1.mlx`, `sEMG_S2.mlx`, `sEMG_S3.mlx`) contains sections that perform the following tasks:

- Load the EMG and motion data.
- Apply preprocessing steps, such as Pass-Band Butterworth and Notch filters; normalization to the MVC.
- Extract relevant features from the data (e.g., mean, RMS, frequency domain features with FFT and PSD).
- Visualize the data through plots for better understanding.

## Acknowledgments

- All subjects who participated in the data collection process.
