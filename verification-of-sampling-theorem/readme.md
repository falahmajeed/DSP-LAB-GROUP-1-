# Sine Wave Sampling and Reconstruction

## Aim:
The objective of this experiment is to explore the effects of different sampling frequencies on the reconstruction of a sine wave. The goal is to demonstrate how signals are reconstructed from samples below, at, and above the Nyquist frequency.

## Theory:
In signal processing, the **Nyquist frequency** is defined as twice the frequency of the signal being sampled. If the sampling rate is less than twice the signal frequency, aliasing occurs, causing distortion in the reconstructed signal. The experiment involves sampling a sine wave at three different frequencies:
- Below the Nyquist rate (undersampling)
- At the Nyquist rate
- Above the Nyquist rate (oversampling)

The reconstruction is done using linear interpolation between the sampled points. The effect of these different sampling rates on signal reconstruction is observed and analyzed by comparing the sampled signals with the original sine wave.

### Key Concepts:
1. **Sampling below Nyquist rate (Fs < 2f)**: This will cause aliasing, and the signal will not be accurately reconstructed.
2. **Sampling at Nyquist rate (Fs = 2f)**: The reconstructed signal will be accurate, as the sampling rate is sufficient to capture all the signal information.
3. **Sampling above Nyquist rate (Fs > 2f)**: This results in an over-sampling situation, where the signal is sampled more than necessary. The reconstructed signal will be very close to the original, but it will also introduce unnecessary data.

## Observation:
_The observation section is left empty for you to paste the output image from the MATLAB simulation._

---

### Plot Details:
1. **Original Sine Wave**: The first subplot shows the continuous sine wave at the user-defined frequency. It serves as the reference for all subsequent reconstructions.
   
2. **Sampling Below Nyquist (Fs < 2f)**: In the second subplot, the sine wave is sampled at a frequency lower than the Nyquist rate. The red stems represent the sampled points, and the green line represents the reconstructed signal. This plot demonstrates aliasing, where the reconstructed signal deviates from the original.
   
3. **Sampling at Nyquist Rate (Fs = 2f)**: The third subplot shows the sine wave sampled at the Nyquist rate. The reconstructed signal should align closely with the original, indicating that the Nyquist sampling theorem has been followed, and no aliasing occurs.
   
4. **Sampling Above Nyquist (Fs > 2f)**: The fourth subplot demonstrates sampling above the Nyquist rate. The signal is sampled more frequently than necessary, but the reconstructed signal still closely follows the original, though it may introduce unnecessary data points.

---

### Conclusion:
From the plots, it is clear that:
- **Below Nyquist**: The reconstructed signal is inaccurate due to aliasing.
- **At Nyquist**: The reconstructed signal perfectly matches the original sine wave.
- **Above Nyquist**: The signal is still reconstructed accurately, but with redundant samples.

This experiment highlights the importance of selecting an appropriate sampling rate to accurately reconstruct a signal without wasting computational resources or introducing errors.
