# Ardunio-Drum-Synth
Drum synth made with Arduino Uno and programmed in the Ardunio IDE using the Tone Library

![Primary Wiring Photo](https://github.com/GarrettOrmsby/Ardunio-Drum-Synth/blob/c6de24ea780543889d6bf56a11e9efb0e81b1f03/Main_Wiring.jpg)

Parts list:
- 1 Ardunio Uno or brand alternative
- 6 Tactile Push Button Switches [5 for sounds pads and one to swap between presets] ![Link](https://www.amazon.com/dp/B008DGA9UY?ref=ppx_yo2ov_dt_b_fed_asin_title)
- 15 Jumper Wires
  - 8 to complete circuit and connect all pieces to ground
  - 7 to connect components to the UNO
- Audio Output Compoenent [I used a 3.5mm Stereo Jack to plug into my PC and capture audio but a simple piezo speaker can work as well.](https://www.amazon.com/dp/B07MFKKWG5?ref=ppx_yo2ov_dt_b_fed_asin_title)


The tone library only allows for the output of a single square wave. In order to get a very specific sound/frequency like done in preset 0 for the Ducktails notes asjust starting frequency to the note you want
and only lower the end frequency to around ~Hz lower with a step of 1. This will mostly prevent a note with significant change/drop.

Other effects like Arpeggio and Noise Burst play multple notes very close together to acheive their effects.

Button pins are listed in the header. If using a 3.5mm audio jack 2 10k Resistors are also required and need to connect the speaker pin to the leftmost and rightmost pins of a 5 pin jack. The center pin needs to be connected to ground.

