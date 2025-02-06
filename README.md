# Analog Function Generator

<img src="Images/Assembly_1.jpg" width="50%">

## Project Overview
A precise analog function generator capable of generating multiple waveforms in a wide range of frequencies. This is an ideal device for electronics enthusiasts to obtain various waveforms they may need.

### Features
- **Waveforms:** Sine, Square, PWM, Triangle, Sawtooth
- **Amplitude:** Adjustable 0-10V output
- **Frequency Range:** 20Hz to 20,000Hz
- **Design:** Build with analog components only.

## Circuit Diagram
<img src="Images/PCBschematic.jpg" width="50%">

## Components
- **Resistors:** 
- **Capacitors:** 
- **Op-Amps:** LM318n
- **Potentiometers:** For adjusting amplitude, frequency, and PWM duty cycle
- **Power Supply:** +/- 12V DC

## How It Works
The function generator runs on a schmitt trigger oscillator, which uses hysteresis to generate triangle and square waves. These waves are then filtered, amplified, and compared to produce sine, pwm, and sawtooth waveforms.

## PCB
<img src="Images/PCB.png" width="50%">
*Caption: PCB.*

## Setup & Usage
1. **Build the Circuit:** Construct the function generator on a PCB or a breadboard, and connect the relevant components.
2. **Power the Circuit:** Connect the +/-12V DC power supply.
3. **Select Waveform:** Select the desired waveform using the selector switch.
4. **Adjust Amplitude, Frequency & PWM Duty cycle:** Select the desired output frequency, amplitude, and PWM duty cycle using the relevant potentiometers and switches.
5. **Connect to Oscilloscope:** Connect to an oscilloscope and verify the output.

## Output Results
<img src="Images/sine_10kHz_10v.jpg" width="50%">
*Caption: Output sine waveform.*

<img src="Images/sine_10kHz_fft.jpg" width="50%">
*Caption: FFT of the sine waveform.*

<img src="Images/square_10kHz_10V.jpg" width="50%">
*Caption: Output square waveform.*

<img src="Images/PWM_10kHz_0.8duty.jpg" width="50%">
*Caption: Output PWM waveform at 80% duty.*

<img src="Images/PWM_10kHz_0.01duty.jpg" width="50%">
*Caption: Output PWM waveform at 1% duty.*

<img src="Images/PWM_10kHz_0.99duty.jpg" width="50%">
*Caption: Output PWM waveform at 99% duty.*

<img src="Images/triangle_10kHz_10v.jpg" width="50%">
*Caption: Output triangle waveform.*

<img src="Images/sawtooth_10kHz_10v.jpg" width="50%">
*Caption: Output sawtooth waveform.*

## Challenges Faced
- **Stability:** Maintaining stability and symmetry across the entire range for the sawtooth waveform.
- **Component Selection:** Selecting readily available components that met the performance requirements of our design.
- **Variable Cut-Off Filter:** Creating a filter that would vary its cut-off, in tune with the frequency of the oscillator.

## Future Improvements
- **Extended Frequency Range:** Increase the stability at higher frequencies.
- **Improved output stage:** Redesigning the output stage to be able to drive smaller loads.
