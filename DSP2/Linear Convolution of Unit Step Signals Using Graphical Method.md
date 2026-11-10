%MATLAB Program to Find Linear Convolution of unit step with unit step Signal using graphical Method 

clc; clear; close all; % Define tau tau = -5:0.01:5; % Define unit step function u = @(t) double(t >= 0); % Time value t = 2; % Define x(tau) and h(tau) x = u(tau); h = u(tau); % Step 1: Time reversal h(-tau) h_reverse = u(-tau); % Step 2: Time shifting h(t-tau) h_shift = u(t - tau); % Step 3: Multiplication product = x .* h_shift; % Step 4: Convolution result y = tau .* u(tau); % Create figure figure; % 1. x(tau) subplot(6,1,1); plot(tau,x,'LineWidth',1.5); grid on; ylabel('x(\tau)'); title('1. x(\tau) = u(\tau)'); % 2. h(tau) subplot(6,1,2); plot(tau,h,'LineWidth',1.5); grid on; ylabel('h(\tau)'); title('2. h(\tau) = u(\tau)'); % 3. h(-tau) subplot(6,1,3); 

plot(tau,h_reverse,'LineWidth',1.5); grid on; ylabel('h(-\tau)'); title('3. h(-\tau) = u(-\tau)'); % 4. h(t-tau) subplot(6,1,4); plot(tau,h_shift,'LineWidth',1.5); grid on; ylabel('h(t-\tau)'); title('4. h(t-\tau), t = 2'); % 5. Product subplot(6,1,5); plot(tau,product,'LineWidth',1.5); grid on; ylabel('Product'); title('5. x(\tau)h(t-\tau)'); % 6. Convolution result subplot(6,1,6); plot(tau,y,'LineWidth',1.5); grid on; xlabel('t'); ylabel('y(t)'); title('6. y(t) = x(t)*h(t) = tu(t)'); 



<!-- Start of picture text -->
' ‘x(q= uly<br>4432A<br><!-- End of picture text -->



<!-- Start of picture text -->
1hf = ult)<br>5432r<br><!-- End of picture text -->



<!-- Start of picture text -->
'Sshff|=ul<br>*<br>5 4 3 2 r 0 1 2 3 1 5<br><!-- End of picture text -->



<!-- Start of picture text -->
4. hert=2<br>oO<br>4 4 3 2 A 0 1 2 3 4 Hy<br>s Sti<br>a<br>432f0t2345<br>6. y(t) =x) = tut<br>5<br>5432f0{2345<br><!-- End of picture text -->



<!-- Start of picture text -->
t<br><!-- End of picture text -->

