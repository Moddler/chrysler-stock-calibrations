# Chrysler-stock-calibrations
Collection of calibrations pulled from Chrysler ECUs

"Calibration" is the Chrysler term for program-code/content of the EPROM.

This repository is meant to collect various calibrations from Chrysler ECUs, especially the older versions from 80s/90s vehicles equipped with LM/SMEC/SBEC ECUs.

To dump the contents of a chip a EPROM reader can be used. This is difficult on SBECs for example, because the PCB is in a putty to protect it from moisture etc. 

An easier way is to use MPTune and a FTDI interface. The ECU can be bootstrapped and then have the content of the EPROM transmitted by the microcontroller.

A tutorial for this will come.

The folders represent the P/N of the ECU. 
For every .bin there is a .txt holding information of the ECU / verhicle.

Some information can be displayed by a DRB II or SnapOn MT 2500 (therefore it is saved in the calibration itself, but I don't know how to extract this information from the .bin)

Year:	e.g. 1994
Engine:	e.g 3.3L SFI DIS / 3.3L MPI DIS / 2.5L TBI
Emmissions:	e.g. BUX TRUCK MODULE / 50 STATE TRK MODULE
Transmission:	e.g. AUTOMATIC TRANS. / MANUAL TRANS.
Module:	e.g. SBEC-IIB / SBEC-IIA (displayed by a DRB II, MT2500 always shows A) 
P/N-Case: e.g. 04686541 (P/N on the sticker on the ECU)

P/N-Readout:	e.g. 04686541-A (read by a diagnostic tool, DRB II is known to show wrong numbers)
EPROM-Sticker:	e.g. A4686541 (sticker on the EPROM in the putty)
AWD/FWD: AWD / FWD (might be derived from the VIN in the ECU, otherwise count the driveshafts)
EGR:	yes / no (derive from vehicle, might be relevant)
