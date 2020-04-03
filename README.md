# RFFE microcontroller board

The RFFE microcontroller board is, as the name implies, the digital controller for the fully analog BPM RF Front end boards. It sets the attenuator in both boards, measure the thermometer in each board and sets the DAC for the heater, besides doing all the external communication with external systems by Ethernet.

This board is based on the mBED NXP LPC1768, having the same pinout, processor and ethernet controller. Functionally, the main differences are the addition of a clock generator with spread spectrum capabilities, and a new FeRAM IC for non-volatile fast storage. However, the main difference in this version is that it goes through great measures to avoid generating noise in the 500-MHz frequency range from the Ethernet circuitry, which was detected in the RF BPM for Sirius. Besides the spread spectrum clock for ethernet, shielding, extra power line isolation and layout tweaks were incorporated to ease this problem.


![Production board for RFFEuc](https://github.com/lnls-dig/rffe-uc-hw/blob/master/documentation/RFFEuc-board.jpg)

Questions about the project, ask Gustavo "Aylons" Bruno (gustavo.bruno at lnls.br).