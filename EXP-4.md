# AIM:
To obtain Pulse Width Modulation & Demodulation using PCM trainer kit.

# THEORY:
Pulse Width Modulation
This technique of modulation controls the variation of duty cycle of the square wave (With some fundamental frequency) according to the input modulating signal. Here the amplitude variation of the modulation signal is reflected in the ON period variation of square wave. Hence, it is a technique of V to T conversion.
Pulse Width Demodulation
The input signal is Pulse Width Modulated, so the ON time of the signal is changing according to the modulating signal. In this demodulation technique during the ON time of PWM signal one counter is enabled. At the end of ON time, counter gives a particular count, which directly corresponds to- the amplitude -of input signal. Then this count is fed to a DAC. The output of DAC corresponds to
the amplitude of input signal. Thus train of varying pulse widths gives varying count values and accordingly DAC give outputs, which is directly proportional to amplitude of input signal. This is then filtered to get original signal. Thus at the output we get the original modulating signal extracted from PWM wave.
 
# EQUIPMENTS:
Experimental kit DCL -08 Connecting chords
Power supply
20 MHz Dual trace oscilloscope
NOTE: Keep The Switch Faults In Off Position.
 

# PROCEDURE:
Refer to the block diagram (Fig. 2) and carry out the following connections	and switch Connect the Power Supply with proper polarity to the kit DCL-08 and switch it on.
Put jumper JP3 to 2nd position.
Keep CH1 knob of CRO on 1 Volt/ divac. Keep CH2 knob of CRO on 2 Volts/ divac. Keep Times/ div knob on 1 msec.
Keep the CRO in Dual channel (Auto/ TV mode). Use X10 for expansion. After proper triggering of CRO, observe both the signals PWM IN and PWM

# BLOCK DIAGRAM:
<img width="583" height="635" alt="image" src="https://github.com/user-attachments/assets/d65bb3f0-2085-4c10-ad1a-197605f35c6f" />


# TABULATION:
<img width="1600" height="1322" alt="image" src="https://github.com/user-attachments/assets/560f463a-618e-4572-aa89-819b16a5ccc3" />


# MODEL GRAPH:
<img width="512" height="473" alt="image" src="https://github.com/user-attachments/assets/b6501fbc-2066-4374-b1ed-23b1107a34ca" />


# OUTPUT GRAPH:
<img width="1600" height="833" alt="image" src="https://github.com/user-attachments/assets/ecaf621e-08e7-4221-a154-a5be18ae8e01" />


# RESULT:
Thus the pulse width modulated and demodulated signals is generated and output is verified.

