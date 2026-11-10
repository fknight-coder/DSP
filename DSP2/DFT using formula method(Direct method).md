% MATLAB code for DFT using formula (Direct method) clc; clear; close all; % Enter input sequence x = input('Enter the sequence x(n): '); N = length(x); % Calculate DFT using the formula X = zeros(1,N); for k = 0:N-1 for n = 0:N-1 X(k+1) = X(k+1) + x(n+1)*exp(-1j*2*pi*k*n/N); end end % Calculate magnitude and phase mag = abs(X); phase = angle(X); % Display results disp('DFT X(k):'); disp(X); disp('Magnitude of DFT:'); disp(mag); disp('Phase in Radians:'); disp(phase); disp('Phase in Degrees:'); disp(rad2deg(phase)); % Define indices n = 0:N-1; k = 0:N-1; % Plot input signal subplot(3,1,1); stem(n,x,'LineWidth',1.5); grid on; xlabel('n'); ylabel('x(n)'); title('Input Signal'); % Plot magnitude subplot(3,1,2); stem(k,mag,'LineWidth',1.5); grid on; xlabel('k'); ylabel('|X(k)|'); title('Magnitude of DFT'); % Plot phase 

subplot(3,1,3); stem(k,rad2deg(phase),'LineWidth',1.5); grid on; xlabel('k'); ylabel('Phase (Degrees)'); title('Phase of DFT'); 

# **OUTPUT** 

Enter the sequence x(n): [1 2 3 4] DFT X(k): 10.0000 + 0.0000i -2.0000 + 2.0000i -2.0000 - 0.0000i -2.0000 - 2.0000i 

Magnitude of DFT: 10.0000 2.8284 2.0000 2.8284 

Phase in Radians: 0 2.3562 -3.1416 -2.3562 

Phase in Degrees: 0 135.0000 -180.0000 -135.0000 



<!-- Start of picture text -->
‘ Input Signal,<br>g2<br>1<br>|<br>ee25 ° 3s 5 eee18 2 eee35 3 ee35<br><!-- End of picture text -->



<!-- Start of picture text -->
o Magnitude<br>SaA 08 ° eeos * 18 of DFT 2 35 3 35<br>«<br><!-- End of picture text -->



<!-- Start of picture text -->
_ Phase<br>3 100 of FT<br>Bo<br>po<br>200<br>08 ° as $ 1s 2 35 3 35<br>«<br><!-- End of picture text -->

