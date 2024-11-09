# MATLAB Bandpass Filter Design with Different Windows

## Aim
To design a bandpass filter with a specified order and passband frequencies, and to analyze its frequency response using different window functions, including Hamming, Hanning, Rectangular, and Triangular windows.

## Theory
A bandpass filter allows signals within a specified frequency range to pass while attenuating frequencies outside this range. In digital signal processing, filters can be designed using various techniques and then modified using window functions to achieve desired characteristics. 

The MATLAB code accomplishes the following steps:
1. **Filter Order (N):** The filter order determines the steepness and complexity of the filter response.
2. **Sampling Frequency (fs):** The rate at which the signal is sampled, used to normalize the filter frequencies.
3. **Passband Frequencies (fpass):** The range of frequencies that the bandpass filter will allow. This range is specified in Hz, but it is normalized to a fraction of the Nyquist frequency (half of the sampling frequency) for processing.
4. **Ideal Filter Design:** Using the `fir1` function, an ideal bandpass filter is created based on the specified order and normalized passband frequencies.
5. **Window Functions:** Different windows are applied to the filter coefficients to modify the filter characteristics. Each window type impacts the filter response, specifically the sidelobe levels and transition width:
   - **Hamming Window:** Known for reducing sidelobes and providing a smooth roll-off.
   - **Hanning Window:** Similar to the Hamming window but with slightly different sidelobe levels.
   - **Rectangular Window:** Produces the narrowest main lobe but has high sidelobe levels, causing ringing effects.
   - **Triangular Window:** Provides a balance between main lobe width and sidelobe levels.
6. **Frequency Response Plotting:** The `freqz` function is used to plot the frequency response for each windowed filter, showing the magnitude and phase response.

## Observations
*(Paste output images here)*

1. **Hamming Window:**
   
2. **Hanning Window:**
   
3. **Rectangular Window:**
   
4. **Triangular Window:**

## Conclusion
Different window functions impact the filter’s frequency response in terms of sidelobe levels and transition width. Window selection is crucial based on the application's requirements for sidelobe attenuation and frequency resolution.
