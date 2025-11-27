# AUTOCORRELATION-AND-PSD

# Aim
Write a program for Autocorrelation and Power Spectral Density (PSD) of signals in Scilab and verify the Wiener–Khinchin relation.

# Equipments Needed

Computer with Intel i3 processor (or higher)

Scilab software

# Theory

The Wiener–Khinchin theorem states that:

The Power Spectral Density (PSD) of a wide-sense stationary random process is the Fourier Transform of its autocorrelation function.

<img width="466" height="74" alt="image" src="https://github.com/user-attachments/assets/2112c284-5506-4e88-8764-ac5e13f198ae" />

 # Algorithm
 ```
Load or Define the Signal: Input your time-domain signal.

Compute Autocorrelation: Calculate the autocorrelation function of the signal.

Compute Power Spectral Density (PSD):

Estimate the PSD using either:

Fourier Transform of the autocorrelation function, or

Methods like Welch’s periodogram.

Plot Results: Visualize both the autocorrelation function and PSD.
```

# Procedure

Refer to the algorithm and write the code for the experiment.

Open Scilab on your system.

Type your code in a new editor.

Save the file.

Execute the code.

If any errors occur, debug and re-run the program.

Verify the generated waveform using tabulation and model waveform comparison.

 # PROGRAM:
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

# OUTPUT:

<img width="763" height="689" alt="image" src="https://github.com/user-attachments/assets/6dc167cc-41e2-4a92-84e9-00d341736096" />

<img width="963" height="1280" alt="image" src="https://github.com/user-attachments/assets/ee799c5c-3fe0-44e0-94c4-5d727d7f5c79" />

# Result:

Thus the Autocorrelation and PSD are executed in Scilab and output is verified.
