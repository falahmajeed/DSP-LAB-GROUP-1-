# C Code Explanation

## Aim
The aim of the given C code is to generate a sine wave signal with a specified frequency and sample rate, and store the values of the sine wave in an array.

## Theory
- **Sine Wave**: A sine wave is a mathematical curve that describes a smooth periodic oscillation. It is a continuous wave and can be described by the function:
  \[
  y(t) = A \sin(2\pi f t + \phi)
  \]
  Where:
  - \( A \) is the amplitude.
  - \( f \) is the frequency of the wave.
  - \( t \) is time.
  - \( \phi \) is the phase shift (not used in this code).
  
- **Sampling Rate**: The sampling rate is the number of samples taken per second when capturing a continuous signal. In this case, the sample rate \( Fs \) is 10000 samples per second.

- **Frequency**: The frequency \( f \) of the sine wave is 100 Hz, meaning the wave oscillates 100 times per second.

- **Array**: The sine values are computed for 100 time instances and stored in an array `s[]`.

## Observation
Please paste the output image of the sine wave generated here.

---
Explanation:
1. The program generates a sine wave with a frequency of 100 Hz, sampled at 10 kHz.
2. The sine wave values are calculated using the equation:
   \[
   \sin\left(\frac{2\pi f i}{Fs}\right)
   \]
   where \( f = 100 \) Hz and \( Fs = 10000 \) Hz.
3. The result is stored in an array `s[]`, which can be plotted to visualize the sine wave.

