% MATLAB code for DFT using Matrix (Twiddle Factor) Method 

clc; clear; close all; % Enter input sequence x = input('Enter the sequence x(n): '); N = length(x); % Calculate Twiddle Factor Matrix W W = zeros(N,N); for k = 0:N-1 for n = 0:N-1 W(k+1,n+1) = exp(-1j*2*pi*k*n/N); end end % Display Twiddle Factor Matrix disp('Twiddle Factor Matrix W:'); disp(W); % Calculate DFT using matrix method X = W*x(:); % Calculate magnitude and phase magnitude = abs(X); phase = angle(X); % Display results disp('Input Sequence x(n):'); disp(x); disp('DFT X(k):'); disp(X.'); disp('Magnitude of DFT:'); disp(magnitude.'); disp('Phase of DFT in Radians:'); disp(phase.'); disp('Phase of DFT in Degrees:'); disp(rad2deg(phase).'); % Define indices n = 0:N-1; k = 0:N-1; % Plot input signal subplot(3,1,1); stem(n,x,'LineWidth',1.5); grid on; xlabel('n'); ylabel('x(n)'); title('Input Signal'); 

% Plot DFT magnitude subplot(3,1,2); stem(k,magnitude,'LineWidth',1.5); grid on; xlabel('k'); ylabel('|X(k)|'); title('Magnitude of DFT'); % Plot DFT phase subplot(3,1,3); stem(k,rad2deg(phase),'LineWidth',1.5); grid on; xlabel('k'); ylabel('Phase (Degrees)'); title('Phase of DFT'); 

# **OUTPUT** 

Enter the sequence x(n): [1 2 3 4] Twiddle Factor Matrix W: 1.0000 + 0.0000i      1.0000 + 0.0000i      1.0000 + 0.0000i      1.0000 + 0.0000i 1.0000 + 0.0000i      0.0000 - 1.0000i      -1.0000 - 0.0000i      -0.0000 + 1.0000i 1.0000 + 0.0000i     -1.0000 - 0.0000i      1.0000 + 0.0000i      -1.0000 - 0.0000i 1.0000 + 0.0000i     -0.0000 + 1.0000i      -1.0000 - 0.0000i      0.0000 - 1.0000i 

Input Sequence x(n): 1 2 3 4 DFT X(k): 10.0000 + 0.0000i -2.0000 + 2.0000i -2.0000 - 0.0000i -2.0000 - 2.0000i 

Magnitude of DFT: 10.0000 2.8284 2.0000 2.8284 

Phase of DFT in Radians: 0 2.3562 -3.1416 -2.3562 

Phase of DFT in Degrees: 0 135.0000 -180.0000 -135.0000 



<!-- Start of picture text -->
4 Input Signal<br>3<br>£2<br>1<br>0<br>5 0 05 1 15 2 25 3 35<br>a<br>» Magnitude<br>x 0{#__+05 0 08 ++}1 18 of DFT 2 +25 {+f3 38<br>k<br>a Phaseof FT<br>8 00<br>2.<br>$100<br>© 00 a5 ° 08 1 13 2 2 3 38<br>i<br><!-- End of picture text -->

