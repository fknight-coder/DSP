% Matlab code to generate standard test signal (Discrete Time Signals) 

clc; clear; close all; n = -10:10; % 1. Impulse impulse = (n == 0); % 2. Unit Step step = (n >= 0); % 3. Exponential alpha = -0.5; exponential = exp(alpha*n); % 4. Unit Ramp ramp = n .* (n >= 0); % 5. Sinc sinc_signal = sinc(n/4); % 6. Rectangular rectangular = (abs(n) <= 1); figure; subplot(3,2,1); stem(n, impulse, 'LineWidth', 2); title('Discrete Impulse Signal'); xlabel('n'); ylabel('Amplitude'); grid on; subplot(3,2,2); stem(n, step, 'LineWidth', 2); title('Discrete Unit Step Signal'); xlabel('n'); ylabel('Amplitude'); grid on; subplot(3,2,3); stem(n, exponential, 'LineWidth', 2); title('Discrete Exponential Signal'); xlabel('n'); ylabel('Amplitude'); grid on; subplot(3,2,4); stem(n, ramp, 'LineWidth', 2); title('Discrete Unit Ramp Signal'); 

xlabel('n'); ylabel('Amplitude'); grid on; subplot(3,2,5); stem(n, sinc_signal, 'LineWidth', 2); title('Discrete Sinc Signal'); xlabel('n'); ylabel('Amplitude'); grid on; subplot(3,2,6); stem(n, rectangular, 'LineWidth', 2); title('Discrete Rectangular Signal'); xlabel('n'); ylabel('Amplitude'); grid on; 



<!-- Start of picture text -->
1 DiscreteImpuise Signal aa 5 DiscretUnit St p e  Signal.on onanan<br>2 3<br>505 Sos<br>EE<br>éé<br>3 % 0 8 % 0 0 5 10 5<br>0 a<br>sc Discrete Exponential Signal = ‘s Discrete Unit Ramp Signal oa<br>31500} 8x8<br>=1000+ | 9 =<br>=E 500 9 5 2Eg<br>ers 10 SCYSSSO POSES POSSE RS ESOS “ B 5 10 15<br>n n<br>: Discrete Sine Signal aa 5 Discrete Rectangular Signal aa<br>$o4 4<br>a Sos}<br>2Eo éE<br>48 30 5 0 5 10 18 3 0 0 i<br>n n<br><!-- End of picture text -->

