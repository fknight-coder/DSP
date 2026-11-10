%matlab code for Overlap-Add method clc; clear; close all; % Input sequences x = input('Enter input sequence x(n): '); h = input('Enter impulse response h(n): '); % Lengths L = length(x); M = length(h); % Choose block length N = 5; K = N + M - 1; % Initialize output y = zeros(1, L + M - 1); % Overlap-Add method for i = 1:N:L block = x(i:min(i+N-1,L)); temp = conv(block,h); y(i:i+length(temp)-1) = ... y(i:i+length(temp)-1) + temp; end % Display output disp('Output using Overlap-Add method:'); disp(y); % Plot output stem(0:length(y)-1,y,'filled'); xlabel('n'); ylabel('y(n)'); title('Overlap-Add Convolution'); grid on; 

# **Output** 

Enter input sequence x(n): [1 2 3 4 5 6 7] Enter impulse response h(n): [1 0 2] Output using Overlap-Add method: 1 2 5 8 11 14 17 12 14 



<!-- Start of picture text -->
48 Overlap-Add Convolution<br>16<br>14<br>12<br>_. 10<br>€<br>><br>8<br>6<br>4<br>2<br>0 012345678<br>n<br><!-- End of picture text -->

