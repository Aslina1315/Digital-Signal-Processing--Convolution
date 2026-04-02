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
```% Noorul aslina M  [212223050033]

clc; % clear screen
clear all; % clear screen
close all; % close all figure windows

% input sequence
% X[n]={2.5,−3,1,3.5,2, 4,6,−3}  h[n]={3,−4,4.7,3,2,4.5,2.4} 

a = input("enter the starting x(n)");
x = input("enter the x(n) sequence");
n = a:1:length(x)+a-1;
figure(1);
stem(n,x);    
xlabel('time');
ylabel('amplitude');
title('input sequence');

%impulse sequence

b= input('enter the starting h(n)');
y = input('enter the h(n) sequence');
m = b:1:length(y)+b-1;
figure(2);
stem(m,y);
xlabel('time');
ylabel('amplitude');
title('impulse response');

%linear convolution

z = conv2(x,y);
n1 = a+b:1:length(z)+a+b-1;
figure(3);
stem(n1,z);
xlabel('time');
ylabel('amplitude');
title('linear convolutiond');


## OUTPUT:
<img width="1908" height="789" alt="Screenshot 2026-04-02 194017" src="https://github.com/user-attachments/assets/7c5dd5c9-6f73-450a-9624-27018363ab2c" />
<img width="1912" height="797" alt="Screenshot 2026-04-02 194227" src="https://github.com/user-attachments/assets/447af9c4-ce60-48fb-aef7-39a6c776fa4d" />
<img width="1917" height="778" alt="Screenshot 2026-04-02 194244" src="https://github.com/user-attachments/assets/87d1851e-309f-4c4a-8639-81c1fdc9785a" />


## RESULT:
![WhatsApp Image 2026-04-02 at 7 43 27 PM](https://github.com/user-attachments/assets/b299f6c7-90aa-48c7-a73a-fa2af8f51a9f)


