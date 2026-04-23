# Chapter 11: Fourier Expansion and FFT

## Overview
This lab focuses on using Fourier series to approximate a periodic pulse waveform and analyzing its frequency content using FFT.

## Signal Specifications from student ID code
- Frequency: 4 kHz
- Peak-to-peak voltage: 2 V
- Duty cycle: 20%

## Method
Python was used to compute the Fourier series coefficients and reconstruct the signal using a finite number of harmonics (N = 7). The approximation was plotted and compared to the expected waveform behavior.

The signal was then implemented in Scopy using the ADALM2000 to compare the theoretical Fourier approximation with a real pulse signal. The oscilloscope and spectrum analyzer were used to observe both time-domain and frequency-domain behavior.

The measured data was exported and analyzed in LTspice, where a low-pass filter with cutoff frequency equal to one-tenth of the signal frequency was applied. The transient response and FFT were observed after filtering.

## Key Concepts
- Fourier series approximation
- Harmonic content of pulse signals
- FFT analysis
- Effects of low-pass filtering

## Results
The Fourier approximation captured the general shape of the pulse waveform but showed ringing near discontinuities due to the limited number of harmonics (Gibbs phenomenon). The FFT showed harmonic peaks at integer multiples of the fundamental frequency. The low-pass filter reduced higher-frequency components, smoothing the waveform.

## Files
- Python code for Fourier expansion
- Plots of waveform approximation (N=7)
- Scopy oscilloscope and FFT screenshots
- LTspice schematic and FFT results
