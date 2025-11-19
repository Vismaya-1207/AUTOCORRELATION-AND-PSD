# AUTOCORRELATION-AND-PSD
PROGRAM:
```
t=0:0.01:2*3.14;
x=(sin(2*t)+cos(2*t));
subplot(3,2,1);
plot(x);
au=xcorr(x,x);
subplot(3,2,2);
plot(au);
v=fft(au);
subplot(3,2,3)
plot(abs(v));
fw=fft(x);
subplot(3,2,4);
plot(fw);
fw2=(abs(fw)).^2;
subplot(3,2,5); 
plot(fw2);
```

OUTPUT:

<img width="763" height="689" alt="image" src="https://github.com/user-attachments/assets/6dc167cc-41e2-4a92-84e9-00d341736096" />
