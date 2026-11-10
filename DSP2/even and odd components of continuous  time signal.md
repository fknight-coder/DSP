% Matlab code to find even and odd components of continuous time signal clc; clear; close all; % Define symbolic variable syms t % Enter signal equation x = input('Enter the signal x(t): ','s'); % Convert input into symbolic expression x = str2sym(x); % Find x(-t) x_neg = subs(x,t,-t); % Find even component x_even = simplify((x + x_neg)/2); % Find odd component x_odd = simplify((x - x_neg)/2); % Display even component fprintf('\nEven Component:\n'); disp(x_even); % Display odd component disp('Odd Component:'); disp(x_odd); % Convert symbolic expressions to functions for plotting f = matlabFunction(x); f_even = matlabFunction(x_even); f_odd = matlabFunction(x_odd); % Define time T = -2:0.01:2; 

# **OUTPUT** 

Enter the signal x(t): 1 + 2*t + 3*t^2 + 4*t^3 

Even Component: 3*t^2 + 1 Odd Component: 4*t^3 + 2*t 

