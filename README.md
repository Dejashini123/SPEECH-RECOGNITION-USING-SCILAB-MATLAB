# EXP 5 : SPEECH RECOGNITION USING SCILAB

## AIM: 

To perform and verify speech recognition using SCILAB. 

## APPARATUS REQUIRED: 
PC installed with SCILAB. 

## PROGRAM : 

//  SPEECH RECOGNITION USING SCILAB
```clc;
close;
n = 0:%pi/50:2*%pi;
x = sin(%pi*n); 

M=input('Enter the downsampling factor');
L=input('Enter the upsampling factor');

downsampling_x = x(1:M:length(x));
disp(x,'Input signal x(n)=');
disp(downsampling_x,'Downsampled Signal');
figure(1);
subplot(2,1,1)
plot2d3(1:length(x),x);
xtitle('original singal')
subplot(2,1,2)
plot2d3(1:length(downsampling_x),downsampling_x);
xtitle('Downsampled Signal by a factor of M');


upsampling_x=[];
for i=1:length(x)
upsampling_x(1,L*i)=x(i);
end
disp(x,'Input signal x(n)=');
disp(upsampling_x,'Upsampled Signal');
figure(2);
subplot(2,1,1);
plot2d3(x);
title('original signal');
subplot(2,1,2);
plot2d3(upsampling_x);
title('Upsampled Signal by a factor of L');
```

## OUTPUT: 
<img width="1918" height="1193" alt="image" src="https://github.com/user-attachments/assets/53e668f4-352a-48f0-978b-2cfbae99fd77" />

<img width="1917" height="1198" alt="image" src="https://github.com/user-attachments/assets/a9c3bb76-abc5-45c9-b4dd-e9da0bf38694" />



## RESULT: 
Thus the speech recognition using SCILAB was performed and verified.
