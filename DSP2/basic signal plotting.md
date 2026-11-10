%MATLAb code to plot the sinusoidal signals 

clc; clear all; close all; t = 0:0.0001:0.04; x1 = sin(200*pi*t); x2 = cos(200*pi*t); x3 = sin(200*pi*t + pi/6); x4 = cos(200*pi*t + pi/6); x5 = sin(200*pi*t - pi/6); x6 = cos(200*pi*t - pi/6); figure; subplot(3,2,1); plot(t,x1,'LineWidth',1.5); title('sin(200\pi t)'); xlabel('Time'); ylabel('Amplitude'); grid on; subplot(3,2,2); plot(t,x2,'LineWidth',1.5); title('cos(200\pi t)'); xlabel('Time'); ylabel('Amplitude'); grid on; subplot(3,2,3); plot(t,x3,'LineWidth',1.5); title('sin(200\pi t + \pi/6)'); xlabel('Time'); ylabel('Amplitude'); grid on; subplot(3,2,4); plot(t,x4,'LineWidth',1.5); title('cos(200\pi t + \pi/6)'); xlabel('Time'); ylabel('Amplitude'); grid on; 

subplot(3,2,5); 

plot(t,x5,'LineWidth',1.5); title('sin(200\pi t - \pi/6)'); xlabel('Time'); ylabel('Amplitude'); grid on; subplot(3,2,6); plot(t,x6,'LineWidth',1.5); title('cos(200\pi t - \pi/6)'); xlabel('Time'); 

ylabel('Amplitude'); grid on; 



<!-- Start of picture text -->
1 sin(200r t)<br>mo}<br>© os<br>=f=} 0<br>€<br><.05<br>1<br>0 0.005 0.01 0.015 0.02 0.025 0.03 0.035 0.04<br>Time<br><!-- End of picture text -->



<!-- Start of picture text -->
, cos(200r t)<br>o 0.5<br>mo}<br>an)2<br>£05—<br>-1<br>0 0.005 0.01 0.015 0.02 0.025 0.03 0.035 0.04<br>Time<br><!-- End of picture text -->



<!-- Start of picture text -->
1 sin(2007 t + 77/6)<br>@ 0.5 /<br>0<br>mo}=2<br>—<br><.05<br>-1<br>0 0.005 0.01 0.015 0.02 0.025 0.03 0.035 0.04<br>Time<br><!-- End of picture text -->



<!-- Start of picture text -->
1 cos(2007 t + 77/6)<br>o 0.5<br>mo]<br>5F=} 0<br>—<br>4A4A<br><.054<br>00.005 0.01 0.015 0.02 0.025 0.03 0.035 0.04<br>Time<br>1 sin(200r t - 17/6)<br>o 05<br>a]<br>=p=} 0<br>—<br>£05<br>-1 /<br>0 0.005 0.01 0.015 0.02 0.025 0.03 0.035 0.04<br>Time<br>1 cos(200r t - 17/6)<br>o 05<br>a]<br>=p=} 0<br>—<br>£05<br>4 IN N IN N<br>0 0.005 0.01 0.015 0.02 0.025 0.03 0.035 0.04<br>Time<br><!-- End of picture text -->

