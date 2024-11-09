# MATLAB Convolution Example

## Aim
To perform and compare the linear and circular convolution of two sequences using MATLAB.

## Theory
Convolution is a fundamental mathematical operation in signal processing used to combine two signals or functions, typically representing an input signal and a system's response. In this experiment, we explore **linear convolution** and **circular convolution**:

1. **Linear Convolution**: This operation gives the output of a linear time-invariant (LTI) system when an input signal passes through it. Linear convolution is typically used for signals of finite length and can be calculated using MATLAB’s built-in `conv` function.

2. **Circular Convolution**: Circular convolution is primarily used when working with periodic signals, applying a wrap-around effect to the convolved result. It can be computed using the Fast Fourier Transform (FFT), which is efficient and commonly used in digital signal processing.

### Steps
1. **Linear Convolution**:
   - Use MATLAB’s built-in `conv` function to calculate the linear convolution of two sequences, \( x \) and \( h \).

2. **Circular Convolution using FFT**:
   - Zero-pad the sequences \( x \) and \( h \) to make their lengths equal to the length of the linear convolution result.
   - Perform FFT on both sequences.
   - Multiply the frequency-domain representations.
   - Apply the inverse FFT to get the circular convolution result in the time domain.

## Observations
- **Linear Convolution Output**:  
  *(Insert output image here)*

- **Circular Convolution Output using FFT**:  
  *(Insert output image here)*

## Conclusion
This experiment demonstrates the use of MATLAB for performing both linear and circular convolution. While linear convolution is straightforward, circular convolution requires transforming the sequences to the frequency domain using FFT, which can be beneficial for processing periodic signals or in applications requiring computational efficiency.
