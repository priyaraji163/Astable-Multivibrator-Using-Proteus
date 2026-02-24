## Experiment No: 5
ASTABLE MULTIVIBRATOR USING 555 TIMER Using Proteus
## Aim
To design and simulate an Astable Multivibrator using NE555 in Proteus Design Suite and observe the continuous square wave output.
## Apparatus Required
•	NE555 Timer IC
•	Resistor R1 = 10 kΩ
•	Resistor R2 = 100 kΩ
•	Capacitor C = 0.01 µF
•	DC Power Supply (5V or 9V)
•	CRO / Oscilloscope
•	Connecting wires
## Circuit Diagram
Pin Configuration of 555 Timer:
•	Pin 1 → Ground
•	Pin 2 → Trigger
•	Pin 3 → Output
•	Pin 4 → Reset (Connected to Vcc)
•	Pin 5 → Control Voltage (Bypass with 0.01 µF capacitor optional)
•	Pin 6 → Threshold
•	Pin 7 → Discharge
•	Pin 8 → Vcc
<img width="509" height="391" alt="ASTABLE" src="https://github.com/user-attachments/assets/6513d600-80e0-4cbc-9ece-079c77180e97" />

## Connections:
•	R1 → Between Vcc and Pin 7
•	R2 → Between Pin 7 and Pins 2 & 6
•	C → Between Pins 2 & 6 and Ground
•	Output → Pin 3
## Theory
•	The NE555 timer is a widely used integrated circuit for generating precise time delays and oscillations. When operated in astable mode, it functions as a free-running oscillator that continuously produces a square wave without any external triggering signal. In this mode, a capacitor connected to the circuit charges through resistors R1 and R2 and discharges through R2 repeatedly. The internal voltage divider of the 555 timer creates two reference levels at 1/3 Vcc and 2/3 Vcc. 
•	When the capacitor voltage reaches 2/3 Vcc, the upper comparator resets the flip-flop and turns ON the discharge transistor, causing the capacitor to discharge. When the voltage falls to 1/3 Vcc, the lower comparator sets the flip-flop, turning OFF the discharge transistor and allowing the capacitor to charge again. This continuous charging and discharging process generates a square wave at the output (Pin 3) and an exponential waveform across the capacitor. The time period of oscillation is given by T=0.693(R1+2R2)CT = 0.693 (R1 + 2R2) CT=0.693(R1+2R2)C, and the frequency depends on the values of R1, R2, and C. Thus, the 555 timer in astable mode acts as a simple and reliable square wave generator used in clock circuits, LED flashers, and pulse generation applications.
## Procedure
1.	Open Proteus software.
2.	Select NE555 IC, resistors, capacitor, and CRO.
3.	Connect circuit in astable configuration.
4.	Apply 5V supply.
5.	Run simulation.
6.	Observe square wave output at Pin 3.
7.	Measure time period and frequency.
## Tabulation
S.No	        R1 (kΩ)	      R2 (kΩ)	       C (µF)	        Theoretical Frequency	          Practical Frequency
<img width="874" height="208" alt="Screenshot 2026-02-23 094953" src="https://github.com/user-attachments/assets/aa96f6e3-17f4-4642-9a73-15015e9529e0" />

## Waveforms
•	Output (Pin 3) → Square wave
•	Capacitor voltage → Exponential charging & discharging waveform
<img width="1368" height="844" alt="Astable wf" src="https://github.com/user-attachments/assets/c267da64-aa48-402d-b02b-7cdd09775487" />


## Result
The Astable Multivibrator using NE555 Timer IC was successfully designed and simulated in Proteus.
A continuous square wave output was obtained.
The practical frequency closely matches the theoretical frequency.
## Conclusion
•	The 555 timer works as a free-running oscillator in astable mode.
•	Frequency depends on R1, R2, and C values.
•	Increasing R or C decreases frequency.
•	Used in clock generation, LED flashing, and tone generation.
## Viva Questions
1.	What are the operating modes of 555 timer?
The 555 timer operates in three modes:

Monostable Mode (One-shot mode)

Produces one single output pulse for a trigger input.

Has one stable state and one quasi-stable state.

Astable Mode (Free-running mode)

Produces continuous square wave output.

No stable state.

Bistable Mode (Flip-flop mode)

Has two stable states (SET and RESET).
2.	What are the threshold levels in astable mode?
In astable mode, the capacitor charges and discharges between:

Upper Threshold Level = 2/3 Vcc

Lower Threshold Level = 1/3 Vcc

These levels are set internally by three 5kΩ resistors (voltage divider inside the IC).
3.	Write the frequency formula.
f=1.44/(R1+2R2)C
C is capacitor
f is frequency in Hz
4.	What is duty cycle?
Duty Cycle is the percentage of time the output is HIGH in one complete cycle.
Ton/Ton+Toff*100%
5.	What happens if R2 increases?
f R₂ increases:

Charging time increases

Discharging time increases

Total time period increases

Frequency decreases

Duty cycle slightly increase
