# DSB-SC Demodulation Project


## Project Summary

This project implements DSB-SC (Double-Sideband Suppressed-Carrier) demodulation to recover an original speech signal from a modulated audio file. The system automatically detects the correct carrier frequency and phase through an energy-maximization approach, successfully extracting the hidden Greek word "ανεμος" (wind) from the modulated signal.

##

 ### Core Features

 + DSB-SC Demodulation: Complete implementation of DSB-SC demodulation algorithm

 + Automatic Parameter Detection: Intelligent search for optimal carrier frequency and phase

 + Signal Processing: Advanced filtering and signal recovery techniques

 + Energy Optimization: Uses energy maximization principle for optimal demodulation

 + MATLAB Implementation: Efficient code compatible with MATLAB and Octave

##


### Key Methods and Algorithms

+ Coherent Detection: Uses the same carrier frequency and phase as modulation

+ Energy Maximization: Finds optimal parameters by maximizing signal energy

+ Low-Pass Filtering: FIR filter to remove high-frequency components

+ Grid Search: Exhaustive search over frequency (10-14 kHz) and phase candidates

+ Signal Reconstruction: Recovers original signal using trigonometric identities

##

### File Overview

| File name  | Desccription |
| ------------- | ------------- |
| DCB-SC_DEMODULATION.m | Contains full DSB-SC demodulation and logging.  |
| dsbmix.wav | Input modulated audio file for testing. |
| demodulated.wav | Output recovered audio after demodulation.  |


##

### How to Run
Prerequisites:

  + MATLAB or GNU Octave

  + Audio file `dsbmix.wav` (original modulated signal)

##

### Execution Steps

  1.  Prepare Files: Ensure `dsbmix.wav` is in your working directory

  2.  Run Script: Execute the `DCB-SC_DEMODULATION.m` script in MATLAB/Octave

  3.  View Results: The script will display:

       + Optimal carrier frequency and phase

       + Maximum energy value

       + Generate demodulated.wav output file

   4. Listen to Output: Play   `demodulated.wav` to hear the recovered word
      
##

## Expected Output


	Optimal frequency: 13543 Hz
	Optimal phase: 2.356194 rad
	Maximum energy Ey: 72.206832

