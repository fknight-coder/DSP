% Matlab code to generate standard test signal (Continuous Time Signals) 

clc; clear; close all; t = -5:0.01:5; % 1. Impulse impulse = (t == 0); % 2. Unit Step step = (t >= 0); % 3. Exponential alpha = -0.5; exponential = exp(alpha*t); % 4. Unit Ramp ramp = t .* (t >= 0); % 5. Sinc sinc_signal = sinc(t); % 6. Rectangular rectangular = (abs(t) <= 1); figure; subplot(3,2,1); stem(t, impulse, 'LineWidth', 2); title('Impulse Signal'); xlabel('Time'); ylabel('Amplitude'); grid on; subplot(3,2,2); plot(t, step, 'LineWidth', 2); title('Unit Step Signal'); xlabel('Time'); ylabel('Amplitude'); grid on; subplot(3,2,3); plot(t, exponential, 'LineWidth', 2); title('Exponential Signal'); xlabel('Time'); ylabel('Amplitude'); grid on; subplot(3,2,4); plot(t, ramp, 'LineWidth', 2); title('Unit Ramp Signal'); 

xlabel('Time'); ylabel('Amplitude'); grid on; subplot(3,2,5); plot(t, sinc_signal, 'LineWidth', 2); title('Sinc Signal'); xlabel('Time'); ylabel('Amplitude'); grid on; subplot(3,2,6); plot(t, rectangular, 'LineWidth', 2); title('Rectangular Signal'); xlabel('Time'); ylabel('Amplitude'); grid on; 



<!-- Start of picture text -->
q Img Signal ~ 4 Unit Step Signal ~<br>2° ry<br>Bos3 3Zog<br>Bos e<br>& &<br>o2<br>5 4 3 2 a 0 1 2 3 4 5 °5 4 3 2 a 0 1 2 3 4 5<br>15; ExponentialTime Signal ~ 6 Unit RampTime Signal _<br>B10 34<br>E é<br><) <7]<br>d s 4 a a2 4 0——4 2 34 5 dla a a ee<br>Time Tine<br>Sine Signal cD<br>1 ; ar Signal ~<br>$09= 8505)<br>£Pd é3<br>as s 4 2 2 4 0 1 +2 3 4 5 a a er<br>Time ‘Time<br><!-- End of picture text -->

