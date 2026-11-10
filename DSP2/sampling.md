%MATLAB code for sampling clc; clear; close all; %% Parameters fm = 1; T = 4; % Original signal t = 0:0.001:T; x = sin(2*pi*fm*t); %% =============== CASE 1 : fs > 2fm =============== fs1 = 10; ts1 = 0:1/fs1:T; xs1 = sin(2*pi*fm*ts1); xr1 = reconstruct(ts1,xs1,t,fs1); figure(1) subplot(3,1,1) plot(t,x,'b','LineWidth',2) grid on title('Original Signal') xlabel('Time (s)') ylabel('Amplitude') xlim([0 4]) xticks(0:1:4) yticks(-1:1:1) subplot(3,1,2) stem(ts1,xs1,'r','filled','LineWidth',1.5) grid on title('Sampling: f_s = 10 Hz > 2f_m') xlabel('Time (s)') ylabel('Amplitude') xlim([0 4]) xticks(0:1:4) yticks(-1:1:1) subplot(3,1,3) 

plot(t,x,'b','LineWidth',2) hold on plot(t,xr1,'r--','LineWidth',2) grid on title('Reconstructed Signal') xlabel('Time (s)') ylabel('Amplitude') legend('Original','Reconstructed') xlim([0 4]) xticks(0:1:4) yticks(-1:1:1) %% =============== CASE 2 : fs = 2fm =============== fs2 = 2; ts2 = 0.25:1/fs2:T; xs2 = sin(2*pi*fm*ts2); xr2 = reconstruct(ts2,xs2,t,fs2); figure(2) subplot(3,1,1) plot(t,x,'b','LineWidth',2) grid on title('Original Signal') xlabel('Time (s)') ylabel('Amplitude') xlim([0 4]) xticks(0:1:4) yticks(-1:1:1) subplot(3,1,2) stem(ts2,xs2,'m','filled','LineWidth',1.5) grid on title('Sampling: f_s = 2f_m (Nyquist Rate)') xlabel('Time (s)') ylabel('Amplitude') xlim([0 4]) xticks(0:1:4) yticks(-1:1:1) subplot(3,1,3) plot(t,x,'b','LineWidth',2) 

hold on plot(t,xr2,'r--','LineWidth',2) grid on title('Reconstructed Signal at Nyquist Rate') xlabel('Time (s)') ylabel('Amplitude') legend('Original','Reconstructed') xlim([0 4]) xticks(0:1:4) yticks(-1:1:1) %% =============== CASE 3 : fs < 2fm =============== fs3 = 1.5; ts3 = 0:1/fs3:T; xs3 = sin(2*pi*fm*ts3); xr3 = reconstruct(ts3,xs3,t,fs3); 

figure(3) subplot(3,1,1) plot(t,x,'b','LineWidth',2) grid on title('Original Signal') xlabel('Time (s)') ylabel('Amplitude') xlim([0 4]) xticks(0:1:4) yticks(-1:1:1) subplot(3,1,2) stem(ts3,xs3,'k','filled','LineWidth',1.5) grid on title('Sampling: f_s < 2f_m (Aliasing)') xlabel('Time (s)') ylabel('Amplitude') xlim([0 4]) xticks(0:1:4) yticks(-1:1:1) 

subplot(3,1,3) plot(t,x,'b','LineWidth',2) hold on 

plot(t,xr3,'r--','LineWidth',2) grid on title('Reconstructed Signal with Aliasing') xlabel('Time (s)') ylabel('Amplitude') legend('Original','Reconstructed') xlim([0 4]) xticks(0:1:4) yticks(-1:1:1) %% =============== Reconstruction Function =============== 

function xr = reconstruct(ts,xs,t,fs) 

xr = zeros(size(t)); for n = 1:length(ts) xr = xr + xs(n)*sinc(fs*(t-ts(n))); end 

End 

# **OUTPUT** 

**CASE 1 : fs > 2fm** 



<!-- Start of picture text -->
1 Original Signal<br>T T<br>§<br>Zo<br>24|1<br>°1 2 3 4<br>Time (8)<br><!-- End of picture text -->



<!-- Start of picture text -->
1 Sampling: f,= 10 Hz > fm<br>g<br>2<br>2411<br>°1 2 3 4<br>Time (6)<br><!-- End of picture text -->



<!-- Start of picture text -->
1 Reconstructed Signal<br>1 T son<br>8 TS Recor<br>Zo<br>24|1<br>°1 2 3 4<br>Time (8)<br><!-- End of picture text -->

**CASE 2 : fs = 2fm** 



<!-- Start of picture text -->
1 origina Signat<br>T i T<br>§<br>Zo)<br>24L1<br>07 Time2 (6) 3 4<br><!-- End of picture text -->



<!-- Start of picture text -->
, Sampling: f= fy (Nyquist Rate)<br>8<br>Zo<br>24L1<br>07 Time2 (6) 3 4<br><!-- End of picture text -->



<!-- Start of picture text -->
Reconstructed Signal at Nyquist Rate<br>= T i T —<br>Zo . Se<br>By > SS aL 1 a LA s =<br>o 7 Time2 (6) 3 4<br><!-- End of picture text -->

**CASE 3 : fs < 2fm** 



<!-- Start of picture text -->
1 Original Signal<br>T i T<br>§<br>Zo)<br>24L1<br>07 Time2 (6) 3 4<br><!-- End of picture text -->



<!-- Start of picture text -->
; Sampling f < 2m (aliasing)<br>8<br>z<br>2411<br>04 Time2 (6) 3 4<br><!-- End of picture text -->



<!-- Start of picture text -->
Reconstructed Signal with Aliasing<br>iF T —— i T = =<br>: oe a a =<br>got. ae 4 oy, “5<br>2 wee “2 a ss<br>ak a L 1 oe L<br>o 7 Time2 (6) 3 4<br><!-- End of picture text -->

