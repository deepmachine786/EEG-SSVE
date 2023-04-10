# Brain Computer Interface (BCI) based on Steady State Visual Evoked Potential (SSVEP)


Instructions on how to use this system

1. Download and unzip all files in “Codes” section.

2. Put the Emotiv device on your head and turn it on.

3. Run GUI at: GUI_OpenGl\ by compiling Stimulator_opengl.cpp

4. In BCI2000 package: run batch\FieldTripBuffer_Emotiv.bat with parameters: parms\Emotive_parameteres.prm

5. Turn on your Bluetooth device** and run Android app on it

6. Run Digital_Signal_Processing_MATLAB\onlinify.m (set “Bluetooth_enable” flag variable to 1, if you are connecting to your Bluetooth device for the first time)


* You should have installed MATLAB, “Emotiv EEG 14 channels” device’s driver prior to use this system.

** Bluetooth device means the device you are using to be connected to MATLAB via Bluetooth and call the phone number processed and acquired by MATLAB.


PURPOSE OF THIS PROJECT:- 

This B.Sc. project aims to implement a Brain Computer Interface (BCI) based on Steady State Visual Evoked Potentials (SSVEP) to allow a user to dial a phone number on a visual keypad displayed on a monitor by simply looking at the numbers sequentially. The system requires the user to wear a cap with 14 sensors to acquire brain signals. The system uses channels O1, O2, T7, and T8 of an Emotiv EEG 14 Channel Device for faster signal processing and better results. The acquired signal is transferred to a computer and handled by BCI 2000, a well-known application in the BCI scientific society. Field Trip Buffer is used to pass online data into MATLAB, where a 5Hz-30Hz bandpass filter and a Common Mode Average Filter are applied to eliminate noise. The system then uses the Minimum Energy Combination method to reduce the influence of noise to the minimum possible level. The system also employs a Dynamic Window Size approach to increase accuracy and time efficiency. When all the required numbers are dialed or the user looks at the "Call" button, the digits are sent via Bluetooth to an Android OS to establish a call connection. The graphical interface is designed using OpenGL, and buttons flicker at specific frequencies, except for 12Hz and 16Hz due to their second harmonic frequencies. The source codes and complete software needed to run the system using an Emotiv EEG 14 Channel Device are available.



