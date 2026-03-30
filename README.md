# Digital-Signal-Processing--Correlation
## AIM:
To generate discrete auto correlation and cross correlation of signals using MATLAB.
## APPARATUS REQUIRED:
MATLAB R2012.
## ALGORITHM:
Step 1: Open matlab. Write the program.

Step 2: Read the input sequence 1 and input sequence 2 sequence.

Step 3: Perform auto correlation and cross correlation for both the sequences. 

Step 4: Plot the output sequence with x-label and y-label with suitable title.

Step 5: Terminate the program.


## PROGRAM: 

```
clc; % clear screen
clear all; % clear screen
close all; % close all figure windows
% INPUT SIGNAL-1
a=input('enter the starting x(n)');
x=input('Enter the x(n) sequence');
n=a:1:length(x)+a-1;
figure(1)
stem(n,x)
xlabel('Time')
ylabel('Amplitude')
title('Input Signal-1')
% INPUT SIGNAL 2
b=input('enter the starting y(n)');
y=input('Enter the y(n) sequence');
m=input('enter the ending of y(n)');
n1=b:1:length(y)+b-1;
figure(2)
stem(n1,y)
xlabel('Time')
ylabel('Amplitude')
title('Input signal-2')
% DISCRETE AUTO CORRELATED SIGNAL
out1=xcorr(x,x)
n2=a-m:1:length(out1)+a-m-1;
figure(3)
stem(n2,out1)
xlabel('Time')
ylabel('Amplitude')
title(' Discrete auto correlated waveform')
% DISCRETE CROSS CORRELATED SIGNAL
out2=xcorr(x,y);
n3=a-m:1:length(out2)+a-m-1;
figure(4)
stem(n3,out2)
xlabel('Time')
ylabel('Amplitude')
title(' Discrete cross correlated waveform')

```
## OUTPUT:

<img width="1704" height="969" alt="image" src="https://github.com/user-attachments/assets/1be28c58-5b16-47e9-afe1-bb306d77cd77" />

<img width="1667" height="986" alt="image" src="https://github.com/user-attachments/assets/c8367373-1474-47e4-a2c6-fc64c1e0f778" />

<img width="1681" height="995" alt="image" src="https://github.com/user-attachments/assets/e1e1ab1c-8aad-4c9b-86b6-451d871c9011" />

<img width="1734" height="951" alt="image" src="https://github.com/user-attachments/assets/002bdad9-b686-498b-bda6-edb8a6589a97" />



## RESULT:

![WhatsApp Image 2026-03-30 at 6 27 37 PM](https://github.com/user-attachments/assets/67edeb4a-aa8d-47f5-8aef-7488fd158fc5)
