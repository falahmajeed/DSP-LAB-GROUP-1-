# MATLAB Convolution Code Explanation

## Aim
To perform both linear and circular convolution of two discrete-time signals using MATLAB.

## Theory
In signal processing, convolution is a mathematical operation on two functions, resulting in a third function that expresses how the shape of one function is modified by the other. There are two primary types of convolution:

1. **Linear Convolution**: Linear convolution of two discrete-time signals `x` and `h` produces a result whose length is the sum of the lengths of the two sequences minus one. MATLAB provides the `conv()` function to perform linear convolution, which computes the convolution by sliding one signal over the other and summing the element-wise products.

2. **Circular Convolution**: Circular convolution, unlike linear convolution, assumes that the sequences are periodic. This means that when the signals overlap, the end of one sequence wraps around to meet the beginning of the other. Circular convolution can be achieved by modifying the linear convolution result to match the length of the original signals, adjusting for the periodic boundary conditions.

In this code, we begin with two signals `x` and `h`, perform a linear convolution using the MATLAB `conv()` function, and then modify the result to simulate circular convolution.

## Observations
*(Paste output image here)*

---

### Explanation of Code Segments

1. **Input Signals**:
   - `x` and `h` are defined as arrays representing the two signals for convolution. 

2. **Linear Convolution**:
   - The code uses `conv(x, h)` to compute the linear convolution of `x` and `h`.
   - The resulting sequence, `x_conv`, has a length of `length(x) + length(h) - 1`.

3. **Adjusting for Circular Convolution**:
   - To create the effect of circular convolution, the code modifies `x_conv` to match the length of the longer signal (`new_len`).
   - Any extra elements in `x_conv` are wrapped around and added to the beginning elements to simulate the circular nature of the convolution. The modified sequence is stored in `x_new`.

4. **Plotting Results**:
   - The code creates three subplots:
     - `x[n]`: The original signal `x`
     - `h[n]`: The original signal `h`
     - `x[n]*h[n]`: The result of the modified circular convolution

Each subplot includes titles and labels for clarity.

---

## Conclusion
The code demonstrates both linear and circular convolution of discrete-time signals using MATLAB. The linear convolution is achieved using MATLAB's built-in `conv()` function, while the circular convolution is simulated by adjusting the linear convolution result.

