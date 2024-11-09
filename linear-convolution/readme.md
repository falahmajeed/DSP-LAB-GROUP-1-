# MATLAB Convolution of Two Signals

## Aim
To perform the convolution of two signals using both the built-in MATLAB `conv` function and a matrix-based convolution method.

## Theory
Convolution is a mathematical operation used frequently in signal processing, systems analysis, and other areas of engineering. It combines two signals, typically an input signal and an impulse response, to produce a third signal representing the cumulative effect of the two signals.

In this experiment:
- The vector `x` represents the input signal.
- The vector `h` represents the impulse response.
  
### Convolution Using Built-in Function
MATLAB provides the `conv` function to calculate the convolution of two signals. This function directly computes the linear convolution, which results in an output signal `y` whose length is the sum of the lengths of `x` and `h` minus 1.

### Matrix-Based Convolution Method
The matrix-based convolution method involves:
1. **Padding:** Both signals `x` and `h` are zero-padded to match the output length of `y`.
2. **Shifted Matrix Formation:** A matrix, `h_mat`, is formed by circularly shifting the padded impulse response `h` for each column, creating a structured matrix.
3. **Multiplication:** The matrix `h_mat` is multiplied by the padded input signal `x` to yield the convolution result.

This method replicates the convolution process by treating it as a matrix multiplication operation, providing an alternative way to understand and compute convolution.

## Observation
![Output Image](path_to_output_image_here)

