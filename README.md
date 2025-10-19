# Am-using-python
EX NO:5 7.	GENERATION AND DDETECTION  OF AM MODULATION  USING PYTHON

AIM:

To generate and detect the amplitude modulation and demodulation u s i n g COLAB and to calculate modulation index of AM.

EQUIPMENTS REQUIRED

• Computer with i3 Processor

• Goolge COLAB

THEORY:

Modulation can be defined as the process by which the characteristics of carrier wave are varied in accordance with the modulating wave (signal). Modulation is performed in a transmitter by a circuit called a modulator. Need for modulation is as follows: • Avoid mixing of signals • Reduction in antenna height • long distance communication • Multiplexing • Improve the quality of reception • Ease of radiation. Amplitude Modulation is the process of changing the amplitude of a relatively high frequency carrier signal in proportion with the instantaneous value of the modulating signal. The output waveform contains all the frequencies that make up the AM signal and is used to transport the information through the system. Therefore the shape of the modulated wave is called the AM envelope. With no modulating signal the output waveform is simply the carrier signal. Coefficient of modulation is a term used to describe the amount of amplitude change present in an AM waveform. There are three degrees of modulation available based on value of modulation index.
1)Under modulation : m<1, Em < Ec 
2)Critical modulation: m-1, Em = Ec 
3)Over modulation: m>1, Em > Ec

Algorithm

1.	Initialize Parameters: Set the values for carrier frequency, message frequency, and sampling frequency.
2.	Generate Time Axis: Create a time vector for the signal duration.
3.	Generate Message Signal: Define the message signal as a cosine wave.
4.	Generate Carrier Signal: Define the carrier signal as a cosine wave.
5.	Modulate Signal: Apply the AM formula to obtain the modulated signal.
6.	Plot the Signals: Use Matplotlib to plot the message signal, carrier signal, and modulated signal

   PROGRAM:
   ``` 
Am=2.18;
fm=274;
fs=27400;
t=0:1/fs:2/fm;
m=Am*cos(2*3.14*fm*t);
subplot(3,1,1);
plot(t,m);
Ac=3.18;
fc=2740;
c=Ac*cos(2*3.14*fc*t);
subplot(3,1,2);
plot(t,c);
s=(Ac+m).*cos(2*3.14*fc*t);
subplot(3,1,3);
plot(t,s);
```
OUTPUT WAVEFORM:
<img width="700" height="500" alt="image" src="https://github.com/user-attachments/assets/f004379c-fda1-4fde-8c9b-b216249427c3" />

TABULATION:
<img width="800" height="1100" alt="image" src="https://github.com/user-attachments/assets/d1137575-2e04-4a02-ad68-0056340c6554" />

CALCULATION:
1.MA(theory)=am/ac:0.655

2.MA(pratical)=(Emax-Emin)/(Emax+Emin)=0.650

<img width="500" height="800" alt="image" src="https://github.com/user-attachments/assets/b5108360-7c0c-49bb-8dbb-399d53a6f6d8" />

RESULT:

Thus the amplitude modulation and demodulation is experimentally done and the output is verified.


   


