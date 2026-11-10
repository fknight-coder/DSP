% MATLAB program to find DFT of a discrete-time signal using FFT command 

clc; clear; close all; % Enter input sequence x = input('Enter the sequence x(n): '); % Calculate DFT X = fft(x); % Display DFT values disp('DFT X(k):'); disp(X); % Define index n = 0:length(x)-1; k = 0:length(X)-1; % Plot input signal subplot(2,1,1); stem(n,x,'LineWidth',1.5); grid on; xlabel('n'); ylabel('x(n)'); title('Input Signal'); % Plot DFT magnitude subplot(2,1,2); stem(k,abs(X),'LineWidth',1.5); grid on; xlabel('k'); ylabel('|X(k)|'); title('Magnitude of DFT'); 

# **OUTPUT** 

Enter the sequence x(n): [8 2 1 5 6 2 4 3] DFT X(k): 31.0000 + 0.0000i 0.5858 + 1.5858i 9.0000 + 4.0000i 3.4142 - 4.4142i 7.0000 + 0.0000i 3.4142 + 4.4142i 9.0000 - 4.0000i 0.5858 - 1.5858i 



<!-- Start of picture text -->
8 Input Signal<br>6<br>;2ft)Tootlapy01234587<br>n<br>Magnitude of DFT<br>30<br>25<br>a)<br>x15<br>10<br>5<br>0 01234567<br>k<br><!-- End of picture text -->

