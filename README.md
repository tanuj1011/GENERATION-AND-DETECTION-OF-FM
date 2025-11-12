# GENERATION-AND-DETECTION-OF-FM
## AIM:
To write a program for Frequency Modulation and Demodulation using SCILAB and to observe and measure the frequency deviation and the modulation index of FM.

## EQUIPMENTS REQUIRED

•	Computer with i3 Processor

•	SCI LAB

## THEORY
  Frequency modulation is a type of modulation in which the frequency of the high frequency (carrier) is varied in accordance with the instantaneous value of the modulating signal.
  
  #### FREQUENCY DEVIATION Δf  and MODULATION INDEX m f :
  
  The frequency deviation Δf represents the maximum shift between the  modulated signal
  frequency, over and under the frequency of the carrier.
  
  We define modulation index m f the ratio between Δf and the modulating frequency
  m= Δf / fm


#### FREQUENCY MODULATION GENERATION:
  The circuits used to generate a frequency modulation must vary the frequency of a high frequency signal (carrier) as function of the amplitude of a low frequency signal (modulating signal). In practice there are two main methods used to generate FM.

## ALGORITHM
  1.	Define Parameters:
     
      •	Fs: Sampling frequency.
      •	T: Duration of the signal.
      •	Fc: Carrier frequency.
      •	Fm: Frequency of the modulating signal.
      •	Beta: Modulation index, which controls the extent of frequency deviation.
  2.	Generate Signals:
     
      •	modulating_signal: Sinusoidal signal used for modulation.
      •	carrier_signal: The high-frequency carrier signal.
      •	modulated_signal: FM modulated signal calculated by varying the carrier frequency according to the modulating signal.
      
  3.	FM Modulation:
     
      •	Modulated_signal is obtained by modulating the carrier signal with the modulating signal.
 
  4.	FM Demodulation:
     
      •	Differentiation: Computes the derivative of the modulated signal to extract frequency variations.
      •	Envelope Detection: Takes the absolute value to retrieve the envelope of the signal.
      •	Low-pass Filtering: Applies a Butterworth low-pass filter to smooth the envelope and recover the original modulating signal.
      
  5.	Visualization:
      
      •	Plots the modulating signal, carrier signal, FM modulated signal, and demodulated signal for analysis.


## PROCEDURE

    •	Refer Algorithms and write code for the experiment.
    •	Open SCILAB in System
    •	Type your code in New Editor
    •	Save the file
    •	Execute the code
    •	If any Error, correct it in code and execute again
    Verify the generated waveform using Tabulation and Model Waveform

## MODEL GRAPH:
<img width="512" height="365" alt="image" src="https://github.com/user-attachments/assets/dfe6bc64-2b6f-4afa-ae79-95391859ab04" />

## PROGRAM
// --- Parameters for FM Signal ---
clc; // Clear console
clear; // Clear variables
close; // Close graphics windows

Ac = 8.1;      // Carrier Amplitude
Am = 16.2;      // Message Amplitude
fc = 79300;    // Carrier Frequency (Hz)
fm = 793;     // Message Frequency (Hz)
m = 5;       // Modulation Index (beta)

Fs = 10 * fc; // Sampling Frequency (must be > 2*fc for carrier)
t_end = 2 / fm; // Duration (e.g., 2 cycles of message signal)
t = 0:1/Fs:t_end; // Time vector

// --- Signal Generation ---

// 1. Message Signal (m(t))
Vm = Am * sin(2 * %pi * fm * t);

// 2. Carrier Signal (c(t))
Vc = Ac * cos(2 * %pi * fc * t);

// 3. FM Modulated Signal (Vfm(t))
// The phase term is: (2*%pi*fc*t) + m*sin(2*%pi*fm*t)
Vfm = Ac * cos((2 * %pi * fc * t) + m * sin(2 * %pi * fm * t));

// --- Plotting the Signals ---
scf(0); // Create new figure window

subplot(3, 1, 1);
plot(t, Vm);
title('Modulating Signal (Message)');
xlabel('Time (s)');
ylabel('Amplitude');

subplot(3, 1, 2);
plot(t, Vc);
title('Carrier Signal');
xlabel('Time (s)');
ylabel('Amplitude');

subplot(3, 1, 3);
plot(t, Vfm);
title('Frequency Modulated Signal');
xlabel('Time (s)');
ylabel('Amplitude');
## TABULATION
![WhatsApp Image 2025-10-17 at 22 43 34_5d1310e6](https://github.com/user-attachments/assets/c3851496-c499-431a-8673-306fb95f3a4f)

## CALCULATION
![WhatsApp Image 2025-10-17 at 22 07 12_af1fa808](https://github.com/user-attachments/assets/75c16d95-1f35-4085-936d-6c5564588c1a)

## OUTPUT
![WhatsApp Image 2025-11-12 at 20 58 06_70875eb2](https://github.com/user-attachments/assets/5b550930-98f7-491e-a798-2a6eab9be432)

## RESULT
Thus the frequency modulation and demodulation is successfully done and the output is experimentally verified.
