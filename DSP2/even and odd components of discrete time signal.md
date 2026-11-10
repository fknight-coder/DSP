% Matlab code to find even and odd components of discrete time signal clc; clear; close all; % User-defined discrete time n = input('Enter the values of n: '); % User-defined signal x = input('Enter the values of x(n): '); % Define x(-n) x_neg = fliplr(x); % Calculate even component x_even = (x + x_neg)/2; % Calculate odd component x_odd = (x - x_neg)/2; % Display results fprintf('\nEven Component:\n'); disp(x_even); fprintf('Odd Component:\n'); disp(x_odd); % Plot original signal subplot(3,1,1); stem(n,x,'LineWidth',1.5); grid on; xlabel('n'); ylabel('x(n)'); title('Original Signal x(n)'); % Plot even component subplot(3,1,2); stem(n,x_even,'LineWidth',1.5); grid on; xlabel('n'); ylabel('x_e(n)'); title('Even Component'); % Plot odd component subplot(3,1,3); stem(n,x_odd,'LineWidth',1.5); grid on; xlabel('n'); ylabel('x_o(n)'); title('Odd Component'); 

# **OUTPUT-** 

Enter the values of n: [-2 -1 0 1 2] Enter the values of x(n): [-3 1 2 -4 2] 

Even Component: -0.5000 -1.5000 2.0000 -1.5000 -0.5000 

Odd Component: -2.5000 2.5000 0 -2.5000 2.5000 



<!-- Start of picture text -->
2 Original Signal x(n)<br>20<br>*%-2<br>4 -2.5 -2 -15 -1 -0.5 0 05 15 2 25<br>n<br><!-- End of picture text -->



<!-- Start of picture text -->
2 Even Component<br>x<br>2 -2.5 -2 -15 -1 -0.5 0 05 1 15 2 25<br>n<br><!-- End of picture text -->



<!-- Start of picture text -->
Odd Component<br>2<br>$ )<br>-2<br>-2.5 » -15 -1 -0.5 0 05 15 2 25<br>n<br><!-- End of picture text -->

