# Athena

_2.1 audio crossover and headphone amplifier_

This is a work-in-progress on a simple 2.1 audio crossover using active 2nd-order RC filters, as well as a headphone amplifier based on the popular CMoy design. The PCBs have not yet been ordered and confirmed.

## Crossover frequency

The crossover frequency is set by the resistors R11-R16 and the capacitors C5-C10. Keep the values for all components the same.

![equation](http://latex.codecogs.com/gif.download?f_c%20%3D%20%5Cfrac%7B1%7D%7B2%5Cpi%20R%20C%7D)

Using a fixed, commonly available 100nF capacitor the following (and more) corner frequencies can be set:

Resistance | Frequency
-----------|----------
22 kOhms   |  72,34 Hz
20 kOhms   |  79,57 Hz
18 kOhms   |  88,42 Hz
16 kOhms   |  99,47 Hz
15 kOhms   | 106,10 Hz
13 kOhms   | 122,48 Hz
12 kOhms   | 132,64 Hz

## Power supply

The unit should be powered by at least 12 volts DC, but no more than 30 volts DC. More voltage will give you higher headroom for greater amplification (headphone) and high-level signal handling, though you should be able to use a regular 12 volts DC power supply for consumer line levels.

__Attention:__ The power supply must _never_ be connected to signal ground because this schematic referencing ground to VCC/2, i.e. the power supply ground is actually the negative voltage rail. Using a wall wart power supply you should not run into any issues. This avoids adding large capacitors in series on the outputs.

## Enclosure

Use Fischer Elektronik KOH-1100 and KOH-2100 case components with lasercut panels from 2mm plexiglas for the enclosure. CAD files for panel cutouts are included.
