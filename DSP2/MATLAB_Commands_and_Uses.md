# MATLAB Commands and Their Uses 

_Simple reference list for Signal Processing / DSP practicals_ 

This document combines the unique MATLAB commands, functions, and operators used in the uploaded practicals. Each item is listed once and explained in simple language. 

## **1. Basic MATLAB Commands** 

|**No.**|**Command**|**Use**|
|---|---|---|
|**1**|clc|Clears the Command Window.|
|**2**|clear|Removes variables from the workspace.|
|**3**|clear all|Clears variables and loaded functions from memory.|
|**4**|close all|Closes all open figure windows.|
|**5**|input()|Takes input from the user.|
|**6**|disp()|Displays values or messages in the Command Window.|
|**7**|fprintf()|Displays formatted text and values.|
|**8**|length()|Finds the number of elements in an array.|
|**9**|zeros()|Creates an array containing zeros.|
|**10**|figure()|Opens a new figure window for plotting.|



## **2. Signal Generation and Mathematical Functions** 

|**No.**|**Command**|**Use**|
|---|---|---|
|**1**|sin()|Generates a sine signal.|
|**2**|cos()|Generates a cosine signal.|
|**3**|exp()|Calculates exponential values.|
|**4**|sinc()|Generates a sinc signal.|
|**5**|abs()|Calculates the absolute value or magnitude.|
|**6**|max()|Finds the maximum value.|
|**7**|min()|Finds the minimum value.|
|**8**|double()|Converts values into double-precision numbers.|
|**9**|angle()|Calculates the phase angle of a complex number in radians.|
|**10**|rad2deg()|Converts radians into degrees.|
|**11**|fliplr()|Reverses the order of elements from left to right.|



## **3. Signal Plotting Commands** 

|**No.**|**Command**|**Use**|
|---|---|---|
|**1**|plot()|Plots continuous-time signals using a line graph.|
|**2**|stem()|Plots discrete-time signals using vertical lines and markers.|
|**3**|subplot()|Divides one figure window into multiple plotting sections.|
|**4**|grid on|Displays grid lines on the graph.|
|**5**|title()|Adds a title to the graph.|
|**6**|xlabel()|Adds a label to the X-axis.|



MATLAB DSP Practical Command Reference  |  Page 1 

|**7**|ylabel()|Adds a label to the Y-axis.|
|---|---|---|
|**8**|legend()|Displays names of different plotted signals.|
|**9**|hold on|Keeps the existing graph and adds another signal to it.|
|**10**|axis()|Sets the limits of the X-axis and Y-axis.|
|**11**|xlim()|Sets the limits of the X-axis.|
|**12**|xticks()|Sets the positions of X-axis tick marks.|
|**13**|yticks()|Sets the positions of Y-axis tick marks.|



## **4. DFT, IDFT and Convolution Commands** 

|**No.**|**Command**|**Use**|
|---|---|---|
|**1**|fft()|Calculates the Discrete Fourier Transform (DFT) using FFT.|
|**2**|ifft()|Calculates the Inverse Discrete Fourier Transform (IDFT).|
|**3**|cconv()|Calculates circular convolution of two signals.|
|**4**|conv()|Calculates linear convolution of two signals.|
|**5**|eval()|Evaluates a MATLAB expression stored as a string.|



## **5. Symbolic Mathematics Commands** 

|**No.**|**Command**|**Use**|
|---|---|---|
|**1**|syms|Creates symbolic variables such as t or x.|
|**2**|str2sym()|Converts a string into a symbolic mathematical expression.|
|**3**|subs()|Substitutes a variable with another value or expression.|
|**4**|simplify()|Simplifies a mathematical expression.|
|**5**|matlabFunction()|Converts a symbolic expression into a MATLAB function.|



## **6. Sampling and Loop Commands** 

|**No.**|**Command**|**Use**|
|---|---|---|
|**1**|for|Repeats a set of statements a specified number of times.|
|**2**|end|Indicates the end of a loop or control block.|
|**3**|reconstruct()|A user-defined function in the sampling program that reconstructs a signal from its<br>samples.|



## **7. Important MATLAB Operators** 

|**No.**|**Operator**|**Use**|
|---|---|---|
|**1**|:|Creates a range of values.|
|**2**|==|Checks whether two values are equal.|
|**3**|>=|Checks whether one value is greater than or equal to another.|
|**4**|.*|Performs element-by-element multiplication.|
|**5**|+|Performs addition.|
|**6**|-|Performs subtraction.|



MATLAB DSP Practical Command Reference  |  Page 2 

|**7**|/|Performs division.|
|---|---|---|
|**8**|*|Performs matrix multiplication or scalar multiplication.|
|**9**|^|Performs a power operation.|
|**10**|()|Used for function arguments and indexing.|
|**11**|[]|Creates an array or matrix.|
|**12**|@|Creates an anonymous function.|
|**13**|%|Used to write comments in MATLAB.|



## **8. Important Commands for Practical Exams** 

Remember these commonly used commands for MATLAB DSP practicals: clc, clear, close all, input(), plot(), stem(), subplot(), fft(), ifft(), conv(), cconv(), abs(), angle(), sinc(), and disp(). 

## **Notes** 

- reconstruct() is a function created inside the sampling program; it is not a standard built-in MATLAB command. 

- The same command may be useful in more than one practical, but it is listed only once in the main command sections. 

- Commands such as plot() and stem() are both plotting functions: plot() is generally used for continuous-time signals, while stem() is generally used for discrete-time signals. 

MATLAB DSP Practical Command Reference  |  Page 3 

