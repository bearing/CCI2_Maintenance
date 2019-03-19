# Cryogenics for CCI-2

As with all germanium-based gamma-ray spectrometers, CCI-2 must be operated at
cryogenic temperatures. 
Cryogenic temperatures are achieved via the use of non-recycled liquid nitrogen
(LN<sub>2</sub>).
The CCI-2 system is not currently equipped with mechanical cooling nor
LN<sub>2</sub> recycling capabilities, and must be kept cold by regular of 
dewar with LN<sub>2</sub>.

## General Overview

The cart on which CCI-2 is mounted contains a standard 30L dewar.
A vertical coldfinger thermally links the inside of the cryostat to the 
LN<sub>2</sub> bath in the dewar.
The temperature inside the cryostat is measured via a temperature sensor 
inserted in a port on the bottom of the cryostat and connected to a digital
display typically kept on top of the uninterruptible power supply (UPS).
**N.B.** The cables for the temperature sensor near the cryostat port are
frayed - avoid placing undue strain on the cabling (be especially careful when
rotating the dewar). If the digital temperature sensor is giving an unexpected
readaing (e.g. 00000 or XXXXX), gently adjust the cable for the temperature
sensor while monitoring the digital display to see if the display recovers.
If the temperature display cannot be recovered, consult your advisor.

Historically, CCI-2 has attained a minimum temperature of 88K.
This temperature is generally only achieved right after cooling the detector
down from room temperature (sometimes referred to as "cryo-pumping") with the
detectors unbiased and the preamplifiers unpowered.
Powering the preamplifiers typically raises the cryostat temperature by ~1.5K,
and applying bias to the detectors raised the temperature by an additional 
0.5-1.5K.
Thus the minimum temperature typically attained while CCI-2 is in operation is
around 90.5 - 92K.
As the vacuum slowly degrades over time, the median temperature in the 
cryostat tends to increase at the rate of approximately 1 K per month.
CCI-2 can be safely operated with no observable degradation in spectroscopic
performance up to about 96 K. At 98K, degradation in energy resolution can 
begin to be observed.
It is recommended that CCI-2 be operated at temperatures less than 96K.
As the temperature rises beyond this point, the detector should be ramped down
and the cryostat pumped using the turbopump (see the Vacuum documentation).

## When to Fill

CCI-2 must be kept cold when in operation.
**Never apply power to the preampflifiers or apply bias to the detectors if
the cryostat temperature is greater than 100K**
Doing so will likely damage the preamplifiers, necessitating replacement (see
the front-end electronics documentation) and may result in damage to the 
detectors themselves.

In addition, it is better to keep CCI-2 at cryogenic temperatures even when
not in regular use.
The segmented contacts were fabricated with amorphous silicon technology.
Amorphous semiconductor contacts of this type have subsequently been shown to
degrade in blocking performance when left at elevated temperatures for 
extended periods.
In the past, CCI-2 has been kept at cryogenic temperatures nearly all of the 
time.
Planned warm-ups have been scheduled during periods when there are not
adequate personnel around to fill (e.g. over the holidays), but these periods
of room-temperature storage have typically lasted 10 days or less.
It is strongly recommended that long periods of room-temperature storage be
avoided.

**The most important thing is that the detector never be allowed to warm up
while bias is applied.**

## Procedure for Filling CCI-2

CCI-2 is filled by transferring LN<sub>2</sub> from a large 150L dewar to the
30L dewar mounted on the cart.
The transfer is typically done by connecting a cryo hose between the two 
dewars and relying on the pressure differential to force LN<sub>2</sub> from
the large dewar into the small.
The large dewars are kept under pressure (typically 22 PSI) while the dewar on
the cart is unpressurized (at atmospheric pressure: 14 PSI).
The procedure for keeping CCI-2 full of LN<sub>2</sub> is broken up into two 
steps that are covered in greater detail in the 
[fill procedure](./fill_procedure.md) and
[dewar exchange procedure](./change_dewar_procedure.md) documents.
