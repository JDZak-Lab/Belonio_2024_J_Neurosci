# Belonio_2025_J_Neurosci
Datasets and Code from Belonio et al., 2024 Journal of Neuroscience

All imaging datasets are provided as a mean dff value of five seconds after the onset of odorant delivery.

Datasets in 'OSN_mean_vals.mat' will open as a matrix with the following dimensions, region of interest x odorant x trial. Missing observations are padded with NaN. The odorant in position 1 corresponds to a blank odorant. The following odorant indices are provided in the publication.

Data extraction code uses a modified version of the CaImAn CMNFe pipeline (https://github.com/flatironinstitute/CaImAn) and NoRMCorre for motion correction and denoising (https://github.com/flatironinstitute/NoRMCorre). To execute, run the function “extract_imaging_data.m”. Input requires an integer “frame_rate” and a logical for running motion correction. Data must exist in a directory containing.tiff files.
