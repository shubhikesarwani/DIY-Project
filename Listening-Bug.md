# Listening Bug Using Op-Amp 741
This circuit is used to amplify the audio signal received from the the Microphone in the form of voltage so that we can have a clear perception of audio. We can use this circuit for spying i.e., to hear the conversation going on in other room.<br>
<br>The **Listening-bug circuit** uses an op-amp 741 which amplifies the signal we get from the microphone. Then capacitor is used to filter out the DC component of the amplified signal.
## <ins>Materials Required</ins>
1. IC LM741
2. Transistor
   * T1 = 2N2222 (Silicon NPN Transistor)
   * T2 = 2N2907 (Silicon PNP Transistor)
3. MIC1 = Condensor Microphone
4. LS1 = 4Ω Loudspeaker
5. Resistors
   * R1 = 22 KΩ
   * R1 = 1 KΩ
   * R3, R4 = 10 KΩ
   * R5 = 5.7 KΩ
   * VR1 = 100 KΩ
6. Capacitors
   * C1 = 0.2 µF
   * C2 = 470 µF/25V
   * C3 = 250 µF/25V
## <ins>Circuit Diagram</ins>
![circuit](https://user-images.githubusercontent.com/58383754/79870505-b8972100-8400-11ea-9a17-ff093fa08b3d.png)

## <ins>Circuit Description</ins>
 A microphone is a transducer which converts audio signal to voltage in range of milli which further need amplification. A long wire from microphone is connected to inverting input (**pin 2**) of IC1 through resistor R2 and capacitor C1. The output of IC1 from **pin 6** is given to base of transistor T1 and T2.<br>
<br>
![IC-LM741](https://user-images.githubusercontent.com/58383754/79864756-9f3da700-83f7-11ea-9fb6-e1f4b7df10e6.png) 
<br><br>
<br>
 A voltage divider network is designed using two 10K resistors (R3 and R4) in order to set reference voltage at non-inverting pin (**Pin 3**). Pure DC power supply of 9V to 15V is given in **pin 7** where as **pin 4** is grounded. Feedback network is designed using one resistor (R5) and one variable resistor (VR1) as shown in figure. The amplified output is taken from **pin 6** which is used to drive the complementary pair transistor (T1 and T2). There we had used complementary pair in order to provide more power to the speaker. Capacitor C2 is used to filter out the DC component if available any.<br>
<br>![2N2907](https://user-images.githubusercontent.com/58383754/79870752-13c91380-8401-11ea-8822-d1019c529fb1.png)
 ![2N2222](https://user-images.githubusercontent.com/58383754/79865057-2b4fce80-83f8-11ea-8004-bbfcc8f22030.png)

**Note: If there is hissing sound coming from the speaker, then we have to change the power supply unit because we need Pure DC power supply unit. Use battery if possible. Capacitor C3 is used here in order to smooth DC power supply. Before using microphone and speaker, please check the appropriate polarity of these two components.**
## <ins>Reference</ins>
* https://bestengineeringprojects.com/listening-bug-using-op-amp-741/
