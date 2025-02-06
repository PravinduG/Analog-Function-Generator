# Analog Function Generator

![Analog Function Generator](Images/Assembly_1.jpg)

## Project Overview
A precise analog function generator capable of generating multiple waveforms in a wide range of frequencies. This is an idea device for electronics enthusiasts to obtain various waveforms they may need.

### Features
- **Waveforms:** Sine, Square, PWM, Triangle, Sawtooth
- **Amplitude:** Adjustable 0-10V output
- **Frequency Range:** 20Hz to 20,000Hz
- **Design:** Build with analog components only.

## Circuit Diagram
![Circuit Diagram](Images/PCBschematic.jpg)

## Components
- **Resistors:** 
- **Capacitors:** 
- **Op-Amps:** LM318n
- **Potentiometers:** For adjusting amplitude, frequency, and PWM duty cycle
- **Power Supply:** +/- 12V DC

## How It Works
The function generator runs on a schmitt trigger oscillator, which uses hysteresis to generate triangle and square waves. These waves are then filtered, amplified, and compared to produce sine, pwm, and sawtooth waveforms.

## PCB
![PCB Photo](Images/PCB.png)
*Caption: PCB.*


## Setup & Usage
1. **Build the Circuit:** Construct the function generator on a PCB or a breadboard, and connect the relevant components.
2. **Power the Circuit:** Connect the +/-12V DC power supply.
3. **Select Waveform:** Select the desired waveform using the selector switch.
4. **Adjust Amplitude, Frequency & PWM Duty cycle:** Select the desired output frequency, amplitude, and PWM duty cycle using the relevant potentiometers and switches.
5. **Connect to Oscilloscope:** Connect to an oscilloscope and verify the output.

## Output Results
![Sine Wave](Images/sine_10kHz_10v.jpg)
*Caption: Output sine waveform.*

![FFT Sine Wave](Images/sine_10kHz_fft.jpg)
*Caption: FFT of the sine waveform.*

![Square Wave](Images/square_10kHz_10V.jpg)
*Caption: Output square waveform.*

![PWM Wave 80%](Images/PWM_10kHz_0.8duty.jpg)
*Caption: Output PWM waveform at 80% duty.*

![PWM Wave 1%](Images/PWM_10kHz_0.01duty.jpg)
*Caption: Output PWM waveform at 1% duty.*

![PWM Wave 99%](Images/PWM_10kHz_0.99duty.jpg)
*Caption: Output PWM waveform at 99% duty.*

![Triangle Wave](Images/triangle_10kHz_10v.jpg)
*Caption: Output triangle waveform.*

![Sawtooth Wave](Images/sawtooth_10kHz_10v.jpg)
*Caption: Output sawtooth waveform.*


## Challenges Faced
- **Stability:** Maintaining stability and symmetry across the entire range for the sawtooth waveform.
- **Component Selection:** Selecting readily available components that met the performance requirements of our design.
- **Variable Cut-Off Filter:** Creating a filter that would vary it's cut-off, in tune with the frequency of the oscillator.

## Future Improvements
- **Extended Frequency Range:** Increase the stability at higher frequencies.
- **Improved output stage:** Redesigning the output stage to be able to drive smaller loads.

