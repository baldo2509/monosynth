# Analog Monosynth

![CC BY-NC-SA 4.0](https://img.shields.io/badge/License-CC%20BY--SA%204.0-lightgrey.svg)

<img 
	src="/Schematics/general_diagram.svg" 
	alt="A block diagram showing the basic structure of the synthesizer."
/>

This is a collection of documentation, schematics, CAD files and code for a
MIDI controlled analog synthesizer with integrated effects and arpeggiator.

## Goals

### Education and fun

* The main goal of this project is to serve as an **easily accessible and inclusive 
teaching tool,** giving people of all ages and backgrounds a chance to **learn 
basic sound design**, along with some **electronics and telecommunications concepts** 
(such as amplitude and frequency modulation), or at the very least the chance to 
by creating interesting sounds on a peculiar instrument.

### Intuitive user experience:

* **'One Knob per Function' design,** which allows for an intuitive understanding 
of the front panel controls without having to know the underlying theory and electronics;

* Although the synthesizer's architecture is based on a modular approach, we have 
opted to __keep the connections between modules hidden,__ so that the user can't 
set up a confusing or potentially dangerous signal flow (for example, a connection 
from a DC control voltage source to the main output could easily damage a speaker);

* The **built-in arpeggiator** makes it very easy for anyone to get something 
that sounds somewhat musical out of the synth, even if they have no experience 
with playing keyboard.

### Versatility

* The 'MIDI to Control Voltage' conversion module can be programmed to _remap the
note pitches to ones that are different
from the standard western chromatic scale:_ this allows us to **play many styles 
of traditional music,** and also to experiment with **micro-tonal compositions.**

### Reliability

* Reliability is very important, as the synthesizer will be used continuously for
many hours at a time, and often by younger demographics that tend to be less careful
around objects; So we have decided to directly build the hardware using PCBs with
SMD technology, as they are extremely reliable. This also has many other advantages,
such as being able to use the PCB fab's in house assembly service, more compact
circuit board designs, and reduced parts costs.

## Modules
### Main Signal Path
* **Input module:** MIDI to Control Voltage converter, arpeggiator 
  and expression wheel controller;
* **2 Voltage Controlled Oscillators**;
* **Sub-Oscillator** (Frequency divider);
* **Audio Source Mixer**;
* **Voltage Controlled Filter** with variable output type 
and dedicated modulation mixer;
* **Voltage Controlled Amplifier**;
* **Output module** with headphone and stereo line output;
### Modulation Sources
* **2 ADSR envelope generators**;
* **Low Frequency Modulation Generator**;
* **Modulation Matrix** for the VCOs;
### Audio effects
* **Distortion**;
* **Chorus** with stereo output;
* **Stereo Delay**;

## Credits

All circuit designs and boards are based on publicly available schematics or
commonly used circuit fragments; for a detailed list of all sources, see the
[CREDITS.md][/CREDITS.md] file.

## License

This project is licensed under the [Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License.](http://creativecommons.org/licenses/by-sa/4.0/)
