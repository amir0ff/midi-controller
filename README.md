# 🎚️🎛️🎚️ MIDI Controller on Arduino (Pro) Micro 5V/16MHz

This is a generic MIDI controller for DJs and music producers built on the ATmega32u4 microcontroller.
It has been tested on Native Instrument's Traktor Pro 2 and Ableton Live 10 and should work on other versions alike.

*It doesn't require any external software such as "The Hairless MIDI" since this is a MIDI over USB Class Compliant device.*

### MIDI mapping:
MIDI In can be assigned from the software to any knob, fader or button you map it to. MIDI Out has to be configured in the `readMIDI()` method in the code and mapped in the software.
##### Traktor Pro 2 (MIDI Out) mappings:
* MIDI Channel = 4
* MIDI CC 80 = Filter On (Deck A)
* MIDI CC 81 = Monitor Cue On (Deck A)
* MIDI CC 84 = Deck Focus Selector (Deck A)
* MIDI CC 82 = Filter On (Deck B)
* MIDI CC 83 = Monitor Cue On (Deck B)
* MIDI CC 85 = Deck Focus Selector (Deck B)

Traktor MIDI mappings file: [Download](https://amiroff.me/files/midi-controller-traktor-midi-mappings.tsi)

### Electronic components used:

1. Arduino (Pro) Micro 5V/16MHz (1x)
2. Rotary encoder (1x)
3. 10k Rotary potentiometer (8x)
4. 10k Slide potentiometer (3x)
5. Momentary pushbutton switch (6x)
6. Standard (3501) Blue 3mm diffused LEDs (4x blue, 2x green)
7. 16-Channel Analog/Digital CD74HC4067 Multiplexer (1x)

Fritzing schematics file: [Download](https://amiroff.me/files/midi-controller-fritzing-schematic.fzz)

### USB device name change:
If you want to change your MIDI controller device name go ahead and read this [here](http://liveelectronics.musinou.net/MIDIdeviceName.php).
