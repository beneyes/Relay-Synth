# Relay Synth
Pure Data Patch to sequence two relays as instruments using MIDI - works well with 16 step MIDI sequencers

Instructions for Use

Install PD Extended - although discontinued the patch uses many objects including Gate and Counter - 

Requires Arduino (Pduino object here https://puredata.info/downloads/pduino/releases/0.5

Connect two relays directly to the PWM outputs of the arduino 0 and 1
Use a common ground

Install Arduino Firmata firmware on the arduino
https://firmata.org/

Once Firmata firmware is installed check you have the main Relay Synth.pd patch in the same folder as the arduino.pd object.

Connect your Relays to Analogue outputs 0 and 1 on the arduino
Launch Relay Synth.pd

Open Serial Port and Check Ardunino is running on the USB port ok and detected.

Set Pin modes to PWM and select 0 and 1 in the blue boxes - this will send analogue out puts for motors or relays. 

Use Mac internal IEC MIDI drivers or MIDI OX on windows to send MIDI from a sequencer to the the Pure Data patch.

You should see activity in the MIDI inputs all being well. 

Higher pitched midi notes will results in faster relay oscillations, lower MIDI notes will give you slow oscillations. 

