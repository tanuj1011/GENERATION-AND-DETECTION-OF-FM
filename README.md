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
<img width="1919" height="1189" alt="image" src="https://github.com/user-attachments/assets/23a7e251-2fba-49e8-91fe-a2ed0572bee9" />


## TABULATION
![WhatsApp Image 2025-10-17 at 22 43 33_85c5bf8d](https://github.com/user-attachments/assets/146f170f-5173-4948-bb9f-49023eddef36)


## CALCULATION
![WhatsApp Image 2025-10-17 at 22 50 15_9959a47d](https://github.com/user-attachments/assets/b2515adb-eab9-4b7f-996e-0409ddb9dd2d)



## OUTPUT
![WhatsApp Image 2025-10-08 at 20 44 34_4529c3b0](https://github.com/user-attachments/assets/c8db5aa1-4f7c-4e0e-8b1f-9f8c369054ce)
<img width="701" height="247" alt="image" src="https://github.com/user-attachments/assets/b528427d-9bfb-43c8-a013-0ac81f51ddbe" />


## RESULT
Thus the frequency modulation and demodulation is successfully done and the output is experimentally verified.
