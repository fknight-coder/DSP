- %  MATLAB code to find CIRCULAR CONVOLUTION 

clc; clear; close all; 

x1 =[1,2,3,4]; x2 =[4,1,1,2]; n = 0:3; y = cconv(x1, x2, 4); 

figure('Name', 'Circular Convolution Results'); subplot(3, 1, 1); stem(n, x1, 'filled', 'LineWidth', 1.5); title('Input Sequence x_1(n)'); xlabel('n'); ylabel('Amplitude'); grid on; 

subplot(3, 1, 2); stem(n, x2, 'filled', 'LineWidth', 1.5); title('Input Sequence x_2(n)'); xlabel('n'); ylabel('Amplitude'); grid on; 

subplot(3, 1, 3); stem(n, y, 'filled', 'r', 'LineWidth', 1.5); title('Output Sequence y(n) = [15, 19, 23, 23]'); xlabel('n'); ylabel('Amplitude'); grid on; 



<!-- Start of picture text -->
=| Figure1: Circular Convolution Results x Code}<br>Ope<br>119 4 Input Sequence x,(n) oe<br>©<br>3S<br>=2<br>=<br><<br>o 05 0 05 1 15 2 25 3 35<br>n<br>Input Sequence x,(n) oe<br>4<br>©<br>3<br>Ei<br>=2<br>i=<br><<br>o 05 0 05 1 15 2 25 3 35<br>n<br>Output Sequence y(n) = [15, 19, 23, 23] a<br>@ 20<br>10)<br>=<br><<br>0 05 0 05 1 15 2 25 3 35<br>n<br>7<br><!-- End of picture text -->

%  MATLAB code to find LINEAR CONVOLUTION clear; clc; x1 = [1, 2, 3, 4]; x2 = [4, 1, 1, 2]; y = conv(x1, x2); 

disp('Linear Convolution Result (y):'); disp(y); figure; 

subplot(3,1,1); stem(x1, 'filled'); title('Sequence x1(n)'); grid on; subplot(3,1,2); stem(x2, 'filled'); title('Sequence x2(n)'); grid on; subplot(3,1,3); stem(y, 'filled'); title('Convolved Sequence y(n)'); grid on; 



<!-- Start of picture text -->
A Sequence x1(n) a<br>2He EE<br>05 1 15 2 25 3 35 4 45<br>4 Sequence x2(n) “<br>i<br>2HE<br>05 1 15 2 25 3 35 4 45<br>Convolved Sequence y(n) _<br>20<br>10<br>0<br>1 2 3 4 5 6 7<br><!-- End of picture text -->

