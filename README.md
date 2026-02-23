## Experiment No: 4
INTEGRATOR USING OP-AMP (μA741)
## Aim
To design and simulate an Integrator circuit using μA741 in Proteus Design Suite and verify that the output is proportional to the integral of the input voltage.
## Apparatus Required
•	μA741 Op-Amp
•	Resistor R = 10 kΩ
•	Capacitor Cf = 0.01 µF
•	Signal Generator
•	Dual Power Supply (±15V)
•	CRO / Oscilloscope
•	Connecting wires
## Circuit Diagram
<img width="983" height="576" alt="image" src="https://github.com/user-attachments/assets/581c08f4-78cb-4ecf-a593-7c43762f1a2b" />

## Connection Details:
•	Input signal → Resistor (R) → Inverting terminal (Pin 2)
•	Feedback capacitor (Cf) → Between Output (Pin 6) and Pin 2
•	Non-inverting terminal (Pin 3) → Ground
•	Pin 7 → +15V
•	Pin 4 → −15V
## Theory
An Integrator circuit produces an output voltage proportional to the integral of the input voltage.
## Working Principle:
•	When input is constant → output is ramp signal
•	Output is inverted
•	Output depends on time
For Sine Wave Input:
•	Output lags input by 90°
•	Output amplitude decreases with frequency
## Procedure
1.	Open Proteus software.
2.	Select μA741, resistor, capacitor, signal generator, and CRO.
3.	Connect circuit in integrator configuration.
4.	Apply ±15V power supply.
5.	Set input waveform (1V, 1kHz).
6.	Run simulation.
7.	Observe input and output waveforms on CRO.
## Tabulation

| Sl. No | Input Voltage (Vin) | Time (ms) | Output Voltage (Vout) |
| ------ | ------------------- | --------- | --------------------- |
| 1      | +5 V                | 0 ms      | 0 V                   |
| 2      | +5 V                | 0.5 ms    | –2.5 V                |
| 3      | +5 V                | 1 ms      | –5 V                  |
| 4      | –5 V                | 1.5 ms    | –2.5 V                |
| 5      | –5 V                | 2 ms      | 0 V                   |
| 6      | +5 V                | 2.5 ms    | –2.5 V                |
| 7      | +5 V                | 3 ms      | –5 V                  |

## Waveforms
<img width="985" height="620" alt="image" src="https://github.com/user-attachments/assets/60dbbed6-9cca-42a8-bb57-e101c9a4841a" />

## Result
The Integrator circuit using μA741 Op-Amp was successfully designed and simulated in Proteus.
The output waveform is proportional to the integral of the input signal.
The circuit behaves as an integrator.
## Conclusion
•	Output lags input by 90° (for sine input).
•	Output amplitude decreases with increase in frequency.
•	Used in waveform generation and analog computation.
## Viva Questions
1.	What is an integrator circuit?
2.	Write the output equation of integrator.
3.	Why does output lag input?
4.	What happens at very low frequency?
5.	What is practical integrator?

ANSWER:

1. **Integrator circuit:**
     An op-amp circuit that produces an output proportional to the integral (area) of the input signal. It performs mathematical integration of the input over time.


2.**Output equation:** 
     ( V_{out} = -\dfrac{1}{RC} \int V_{in}, dt ). 
    Output depends on the accumulated input voltage over time.


3. **Why output lags input:**
       Integration smooths and delays the signal since output builds up gradually from the input. Hence the output lags the input in phase.


4.**At very low frequency:** 
      Gain becomes very high, causing drift and possible saturation due to DC components. The circuit may lose stability.


5.**Practical integrator:**  
     A modified integrator with a resistor in parallel with the capacitor to limit low-frequency gain. It prevents saturation and improves stability.

