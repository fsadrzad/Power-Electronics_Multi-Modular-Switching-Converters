# Power-Electronics_Multi-Modular-Switching-Converters

Four boards were designed, fabricated, tested, programmed, and interconnected towards the goal of making a multi-modular switching DC/DC converter. This project was done under the supervision of Dr. Amirnaser Yazdani. The project included the making of four boards: 1) a main switching board,  2) an isolated voltage sensing board, 3) an isolated dual-channel current sense board, and 4) an interface board for connecting multiple copies of boards 1-3 together. The main switching converter pre-charged a capacitor to prepare the multi-modular conversion. It also allowed for the full control of an h-bridge onboard. The switching board featured galvanic isolation from the input and fail-safe capabilities. Multiple switching boards can be wired in series in order to add additional stepwise resolution to the switching waveforms, therefore able to generate pseudo-analog waveforms, with a very low output impedance. Using such a setup, power waveforms can be generated at much higher efficiencies than class A, B, AB amplifiers. Such a setup is different than class D amplifier, since it does not rely on pulse-width-modulation, though yet capable of emulating the switching behavior of a class D amplifier. 

The voltage sense board was made as a supervisory accessory. This device is able to measure floating differential high voltages and translate them into a down-scaled common-grounded analog voltage that can be sensed using the central controller. This board provides 5kV of galvanic isolation between its input and its output to the controller. 

The current sense board contains two HAL effect sensors that can translate a current magnitude into a proportional voltage that can be sensed by the main controller. This device also provides high voltage galvanic isolation between its inputs and the controller. 

The interface board allows for the convenient connection between multiple copies of the switching, voltage-sense, and current-sense boards with the main controller (daughter boards). The interface board also featured on-board regulation for powering multiple daughter boards. It also features coil drivers for contactors. In this scenario, a National Instruments (NI) control module was used to control the switching action across all of the boards. 
