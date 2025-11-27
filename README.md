# Digital-Signal-Processing--Convolution

## Aim:
To perform linear convolution using MAT LAB.

## Software Required:
MAT LAB R2012

## Algorithm:
Step 1: Open mat lab. Write the program.

Step 2: Read the first input sequence.

Step 3: Read the second impulse sequence.

Step 4: Plot the input sequences with x-label and y-label with suitable title. 

Step 5: Perform convolution for both the sequences using conv2() function.
  
Step 6: Plot the sequence with x-label and y-label with suitable title

Step 7: Terminate the program.

## PROGRAM: 

```
clc; % clear screen
clear all; % clear screen
close all; % close all figure windows
% INPUT SEQUENCE
a=input('enter the starting x(n)');
x=input('enter the x(n) sequence');
n=a:1:length(x)+a-1;
figure(1);
stem(n,x);
xlabel('time');
ylabel('amplitude');
title('input sequence');
% IMPULSE SEQUENCE
b=input('enter the starting h(n)');
y=input('enter the h(n) sequence');
m=b:1:length(y)+b-1;
figure(2);
stem(m,y);
xlabel('time');
ylabel('amplitude');
title('impulse response')
% LINEAR CONVOLUTION
z=conv2(x,y);
n1=a+b:1:length(z)+a+b-1;
figure(3);
stem(n1,z);
xlabel('time');
ylabel('amplitude');
title( 'linear convolution');
```
## CALCULATION:
![28f48300-6ef6-460b-8bec-a8f358fc03d9](https://github.com/user-attachments/assets/aabea8fc-0f82-4551-a321-44994e56d247)


## OUTPUT:

<img width="1920" height="1080" alt="Screenshot 2025-09-26 153507" src="https://github.com/user-attachments/assets/ef8cee44-130a-436f-8aed-42a291f34d72" />

## RESULT:
![b6fd3a94-ebe2-4f17-a9cb-d47d1b9e89a5](https://github.com/user-attachments/assets/54d81079-a1e6-4989-84a7-8da83f439447)

