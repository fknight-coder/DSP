% MATLAB code to find circular convolution of discrete time signals. 

clc; clear; close all; % Take input from user x1 = input('Enter x1(n): '); x2 = input('Enter x2(n): '); % Number of points N = max(length(x1), length(x2)); % Circular convolution y = cconv(x1, x2, N); % Display result disp('Circular Convolution Result:'); disp(y); % Plot x1 subplot(3,1,1); stem(0:length(x1)-1, x1, 'filled'); title('x1(n)'); xlabel('n'); ylabel('Amplitude'); grid on; % Plot x2 subplot(3,1,2); stem(0:length(x2)-1, x2, 'filled'); title('x2(n)'); xlabel('n'); ylabel('Amplitude'); grid on; % Plot output subplot(3,1,3); stem(0:N-1, y, 'filled'); title('Circular Convolution y(n)'); xlabel('n'); ylabel('Amplitude'); grid on; 

# **OUTPUT** 

Enter x1(n): [1,1,1] Enter x2(n): [2,-1,2] Circular Convolution Result: 3 3 3 



<!-- Start of picture text -->
x4(n)<br>» 1<br>3<br>i<9E or05 0 05 1 15 2 25<br>n<br>2 x2(n)<br>Uv<br>21<br>£0<br><405 0 05 15 2 25<br>n<br>3 Circular Convolution y(n)<br>ft<br>ao—————<br><o05 0 05 1 15 2 25<br>n<br><!-- End of picture text -->

