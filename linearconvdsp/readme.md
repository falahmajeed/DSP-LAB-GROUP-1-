# Convolution Operation in Embedded C

## Aim
To implement a convolution operation using two discrete signals, \( x(n) \) and \( h(n) \), in embedded C.

## Theory
Convolution is a mathematical operation used in signal processing to combine two signals and determine the resulting signal. In digital signal processing, convolution between two discrete signals \( x(n) \) and \( h(n) \) is calculated by summing the products of overlapping samples as they shift over one another. Mathematically, for two sequences \( x(n) \) and \( h(n) \), the convolution \( y(n) \) can be expressed as:

\[
y(n) = \sum_{k=0}^{n} x(k) \cdot h(n - k)
\]

where:
- \( x(n) \): The first discrete signal or input.
- \( h(n) \): The second discrete signal, often considered an impulse response.
- \( y(n) \): The resulting output signal after the convolution operation.

The implementation in C makes use of specific memory addresses to store these values, which is typical in embedded systems to control data flow and manage memory directly.

### Key Variables and Memory Allocation
1. **Input Arrays**:
   - `Xn`: Pointer to the memory address for the input signal \( x(n) \).
   - `Hn`: Pointer to the memory address for the impulse response \( h(n) \).
   
2. **Lengths**:
   - `XnLength`: Pointer to the length of the input signal \( x(n) \).
   - `HnLength`: Pointer to the length of the impulse response \( h(n) \).
   
3. **Output Array**:
   - `Output`: Pointer to the memory address where the resulting convolved signal will be stored.

### Process Flow
1. **Initialization and Memory Clearing**: 
   - The output array and extended input arrays are initialized to zero.
   
2. **Convolution Operation**:
   - For each output element \( y(n) \), the program calculates the sum of products between \( x(k) \) and \( h(n - k) \), iterating through overlapping samples as per the convolution formula.

## Observation
<!-- Paste output image here -->

