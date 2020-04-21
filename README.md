# Listening Bug Using Op-Amp 741
We can use this circuit for spying i.e., to hear the conversation going on in other room.<br>
The **Listening bug** uses on op-amp 741 which amplify the signal we get from the microphone.
## <ins>Materials required</ins>
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
![listening-bug-circuit-using-741](https://user-images.githubusercontent.com/58383754/79861123-80d4ad00-83f1-11ea-9573-5e900e72ffab.png)
## <ins>Circuit Description</ins>
 A microphone is a transducer which converts audio signal to voltage in range of milli which further need amplification. A long wire from microphone is connected to inverting input (**pin 2**) of IC1 through resistor R2 and capacitor C1. The output of IC1 from pin 6 is given to base of transistor T1 and T2.<br>
<br>
![op-amp741](https://user-images.githubusercontent.com/58383754/79862889-66e89980-83f4-11ea-9bb9-e6dc6ef2e3d6.png)
<br>
 A voltage divider network is designed using two 10K resistors (R3 and R4) in order to set reference voltage at non-inverting pin (**Pin 3**). Pure DC power supply of 9V to 15V is given in **pin 7** where as **pin 4** is grounded. Feedback network is designed using one resistor (R5) and one variable resistor (VR1) as shown in figure. The amplified output is taken from **pin 6** which is used to drive the complementary pair transistor (T1 and T2). There we had used complementary pair in order to provide more power to the speaker. Capacitor C2 is used to filter out the DC component if available any.
