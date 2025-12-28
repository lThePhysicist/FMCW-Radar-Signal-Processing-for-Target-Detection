# FMCW-Radar-Signal-Processing-for-Target-Detection
MATLAB-based FMCW radar signal processing pipeline implementing 2D-FFT (Range-Doppler), MTI clutter suppression, and automated target detection.
Project Overview
Developed a robust signal processing pipeline in MATLAB to process raw ADC data from a Frequency-Modulated Continuous Wave (FMCW) radar. This project implements a complete chain from raw data ingestion to high-resolution Range-Doppler visualizations.

The system is designed to detect valid targets in noisy environments by utilizing 2D-FFT processing, MTI (Moving Target Indication) filtering, and adaptive noise floor analysis. It provides real-time insights into target range and velocity dynamics, making it suitable for automotive or surveillance radar applications.

Key Features
2D-FFT Chain: Implements Range FFT and Doppler FFT sequentially to generate high-resolution Range-Doppler Maps (RDM).

Clutter Suppression: Utilizes MTI filtering to remove static objects and low-frequency clutter from the scene.

Sidelobe Reduction: Applies Hamming windowing prior to FFT processing to minimize spectral leakage.

Automated Target Detection: identifying targets based on dynamic noise floor analysis (thresholding).

Visualization: Generates 2D and 3D plots for Range-Doppler surfaces and velocity tracking.

Configuration & Parameters
Important Note: The radar parameters (such as Bandwidth, Chirp Slope, Sampling Frequency, and Max Range) defined in the script are calibrated for the specific ADC dataset used in this demonstration.

If you are using a different dataset or simulation: You must update the System Configuration section in the MATLAB script to match your hardware specifications.

Technologies
MATLAB (Signal Processing Toolbox, Phased Array System Toolbox)

Algorithms: FFT, CFAR (Concept), MTI, Windowing.
