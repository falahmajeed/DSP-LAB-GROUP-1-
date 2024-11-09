# Discrete Fourier Transform (DFT) in MATLAB

## Aim
To calculate and visualize the Discrete Fourier Transform (DFT) of a discrete-time signal \( x[n] = [1, 2, 3, 4] \) using MATLAB's built-in `fft` function and a manually implemented DFT formula.

## Theory
The Discrete Fourier Transform (DFT) is a mathematical technique used to analyze the frequency components of discrete signals. Given a signal \( x[n] \) with \( N \) points, the DFT \( X[k] \) is defined as:

\[
X[k] = \sum_{n=0}^{N-1} x[n] \cdot e^{-j \frac{2 \pi k n}{N}}
\]

where:
- \( x[n] \) is the input signal.
- \( X[k] \) represents the DFT output, which is a complex sequence that provides both amplitude and phase information about the signal at different frequencies.
- \( N \) is the total number of samples in \( x[n] \).
- \( k \) is the frequency index, ranging from \( 0 \) to \( N-1 \).

The DFT allows for the transformation of a time-domain signal into its frequency-domain representation, providing insights into the signal's frequency content.

### Key Steps in the Code
1. **Using MATLAB's `fft` function**:
   - `fft(x)` computes the DFT of the input signal using an efficient algorithm.
   - The code displays the magnitude of the result to observe the frequency components.

2. **Manual DFT Calculation**:
   - The code implements the DFT formula explicitly by iterating over each frequency component \( k \) and summing over all time-domain samples \( n \).
   - This approach, while computationally less efficient than `fft`, serves as a demonstration of the DFT calculation.

3. **Plotting**:
   - The code visualizes the magnitude of the DFT results using `stem`, which provides a clear view of the signal's frequency content.

## Observations
Insert your output images here.

## Conclusion
The code successfully calculates the DFT of the signal \( x[n] \) using both MATLAB's built-in `fft` function and a manually implemented DFT formula. The plots of the magnitude show the frequency components of the signal, giving insight into the distribution of energy across different frequencies.
